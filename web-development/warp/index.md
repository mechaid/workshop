---
title: Warp - Rust Web Framework
---

## Trait : Filter
- Filter request HTTP yang dapat dipadupadankan sesamanya
- Mengekstrak data dari request
- Menggabungkan data dari request dengan Filter lainnya
- Merespon request dalam bentuk reply

### Method : and\<F\>(self, other : F) -\> And\<Self, F\> 
- Membentuk Filter baru yang menerapkan Filter ini dan Filter yang menjadi parameter input
- Menggabungkan nilai balikan dari kedua Filter
