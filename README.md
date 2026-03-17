# 🌌 Portofolio Ripan Nursalam

> Portofolio digital berbasis HTML statis dengan tema Night Sky + Meteor.  
> Perencanaan Wilayah & Kota · ITENAS Bandung · 2026

---

## 📁 Struktur Folder

```
portofolio-ripan/
│
├── index.html                          ← 🏠 HALAMAN UTAMA (index navigasi)
│
├── 📄 Pages — Tersedia
│   ├── gis_peta.html                   ← 🗺️ GIS & Peta (auto-detect upload)
│   ├── Skripsi.html                    ← 🔬 Skripsi Terminal Leuwi Panjang
│   └── kajian_transportasi_batang_detail.html  ← 🚌 Kajian Transportasi KITB
│
├── 📄 Pages — Segera Dibuat
│   ├── pengalaman_kerja.html           ← 💼 Pengalaman (ATR/BPN, Bappedalitbang, PMM)
│   ├── tugas_kuliah.html               ← 📚 Tugas & Proyek Akademik
│   ├── sertifikat_organisasi.html      ← 🏅 Sertifikat & Organisasi
│   ├── desain_visual.html              ← 🎨 Desain Grafis & Visualisasi
│   └── tentang_saya.html              ← 🪐 Profil, Hobi, Visi Karir
│
└── 📁 peta/                            ← 🗂️ Folder aset peta (untuk gis_peta.html)
    ├── rdtr/
    │   ├── batang_asai_delineasi.png
    │   ├── pola_ruang_singkut.png
    │   └── struktur_ruang_*.png
    ├── analisis/
    │   ├── trip_generation_kitb.png
    │   ├── aksesibilitas_batang.png
    │   └── buffer_analysis_*.png
    ├── tematik/
    │   ├── peta_kependudukan_*.png
    │   ├── penggunaan_lahan_*.png
    │   └── tipologi_terminal_*.png
    ├── topografi/
    │   ├── dem_*.png
    │   ├── kontur_*.png
    │   └── kemiringan_lereng_*.png
    └── lainnya/
        └── (peta lain yang tidak masuk kategori di atas)
```

---

## 🔗 Navigasi Antar Halaman

Setiap halaman detail memiliki tombol **← Portfolio** di sudut kiri atas yang kembali ke `index.html`.

```
index.html
    ├──→ gis_peta.html              (← kembali ke index)
    ├──→ Skripsi.html               (← kembali ke index)
    ├──→ kajian_transportasi_batang_detail.html  (← kembali ke index)
    └──→ [halaman lainnya...]       (← kembali ke index)
```

---

## 🗺️ Cara Menggunakan GIS & Peta (`gis_peta.html`)

Halaman ini memiliki fitur **auto-detect & auto-display** untuk file peta:

### Upload File
1. Buka `gis_peta.html` di browser
2. Drag & drop file peta (PNG/JPG/TIFF/WEBP/PDF) ke zona upload
3. File otomatis **terdeteksi tipenya** berdasarkan nama file:

| Keyword dalam nama file | Kategori Terdeteksi |
|------------------------|---------------------|
| `rdtr`, `pola_ruang`, `delineasi`, `struktur_ruang` | 🔵 RDTR |
| `analisis`, `bangkitan`, `tarikan`, `buffer`, `trip`, `aksesi` | 🟢 Analisis |
| `tematik`, `penduduk`, `lahan`, `tipologi` | 🟣 Tematik |
| `topo`, `kontur`, `dem`, `lereng`, `ketinggian` | 🟡 Topografi |
| *(lainnya)* | 🔴 Lainnya |

### Contoh Penamaan File yang Ideal
```
rdtr_batang_asai_delineasi_2024.png       → auto: RDTR
analisis_bangkitan_kitb_2030.png          → auto: Analisis
tematik_penggunaan_lahan_sarolangun.png   → auto: Tematik
topografi_dem_batang.png                  → auto: Topografi
```

### Fitur Galeri
- **Filter** berdasarkan kategori (RDTR / Analisis / Tematik / Topografi / Lainnya)
- **Lightbox** klik gambar untuk lihat full-screen
- **Navigasi** ← → di lightbox untuk pindah antar peta
- **Folder tree** di sisi kiri menampilkan file yang sudah diupload

---

## 🎨 Tema & Desain

| Elemen | Detail |
|--------|--------|
| **Tema** | Night Sky + Meteor shower |
| **Background** | `#03060f` (hitam langit malam) |
| **Accent utama** | `#7ec8ff` (biru bintang) |
| **Font** | Syne (heading) + Space Grotesk (body) |
| **Animasi** | Bintang berkedip + meteor jatuh (Canvas API) |
| **Warna tiap section** | Biru · Hijau mint · Ungu · Kuning · Merah muda |

---

## 🚀 Cara Deploy

### Opsi 1 — Buka Lokal (paling mudah)
```bash
# Cukup buka index.html di browser
# Klik dua kali index.html di File Explorer
```

### Opsi 2 — GitHub Pages (gratis, bisa diakses siapa saja)
```bash
# 1. Buat repo baru di github.com (misal: ripan-portfolio)
# 2. Upload semua file ke repo
# 3. Settings → Pages → Source: main branch / root
# 4. Akses di: https://[username].github.io/ripan-portfolio
```

### Opsi 3 — Netlify Drop (paling cepat, drag & drop)
```
1. Buka netlify.com/drop
2. Drag seluruh folder portofolio
3. Dapat link publik dalam hitungan detik
```

---

## ✅ Checklist Pengembangan

### Sudah Selesai
- [x] `index.html` — Halaman utama dengan navigasi
- [x] `gis_peta.html` — Galeri peta dengan auto-detect upload
- [x] `Skripsi.html` — Detail skripsi Terminal Leuwi Panjang
- [x] `kajian_transportasi_batang_detail.html` — Kajian KITB Batang
- [x] Tombol ← Portfolio di semua halaman detail

### Perlu Dibuat
- [ ] `pengalaman_kerja.html` — Timeline 3 pengalaman magang
- [ ] `tugas_kuliah.html` — Grid tugas akademik per semester
- [ ] `sertifikat_organisasi.html` — Galeri sertifikat + timeline organisasi
- [ ] `desain_visual.html` — Galeri karya desain
- [ ] `tentang_saya.html` — Bio, hobi, nilai, visi karir

---

## 📞 Kontak

| | |
|--|--|
| **Email** | nursalamripan231@gmail.com |
| **LinkedIn** | linkedin.com/in/ripan-nursalam |
| **Lokasi** | Bandung, Jawa Barat |
| **HP** | (+62) 859-1099-1649 |

---

*Dibuat dengan HTML + CSS + Canvas API · Tidak memerlukan framework atau build tool*
