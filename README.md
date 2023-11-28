# praktikum5
| Variable       |      DATA DIRI        |
| ---------------| --------------------- |
| Nama           | Lutpiah ainus shiddik |                                          
| NIM            | 312310475             |
| Kelas          | TI.23.A.5             |
| Mata Kuliah    |Bahasa Pemrograman     |

Tugas Praktikum
Buat program sederhana yang akan menampilkan daftar nilai mahasiswa, dengan ketentuan :

-Tampilkan menu pilihan: (Tambah Data, Ubah Data, Hapus Data, Tampilkan Data, Cari Data)
-Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)
-Buat flowchart dan penjelasan programnya pada README.md. • Commit dan push repository ke github.
#Latihan
membuat kontak awal / b = {'ari' : '085267888', 'dina' : 087677776}
menampilkan kontak ari / print(b['ari'])
menambhkan kontak riko / b['riko']= 087888999
mengubah kontak dina / b['dina]= '089555777
menampilkan semua nama / print(b.keys())
menampilkan semua nomor / print(b.values())
menampilkan semua nama dan nomor / print(b)
menghapus kontak dina / del b['dina']

BERIKUT ADALAH CODINGAN PROGRAM NYA
list = {
    "Arii" : "081267888", "Dina" : "087677776"  
}
print("\nTampilkan kontak Arii :")
print(29*"=")
print(" {0:^2} |".format("Nama"), "Nomor Telepon")      
print("=============================")
# Tampilkan Kontak Ari
print(" {0:^2} |".format("Arii") ,list["Arii"],"\n")
# Tambah Kontak baru
list["Riko"] = "087654544"
# Ubah kontak dina dengan nomor baru
list["Dina"] = "088999776"
# Tampilkan semua Nama 
print("Tampilan semua Nama :")
print("=============================")
# Setelah di ubah
print(" {0:^2} |".format("Nama"), "Nomor Telepon")
print("=============================")
for x in list.keys():
    print(" {0:^2} |".format(x))
print("\n")
# Tampilkan Semua Nomor 
print("Tampilan semua Nomor :")
print("=============================")
# Setelah di ubah
print(" {0:^2} |".format("Nama"), "Nomor Telepon")
print("=============================")

for x in list.values():
    print(" {0:^2} |".format(x))
print("\n")
# Tampilkan daftar Nama & Nomor
print("Tampilan daftar Nama & Nomor :")
print("=============================")
# Setelah di ubah
print(" {0:^2} |".format("Nama"), "Nomor Telepon")
print("=============================")

for x, y in list.items():
    print(" {0:^2} |".format(x), (y))
print("\n")
# Menghapus Kontak Dina
print("Menghapus Kontak Dina :")
print(29*"=")
del list["Dina"]
print(" {0:^2} |".format("Nama"), "Nomor Telepon")
print("=============================")
for x, y in list.items():
    print(" {0:^2} |".format(x), (y))
print("\n")
![latihan1](https://github.com/lutpi9/praktikum5/assets/147919251/499c4f5d-c442-47a9-9428-15339aa544a7)
![latihan 1](https://github.com/lutpi9/praktikum5/assets/147919251/a28ab7da-ba34-4434-b2e8-7bae4e19502c)


