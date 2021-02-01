---
title: Bahasa Pemrograman Rust
layout: workshop-index
description: Bahasa pemrograman Rust
course-parent: Programming
course-parent-url: ../
tags: rust
---

https://doc.rust-lang.org/rust-by-example/

# Fitur Bahasa

## Pointer

## Generic
- Fungsi utama dari generic adalah membuat type pada function, struct, enum, method menjadi dinamis
- Variabel untuk generic itu bebas gak harus E dan T
- Ada type parameter ada value parameter
- Salah satu kegunaannya adalah agar tipe dari parameter input output **Function**, maupun atribut dari **Struct** menjadi dinamis, tidak terikat type tertentu
- Generic menggunakan angle bracket \<\>

```rust
struct Koordinat<TipeX> {
    x: TipeX,
    y: TipeX,
}
```

- https://doc.rust-lang.org/book/ch10-01-syntax.html
- 

https://stackoverflow.com/questions/58027416/what-are-the-brackets-before-a-function-in-rust

## Trait

Trait dapat menjadi parameter function
```rust
pub fn bersuara(a: &impl Benda) {
    println!("Bersuara seperti ini {}", a.suara());
}
```
## Struct

### Impl
Mendefinisikan method untuk Struct dan Enum

## Attributes

## Types

Type pada setiap item di Rust menunjukan operasi-operasi yang dapat dilakukan item tersebut, dan bagaimana interpretasi dari memory-nya.

Referensi:
- https://doc.rust-lang.org/reference/types.html

### Deklarasi Type

### Type Alias

Dapat digunakan untuk mempersingkat dan menyederhanakan type. Contoh :
```rust
type DBCon = Connection<PgConnectionManager<NoTls>>;
```

### Option

### Result

## Ownership

## Future

# Contoh Script dan Cara Memahaminya

## Contoh 1

```rust
impl<F> FilterBase for BoxingFilter<F>
where
    F: Filter,
    F::Future: Send + 'static,
{
    type Extract = F::Extract;
    type Error = F::Error;
    type Future = Pin<Box<dyn Future<Output = Result<Self::Extract, Self::Error>> + Send>>;

    fn filter(&self, _: Internal) -> Self::Future {
        Box::pin(self.filter.filter(Internal).into_future())
    }
}
```

- Mengimplementasikan Trait FilterBase ke Struct BoxingFilter
