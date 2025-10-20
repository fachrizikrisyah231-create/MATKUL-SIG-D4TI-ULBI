# MATKUL-SIG-D4TI-ULBI
Tugas Matakuliah Sistem Informasi Geografis

# 🌍 Data GeoJSON Jalan Kampung Srijaya – Tugas Sistem Informasi Geografis (SIG)

## 📖 Deskripsi
Repository ini berisi **data spasial berbentuk GeoJSON** yang merepresentasikan **jaringan jalan (LineString)** di wilayah **Kelurahan Srijaya, Kecamatan Bukit Besar, Kota Palembang**.  
Data ini dibuat sebagai bagian dari tugas praktikum mata kuliah **Sistem Informasi Geografis (SIG)** dengan tujuan memahami bagaimana data geografis disusun, divisualisasikan, dan disimpan secara digital.

---

## 🗺️ Tujuan Tugas
1. Membuat data jalan dalam format **GeoJSON** (LineString).
2. Memastikan data **valid secara sintaks dan semantik** menggunakan [geojson.io](https://geojson.io).
3. Menyimpan hasil GeoJSON ke dalam **repository GitHub**.
4. Menyimpan data ke dalam **database MongoDB**, dengan aturan satu jalan = satu record.

---

## 🧱 Struktur File
- `jalan_kampung.geojson` → berisi data jalan dalam format GeoJSON.
- `README.md` → berisi penjelasan tugas, struktur data, dan langkah-langkah validasi.

---

## 🧭 Tentang GeoJSON
**GeoJSON** adalah format berbasis teks (JSON) yang digunakan untuk menyimpan data geografis.  
Setiap fitur (feature) berisi dua bagian penting:
- **geometry** → bentuk spasial (dalam hal ini `LineString` untuk menggambar jalan).
- **properties** → atribut atau informasi tambahan tentang jalan tersebut.

Elemen	Arti
"type": "FeatureCollection"	Menandakan kumpulan fitur geografis.
"type": "Feature"	Satu fitur (objek) dalam peta, dalam hal ini satu ruas jalan.
"geometry.type": "LineString"	Menandakan bentuknya garis (jalan).
"coordinates"	Menyimpan pasangan nilai longitude dan latitude dari tiap titik pembentuk jalan.
"properties"	Dapat diisi atribut tambahan seperti nama jalan, panjang, atau jenis jalan. (kosong dalam tugas ini).
