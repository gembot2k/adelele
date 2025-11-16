## Code Membuat Mie Kuah

```python3
# Mendefinisikan fungsi utama untuk membuat mie kuah
def buat_mie_kuah():
    # --- Komponen 1: Variable & 2: Array (List) ---
    # Membuat variable berupa array/list untuk menampung alat dan bahan
    alat_dan_bahan = ["Panci", "Kompor", "Air", "Indomie", "Mangkuk", "Garpu", "Bumbu"]
    
    # Menampilkan langkah pertama: menyiapkan alat dan bahan
    print("Langkah 1: Menyiapkan alat dan bahan.")
    # --- Komponen 3: Loop ---
    # Menggunakan loop untuk menampilkan setiap item dalam array alat_dan_bahan
    for item in alat_dan_bahan:
        # Mencetak setiap alat dan bahan yang disiapkan
        print(f"- {item}")

    # Menampilkan langkah kedua dan ketiga: merebus air
    print("\nLangkah 2 & 3: Memasukkan air ke panci dan merebusnya.")
    # Membuat variable boolean untuk status air (awalnya belum mendidih)
    air_mendidih = False
    # Mensimulasikan proses pemanasan
    print("Menyalakan kompor, menunggu air mendidih...")
    # Mengubah nilai variable menjadi True karena air sudah mendidih
    air_mendidih = True

    # --- Komponen 4: If ---
    # Menggunakan 'if' untuk mengecek kondisi apakah air sudah mendidih
    if air_mendidih:
        # Jika True, cetak pesan bahwa air sudah mendidih
        print("Air sudah mendidih!")
        # Menampilkan langkah keempat: memasukkan mie
        print("\nLangkah 4: Memasukkan mie ke dalam air mendidih.")
        
        # Menampilkan langkah kelima: menunggu 5 menit
        print("\nLangkah 5: Menunggu mie matang selama 5 menit.")
        # Menggunakan loop 'for' untuk simulasi penungguan dari menit 1 hingga 5
        for menit in range(1, 6):
            # Mencetak proses penungguan setiap menitnya
            print(f"Menunggu {menit} menit...")
        
        # Menampilkan langkah-langkah terakhir
        print("\nLangkah 6: Mie sudah matang, mengangkat mie dan kuah ke mangkuk.")
        print("Langkah 7: Memasukkan bumbu.")
        print("Langkah 8: Mengaduk hingga merata.")
        print("\nLangkah Terakhir: Mie kuah siap disantap! 🍜")

# Memanggil fungsi utama untuk menjalankan program
buat_mie_kuah()

# --- Print Hasil Capture dari Code ---
# Mencetak garis pemisah untuk hasil akhir
print("\n" + "="*40)
# Mencetak pesan bahwa simulasi telah selesai
print("Hasil: Program berhasil mensimulasikan")
print("algoritma membuat mie kuah dari flowchart.")
# Mencetak garis pemisah
print("="*40)
```
