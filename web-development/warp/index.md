---
title: Warp - Rust Web Framework
---

## Trait : Filter
- Merupakan struktur utama pembangun web server Warp
- Filter request HTTP yang dapat dipadupadankan sesamanya
- Mengekstrak data dari request
- Menggabungkan data dari request dengan Filter lainnya
- Merespon request dalam bentuk reply

### Method : and\<F\>(self, other : F) -\> And\<Self, F\> 
- Membentuk Filter baru yang menerapkan Filter ini dan Filter yang menjadi parameter input
- Menggabungkan nilai balikan dari kedua Filter

### Method : or\<F\>(self, other : F) -\> Or\<Self, F\> 
- Membentuk Filter baru yang menerapkan salah satu dari Filter yang ada

### Method : map\<F\>(self, fun: F) -\> Map\<Self, F\> 

### Method : boxed

## Struct : Rejection

## Struct : BoxedFilter
