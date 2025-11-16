## Code Membuat Mie Kuah

```python3
# Membuat fungsi utama untuk membuat mie kuah
def membuat_mie_kuah():
    # Membuat array untuk menampung alat dan bahan
    alat_dan_bahan = ["Panci", "Kompor", "Air", "Indomie", "Mangkuk", "Garpu"]
    
    # Menampilkan daftar alat dan bahan
    print("Langkah 1: Menyiapkan alat dan bahan.")

    # Menggunakan loop untuk menampilkan item dari array alat_dan_bahan
    for item in alat_dan_bahan:
        # Menampilkan setiap alat dan bahan yang disiapkan
        print("-", item)

    # Membuat variable untuk status air (awalnya belum mendidih)
    air_mendidih = "tidak"

    # Memasukkan air ke panci dan merebusnya hingga mendidih
    print("\nLangkah 2: Memasukkan air ke panci dan rebus hingga mendidih.")
    print("\nLangkah 3: Rebus air hingga mendidih.")
    
    # Mengubah variable menjadi "ya" karena air sudah mendidih
    air_mendidih = "ya"

    # Menggunakan 'if' untuk mengecek kondisi apakah air sudah mendidih
    if (air_mendidih == "ya"):
        # Jika sudah mendidih, menampilkan air sudah mendidih
        print("Air sudah mendidih!")

        # Menampilkan langkah keempat: memasukkan mie
        print("\nLangkah 4: Memasukkan mie ke dalam air mendidih.")
        
        # Menampilkan langkah kelima: menunggu 5 menit
        print("\nLangkah 5: Menunggu mie matang selama 5 menit.")

        # Menggunakan loop untuk simulasi menunggu dari menit 1 hingga 5
        for menit in range(1, 6):
            # Menampilan waktu sampai 5 menit
            print(f"Menunggu {menit} menit...")
        
        # Menampilkan langkah-langkah akhit
        print("\nLangkah 6: Mie sudah matang, mengangkat mie dan kuah ke mangkuk.")
        print("\nLangkah 7: Memasukkan bumbu.")
        print("\nLangkah 8: Mengaduk hingga merata.")

        print("\nLangkah Terakhir: Mie kuah siap disantap! 🍜")

# Memanggil fungsi utama untuk menjalankan program
membuat_mie_kuah()
```

## Hasil print dari code
```
Langkah 1: Menyiapkan alat dan bahan.
- Panci
- Kompor
- Air
- Indomie
- Mangkuk
- Garpu

Langkah 2: Memasukkan air ke panci dan rebus hingga mendidih.

Langkah 3: Rebus air hingga mendidih.
Air sudah mendidih!

Langkah 4: Memasukkan mie ke dalam air mendidih.

Langkah 5: Menunggu mie matang selama 5 menit.
Menunggu 1 menit...
Menunggu 2 menit...
Menunggu 3 menit...
Menunggu 4 menit...
Menunggu 5 menit...

Langkah 6: Mie sudah matang, mengangkat mie dan kuah ke mangkuk.

Langkah 7: Memasukkan bumbu.

Langkah 8: Mengaduk hingga merata.

Langkah Terakhir: Mie kuah siap disantap! 🍜
```
