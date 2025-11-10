## 🧩 **Deskripsi Singkat**

Program ini dibuat untuk mengelola data nilai beberapa siswa.
Program akan:

* Menerima input nama dan nilai dari pengguna,
* Menyimpan data ke dalam *list*,
* Menampilkan kembali data yang sudah diinput,
* Menghitung total dan rata-rata nilai,
* Menentukan status **LULUS** atau **TIDAK LULUS** berdasarkan nilai.

---

## 💻 **Kode Program Lengkap**

```python
# Program Pengelolaan Nilai (sesuai kisi-kisi)
# 1. Buat dua list kosong untuk menyimpan nama_siswa dan nilai_siswa
nama_siswa = []       # list untuk menyimpan nama siswa
nilai_siswa = []      # list untuk menyimpan nilai siswa

# 5. Gunakan for agar program bisa menerima data 3 siswa sekaligus
JUMLAH_SISWA = 3
for i in range(JUMLAH_SISWA):
    # 8. Tambahkan garis pembatas agar output lebih rapi
    print("=" * 40)
    print("Input data siswa ke-", i + 1)

    # 2. Minta pengguna memasukkan nama siswa (input -> string)
    nama = input("Masukkan nama siswa: ")

    # 3. Minta pengguna memasukkan nilai, lalu ubah ke tipe data angka
    nilai_str = input("Masukkan nilai (0-100): ")
    nilai = float(nilai_str)   # konversi string ke float agar bisa dihitung

    # 4. Masukkan data nama dan nilai ke dalam list dengan .append()
    nama_siswa.append(nama)
    nilai_siswa.append(nilai)

# 6. Tampilkan semua data yang sudah diinput
print("=" * 40)
print("\nData yang sudah diinput:")

# gunakan indexing sederhana (tanpa zip/enumerate)
i = 0
while i < len(nama_siswa):
    # 7. Gunakan if untuk menentukan lulus atau tidak (nilai >= 70)
    if nilai_siswa[i] >= 70:
        status = "LULUS"
    else:
        status = "TIDAK LULUS"

    # tampilkan nomor, nama, nilai, dan status
    print(str(i+1) + ". " + nama_siswa[i] + " — Nilai: " + str(nilai_siswa[i]) + " — " + status)
    i = i + 1

# 9. Gunakan sum() untuk menghitung total semua nilai_siswa
total_nilai = sum(nilai_siswa)

# 11. Buat fungsi hitung_rata agar perhitungan rata-rata lebih praktis
def hitung_rata(list_nilai):
    # jika list kosong, kembalikan 0 untuk menghindari pembagian dengan nol
    if len(list_nilai) == 0:
        return 0
    # 10. Hitung rata-rata dari seluruh nilai menggunakan len()
    return sum(list_nilai) / len(list_nilai)

# 12. Gunakan fungsi hitung_rata() untuk menampilkan hasil rata nilai_siswa
rata2 = hitung_rata(nilai_siswa)

# tampilkan total dan rata-rata
print("\n" + "-" * 40)
print("Total nilai: " + str(total_nilai))
print("Rata-rata nilai: " + str(round(rata2, 2)))
print("-" * 40)

# 13. Tambahkan pesan setelah semua hasil ditampilkan
print("\nTERIMA KASIH ATAS WAKTUNYA")
```

---

## 🧠 **Penjelasan Langkah per Langkah**

|    No   | Penjelasan                                                                                                |
| :-----: | :-------------------------------------------------------------------------------------------------------- |
|  **1.** | `nama_siswa = []` dan `nilai_siswa = []` → membuat dua list kosong untuk menampung data nama dan nilai.   |
|  **2.** | `input("Masukkan nama siswa: ")` → menerima input nama dari pengguna.                                     |
|  **3.** | `input("Masukkan nilai (0-100): ")` + `float()` → mengubah input teks menjadi angka agar bisa dihitung.   |
|  **4.** | `.append()` → menambahkan data baru ke dalam list (array).                                                |
|  **5.** | `for i in range(JUMLAH_SISWA):` → melakukan pengulangan agar dapat input data beberapa siswa sekaligus.   |
|  **6.** | `print("\nData yang sudah diinput:")` → menampilkan data setelah semua input selesai.                     |
|  **7.** | `if nilai_siswa[i] >= 70:` → kondisi logika untuk menentukan apakah siswa **LULUS** atau **TIDAK LULUS**. |
|  **8.** | `print("=" * 40)` → mencetak garis pembatas agar hasil output lebih rapi.                                 |
|  **9.** | `sum(nilai_siswa)` → menjumlahkan seluruh nilai siswa.                                                    |
| **10.** | `len(nilai_siswa)` → menghitung jumlah elemen di dalam list, digunakan untuk rata-rata.                   |
| **11.** | `def hitung_rata(list_nilai):` → membuat fungsi untuk menghitung rata-rata nilai.                         |
| **12.** | `rata2 = hitung_rata(nilai_siswa)` → memanggil fungsi rata-rata dan menampilkan hasilnya.                 |
| **13.** | `print("TERIMA KASIH ATAS WAKTUNYA")` → menutup program dengan ucapan terima kasih.                       |

---

## 📋 **Alur Program Singkat**

1. Buat dua list kosong untuk nama dan nilai siswa.
2. Gunakan `for` loop agar bisa input beberapa data sekaligus.
3. Konversi nilai dari string ke angka (`float`).
4. Tambahkan data ke list dengan `.append()`.
5. Tampilkan kembali semua data menggunakan `while`.
6. Gunakan `if` untuk menentukan kelulusan.
7. Hitung total dan rata-rata nilai.
8. Tampilkan hasil akhir dan ucapan terima kasih.

---

## ✅ **Contoh Output**

```
========================================
Input data siswa ke- 1
Masukkan nama siswa: Dinda
Masukkan nilai (0-100): 85
========================================
Input data siswa ke- 2
Masukkan nama siswa: Reza
Masukkan nilai (0-100): 65
========================================
Input data siswa ke- 3
Masukkan nama siswa: Lani
Masukkan nilai (0-100): 90
========================================

Data yang sudah diinput:
1. Dinda — Nilai: 85.0 — LULUS
2. Reza — Nilai: 65.0 — TIDAK LULUS
3. Lani — Nilai: 90.0 — LULUS
----------------------------------------
Total nilai: 240.0
Rata-rata nilai: 80.0
----------------------------------------

TERIMA KASIH ATAS WAKTUNYA
```

---

Apakah kamu mau saya buatkan file `.md`-nya langsung biar bisa kamu unduh (misalnya `Laporan_Uji_Praktik_Informatika.md`)?
