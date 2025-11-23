# 🌡️ Konversi Suhu

<div align="center">

![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-success)
![GUI](https://img.shields.io/badge/GUI-Tkinter-orange)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey)

**Aplikasi konversi suhu dengan GUI modern dan penyimpanan riwayat**

</div>

## 📋 Daftar Isi

- [Gambaran Umum](#-gambaran-umum)
- [Fitur](#-fitur)
- [Instalasi](#-instalasi)
- [Penggunaan](#-penggunaan)
- [Dokumentasi](#-dokumentasi)
- [Contoh Penggunaan](#-contoh-penggunaan)
- [FAQ](#-faq)

## 🚀 Gambaran Umum

**Konversi Suhu** adalah aplikasi konversi suhu modern yang mendukung konversi antara 4 skala suhu utama: Celsius (C), Fahrenheit (F), Reamur (R), dan Kelvin (K). Aplikasi ini dilengkapi dengan antarmuka grafis yang user-friendly, penyimpanan riwayat otomatis, dan berbagai fitur tambahan yang membuat pengalaman konversi suhu menjadi lebih mudah dan menyenangkan.

### ✨ Highlights

- 🎨 **GUI Modern** dengan antarmuka yang intuitif
- 🔄 **Konversi Lengkap** antara 4 skala suhu
- 💾 **Penyimpanan Riwayat** otomatis dalam format JSON
- ⚡ **Konversi Cepat** dengan tombol one-click
- 📊 **Riwayat Terorganisir** dengan timestamp
- 🎯 **Presisi Tinggi** dengan format desimal
- 🚀 **Multi-platform** support

## 🌟 Fitur

### 🔥 Core Features
- **Konversi 4 Arah** - Celsius, Fahrenheit, Reamur, Kelvin
- **Presisi Tinggi** - Hasil dengan 2 angka desimal
- **Validasi Input** - Penanganan error yang elegan
- **Real-time Conversion** - Hasil langsung terupdate

### 💾 Data Management
- **Auto-save History** - Setiap konversi langsung tersimpan
- **JSON Storage** - Format penyimpanan terstruktur
- **Riwayat Terstempel** - Dengan tanggal dan waktu
- **Clear History** - Opsi hapus riwayat
- **Persistent Data** - Data tetap tersimpan setelah aplikasi ditutup

### 🎨 GUI Features
- **Modern Interface** - Desain bersih dan modern
- **Tab System** - Antarmuka terorganisir dengan tab
- **Responsive Design** - Adaptif berbagai ukuran layar
- **Quick Buttons** - Tombol konversi cepat
- **Visual Feedback** - Hasil yang jelas dan mudah dibaca

### ⚡ Utility Features
- **Konversi Cepat** - Tombol one-click untuk konversi populer
- **Copy-Friendly** - Format hasil yang mudah disalin
- **Error Handling** - Pesan error yang informatif
- **Input Validation** - Validasi input otomatis

## 📥 Instalasi

### Prerequisites

- Python 3.7 atau lebih tinggi
- Tkinter (biasanya sudah termasuk dalam instalasi Python)

### Step-by-Step Installation

1. **Download Repository**
   ```bash
   # Jika menggunakan git
   git clone https://github.com/username/super-konversi-suhu.git
   cd super-konversi-suhu
   
   # Atau download manual dan extract
   ```

2. **Buat Virtual Environment (Recommended)**
   ```bash
   python -m venv suhu_env
   
   # Aktifkan virtual environment
   # Windows:
   suhu_env\Scripts\activate
   # Linux/Mac:
   source suhu_env/bin/activate
   ```

3. **Verifikasi Tkinter**
   ```bash
   python -m tkinter
   # Jika muncul window tkinter, berarti sudah terinstall
   ```

4. **Jalankan Aplikasi**
   ```bash
   python main.py
   ```

### Quick Install (Windows)
```bash
# Download semua file ke satu folder
# Double click main.py atau jalankan dari command line
python main.py
```

## 🎮 Penggunaan

### Menjalankan Aplikasi

```bash
python main.py
```

### Basic Usage

1. **Konversi Standar:**
   - Masukkan nilai suhu di field input
   - Pilih satuan asal dari dropdown
   - Pilih satuan tujuan dari dropdown  
   - Klik tombol "Konversi" atau tekan Enter

2. **Konversi Cepat:**
   - Gunakan tombol one-click (C→F, C→R, C→K, F→C, R→C, K→C)
   - Nilai akan dikonversi langsung dari input yang ada

3. **Melihat Riwayat:**
   - Klik tab "Riwayat Konversi"
   - Lihat semua konversi yang pernah dilakukan
   - Gunakan tombol refresh untuk update terbaru

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Enter` | Jalankan konversi |
| `Tab` | Navigasi antara field |
| `Ctrl + Q` | Keluar aplikasi |

## 📚 Dokumentasi

### Rumus Konversi yang Didukung

| Dari | Ke | Rumus |
|------|-----|--------|
| Celsius | Fahrenheit | `(C × 9/5) + 32` |
| Celsius | Reamur | `C × 4/5` |
| Celsius | Kelvin | `C + 273.15` |
| Fahrenheit | Celsius | `(F - 32) × 5/9` |
| Fahrenheit | Reamur | `(F - 32) × 4/9` |
| Fahrenheit | Kelvin | `(F - 32) × 5/9 + 273.15` |
| Reamur | Celsius | `R × 5/4` |
| Reamur | Fahrenheit | `(R × 9/4) + 32` |
| Reamur | Kelvin | `(R × 5/4) + 273.15` |
| Kelvin | Celsius | `K - 273.15` |
| Kelvin | Fahrenheit | `(K - 273.15) × 9/5 + 32` |
| Kelvin | Reamur | `(K - 273.15) × 4/5` |

### File Descriptions

| File | Description |
|------|-------------|
| `main.py` | Entry point aplikasi, menjalankan GUI |
| `konversi_suhu.py` | Kelas untuk semua fungsi konversi suhu |
| `history_manager.py` | Mengelola penyimpanan dan load riwayat |
| `gui.py` | Implementasi antarmuka pengguna dengan Tkinter |


## 💡 Contoh Penggunaan

### Contoh Konversi Populer

```python
# Water boiling point
print(KonversiSuhu.konversi_suhu(100, 'C', 'F'))   # 212.00°F
print(KonversiSuhu.konversi_suhu(100, 'C', 'K'))   # 373.15°K

# Water freezing point  
print(KonversiSuhu.konversi_suhu(0, 'C', 'F'))     # 32.00°F
print(KonversiSuhu.konversi_suhu(0, 'C', 'R'))     # 0.00°R

# Absolute zero
print(KonversiSuhu.konversi_suhu(0, 'K', 'C'))     # -273.15°C
print(KonversiSuhu.konversi_suhu(0, 'K', 'F'))     # -459.67°F

# Room temperature
print(KonversiSuhu.konversi_suhu(25, 'C', 'F'))    # 77.00°F
print(KonversiSuhu.konversi_suhu(25, 'C', 'R'))    # 20.00°R
```

## ❓ FAQ

### Q: Apakah perlu install library tambahan?
**A:** Tidak! Aplikasi ini menggunakan pure Python standard library saja, termasuk Tkinter untuk GUI.

### Q: Bagaimana cara backup riwayat konversi?
**A:** File `history_konversi.json` berisi semua riwayat. Backup file ini untuk menyimpan data.

### Q: Bisakah menambah satuan suhu lain?
**A:** Ya! Structure code sudah modular dan mudah dikembangkan.

### Q: Apakah data riwayat aman?
**A:** Data disimpan lokal di komputer Anda dalam format JSON yang aman.

### Q: Bagaimana cara reset semua data?
**A:** Hapus file `history_konversi.json` dan restart aplikasi.

### Q: Bisakah diintegrasikan dengan aplikasi lain?
**A:** Ya! Module `konversi_suhu.py` bisa diimport dan digunakan di project lain.

### Q: Apakah support high DPI displays?
**A:** Ya, Tkinter secara otomatis menangani scaling untuk high DPI displays.

---

<div align="center">

## ⭐ Dukung Project Ini ⭐

Jika project ini membantu Anda, berikan bintang!

**"Dari developer untuk developer"** 🚀

</div>