---
title: Bahasa Pemrograman Rust
layout: workshop-index
description: Bahasa pemrograman Rust
course-parent: Programming
course-parent-url: ../
tags: rust
---

https://doc.rust-lang.org/rust-by-example/

Aneh-aneh di Rust:

```rust
Connection<PgConnectionManager<NoTls>>
```
Ginian apa artinya di Rust

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

## Attributes

## Types

### Deklarasi Type

### Type Alias

### Option

### Result

## Ownership
