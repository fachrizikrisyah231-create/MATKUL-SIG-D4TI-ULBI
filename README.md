<img width="1355" height="924" alt="Screenshot 2025-10-20 160346" src="https://github.com/user-attachments/assets/a8d5ccc3-0815-4fca-8fd7-043931876f35" /># MATKUL-SIG-D4TI-ULBI
Tugas Matakuliah Sistem Informasi Geografis

# 🌍 Data GeoJSON Jalan Kampung Srijaya – Tugas Sistem Informasi Geografis (SIG)

## 📖 Deskripsi
Repository ini berisi **data spasial berbentuk GeoJSON** yang merepresentasikan **jaringan jalan (LineString)** di wilayah **Jalan Srijaya Negara Kelurahan Bukit lama, Kecamatan ilir Barat I, Kota Palembang**.  
Data ini dibuat sebagai bagian dari tugas praktikum mata kuliah **Sistem Informasi Geografis (SIG)** dengan tujuan memahami bagaimana data geografis disusun, divisualisasikan, dan disimpan secara digital.

---

## 🗺️ Tujuan Tugas
1. Membuat data jalan dalam format **GeoJSON** (LineString).
2. Memastikan data **valid secara sintaks dan semantik** menggunakan [geojson.io](https://geojson.io).
3. Menyimpan hasil GeoJSON ke dalam **repository GitHub**.
4. Menyimpan data ke dalam **database MongoDB**, dengan aturan satu jalan = satu record.

---

## 📍 Lokasi Penelitian
- **Nama Jalan Utama:** Jalan Srijaya Negara  
- **Kelurahan:** Bukit Lama  
- **Kecamatan:** Ilir Barat I  
- **Kota:** Palembang  
- **Provinsi:** Sumatera Selatan    
- **Wilayah Sekitar:** Demang Lebar Daun, Srijaya Negara, Ogan.
<img width="1355" height="924" alt="Screenshot 2025-10-20 160346" src="https://github.com/user-attachments/assets/4200154d-39f8-42c4-8857-89985e2f5824" />




## 🧱 Struktur File
{
  "type": "FeatureCollection",
  "features": [
    { "type": "Feature", "properties": { ... }, "geometry": { ... } }
  ]
}

---


Elemen	Arti
"type": "FeatureCollection"	Menandakan kumpulan fitur geografis.
"type": "Feature"	Satu fitur (objek) dalam peta, dalam hal ini satu ruas jalan.
"geometry.type": "LineString"	Menandakan bentuknya garis (jalan).
"coordinates"	Menyimpan pasangan nilai longitude dan latitude dari tiap titik pembentuk jalan.
"properties"	Dapat diisi atribut tambahan seperti nama jalan, panjang, atau jenis jalan. (kosong dalam tugas ini).

✅ Validasi GeoJSON

Data ini diuji di situs geojson.io
.
Langkah:

Buka situs geojson.io

Hapus data default

Paste isi file jalan_kampung.geojson ke kolom kiri

Lihat hasil di peta → muncul beberapa garis jalan di area Palembang

📸 Hasilnya:
Semua garis muncul dengan benar → GeoJSON valid secara sintaks dan semantik ✅
