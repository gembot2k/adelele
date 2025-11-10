# 🧩 **Rangkuman Uji Praktik Informatika**

## Program: Pengelolaan Nilai Siswa 

---

## 💻 **Kode Program**

```python
nama_siswa = []
nilai_siswa = []

for i in range(3):
    nama = input("Masukkan nama siswa: ")
    nilai = int(input("Masukkan nilai siswa: "))
    nama_siswa.append(nama)
    nilai_siswa.append(nilai)

print("\nData nilai siswa:")
for i in range(3):
    if nilai_siswa[i] >= 70:
        print(nama_siswa[i], "-", nilai_siswa[i], "Lulus")
    else:
        print(nama_siswa[i], "-", nilai_siswa[i], "Tidak Lulus")
print("================================")

def hitung_rata(data):
    total = sum(nilai_siswa)
    print("Total nilai:", total)
    rata = total / len(nilai_siswa)
    print("Rata-rata nilai:", rata)
    return sum(data) / len(data)

print("Rata-rata nilai:", hitung_rata(nilai_siswa))
print("=== Program Selesai ===")
```

---

## 🧠 **Penjelasan Baris per Baris**

| Baris | Kode                                                  | Penjelasan                                                                          |
| :---: | :---------------------------------------------------- | :---------------------------------------------------------------------------------- |
|   1   | `nama_siswa = []`                                     | Membuat list kosong untuk menyimpan nama-nama siswa.                                |
|   2   | `nilai_siswa = []`                                    | Membuat list kosong untuk menyimpan nilai masing-masing siswa.                      |
|   4   | `for i in range(3):`                                  | Loop untuk mengulang proses input sebanyak 3 kali (3 siswa).                        |
|   5   | `nama = input("Masukkan nama siswa: ")`               | Meminta pengguna mengetik nama siswa, hasilnya berupa string.                       |
|   6   | `nilai = int(input("Masukkan nilai siswa: "))`        | Meminta pengguna memasukkan nilai (string), lalu mengubahnya menjadi angka (`int`). |
|   7   | `nama_siswa.append(nama)`                             | Menyimpan nama ke dalam list `nama_siswa`.                                          |
|   8   | `nilai_siswa.append(nilai)`                           | Menyimpan nilai ke dalam list `nilai_siswa`.                                        |
|   10  | `print("\nData nilai siswa:")`                        | Menampilkan judul bagian data nilai siswa.                                          |
|   11  | `for i in range(3):`                                  | Mengulang lagi sebanyak 3 kali untuk menampilkan hasil dari tiap siswa.             |
| 12–15 | `if ... else`                                         | Mengecek apakah nilai siswa ≥ 70 → **Lulus**, jika tidak → **Tidak Lulus**.         |
|   16  | `print("================================")`           | Menampilkan garis pembatas agar tampilan rapi.                                      |
|   18  | `def hitung_rata(data):`                              | Membuat fungsi bernama `hitung_rata` untuk menghitung rata-rata nilai.              |
|   19  | `total = sum(nilai_siswa)`                            | Menjumlahkan semua nilai dalam list `nilai_siswa`.                                  |
|   20  | `print("Total nilai:", total)`                        | Menampilkan jumlah total nilai dari semua siswa.                                    |
|   21  | `rata = total / len(nilai_siswa)`                     | Menghitung rata-rata dengan rumus total dibagi jumlah data.                         |
|   22  | `print("Rata-rata nilai:", rata)`                     | Menampilkan nilai rata-rata ke layar.                                               |
|   23  | `return sum(data) / len(data)`                        | Mengembalikan hasil rata-rata agar bisa digunakan di luar fungsi.                   |
|   25  | `print("Rata-rata nilai:", hitung_rata(nilai_siswa))` | Memanggil fungsi `hitung_rata()` dan menampilkan hasilnya.                          |
|   26  | `print("=== Program Selesai ===")`                    | Menandakan bahwa program sudah berakhir.                                            |

---

## 📋 **Deskripsi Program**

Program ini digunakan untuk **menginput data 3 siswa**, menyimpan **nama dan nilai** ke dalam list, lalu menampilkan hasil dengan status kelulusan.
Setelah semua data dimasukkan, program juga akan **menghitung total nilai dan rata-rata nilai siswa** menggunakan fungsi `hitung_rata()`.

Kriteria kelulusan:

* Nilai **≥ 70** → **Lulus**
* Nilai **< 70** → **Tidak Lulus**

---

## 🧾 **Contoh Input dan Output**

### **Input (dari pengguna):**

```
Masukkan nama siswa: Ahmad
Masukkan nilai siswa: 90
Masukkan nama siswa: Rizky
Masukkan nilai siswa: 70
Masukkan nama siswa: Yudho
Masukkan nilai siswa: 50
```

### **Output (hasil di terminal):**

```
Data nilai siswa:
Ahmad - 90 Lulus
Rizky - 70 Lulus
Yudho - 50 Tidak Lulus
================================
Total nilai: 210
Rata-rata nilai: 70.0
Rata-rata nilai: 70.0
=== Program Selesai ===
```

---

## 🧩 **Kesimpulan**

* Program ini menggunakan **list**, **loop (for)**, dan **fungsi (def)**.
* Fungsi `append()` digunakan untuk menambahkan data.
* Fungsi `sum()` dan `len()` digunakan untuk menghitung total dan rata-rata nilai.
* Struktur `if–else` digunakan untuk menentukan status kelulusan.
* Output akhir menampilkan **total nilai, rata-rata nilai, dan status tiap siswa**.

---
