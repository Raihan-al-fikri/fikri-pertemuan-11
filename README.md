# fikri-pertemuan-11

Nama : Moh. Raihan al fikri
Nim  : 352310871
Kelas: IE.23.C12

![Screenshot 2024-12-11 112941](https://github.com/user-attachments/assets/1a269d3a-32ad-4f70-b481-4d7ce89ccbfa)




![Screenshot 2024-12-11 113003](https://github.com/user-attachments/assets/29e322b3-f451-40e7-a2eb-c52138e6e042)





![Screenshot 2024-12-11 113024](https://github.com/user-attachments/assets/7398b8e8-a1b6-4e7c-b5c3-6a067aa48c83)








Daftar mahasiswa
mahasiswa = []

Fungsi untuk menambah data mahasiswa
def tambah(): nama = input("Masukkan nama mahasiswa: ") nilai = input("Masukkan nilai mahasiswa: ") mahasiswa.append({"nama": nama, "nilai": nilai}) print("Data mahasiswa berhasil ditambahkan!")

Fungsi untuk menampilkan data mahasiswa
def tampilkan(): if not mahasiswa: print("Tidak ada data mahasiswa.") else: print("\nDaftar Nilai Mahasiswa:") for mhs in mahasiswa: print(f"Nama: {mhs['nama']}, Nilai: {mhs['nilai']}")

Fungsi untuk menghapus data mahasiswa berdasarkan nama
def hapus(nama): global mahasiswa mahasiswa = [mhs for mhs in mahasiswa if mhs['nama'] != nama] print(f"Data mahasiswa dengan nama {nama} telah dihapus!")

Fungsi untuk mengubah data mahasiswa berdasarkan nama
def ubah(nama): for mhs in mahasiswa: if mhs['nama'] == nama: nilai_baru = input(f"Masukkan nilai baru untuk {nama}: ") mhs['nilai'] = nilai_baru print(f"Data nilai mahasiswa {nama} berhasil diubah!") return print(f"Mahasiswa dengan nama {nama} tidak ditemukan!")

Menu utama program
def main(): while True: print("\nMenu:") print("1. Tambah Data Mahasiswa") print("2. Tampilkan Data Mahasiswa") print("3. Hapus Data Mahasiswa") print("4. Ubah Data Mahasiswa") print("5. Keluar")

    pilihan = input("Pilih menu (1/2/3/4/5): ")
    
    if pilihan == "1":
        tambah()
    elif pilihan == "2":
        tampilkan()
    elif pilihan == "3":
        nama = input("Masukkan nama mahasiswa yang ingin dihapus: ")
        hapus(nama)
    elif pilihan == "4":
        nama = input("Masukkan nama mahasiswa yang ingin diubah: ")
        ubah(nama)
    elif pilihan == "5":
        print("Terima kasih, program selesai.")
        break
    else:
        print("Pilihan tidak valid. Silakan coba lagi.")
if name == "main": main()


#FLOW CHART

![Screenshot 2024-12-11 113832](https://github.com/user-attachments/assets/3d21dd9c-f97e-456f-b2cd-8756c37359e9)




