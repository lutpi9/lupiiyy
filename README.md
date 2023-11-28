# praktikum5
| Variable       |      DATA DIRI        |
| ---------------| --------------------- |
| Nama           | Lutpiah ainus shiddik |                                          
| NIM            | 312310475             |
| Kelas          | TI.23.A.5             |
| Mata Kuliah    |Bahasa Pemrograman     |

Tugas Praktikum
Buat program sederhana yang akan menampilkan daftar nilai mahasiswa, dengan ketentuan :

#Program dibuat dengan menggunakan Dictionary

#Tampilkan menu pilihan: (Tambah Data, Ubah Data, Hapus Data, Tampilkan Data, Cari Data)

#Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)

#Buat flowchart dan penjelasan programnya pada README.md. • Commit dan push repository ke github.


#LATIHAN 1
Latihan

membuat kontak awal / b = {'ari' : '085267888', 'dina' : 087677776}
menampilkan kontak ari / print(b['ari'])
menambhkan kontak riko / b['riko']= 087888999
mengubah kontak dina / b['dina]= '089555777
menampilkan semua nama / print(b.keys())
menampilkan semua nomor / print(b.values())
menampilkan semua nama dan nomor / print(b)
menghapus kontak dina / del b['dina']Penjelasan Program


CODINGAN PROGRAM
 
list = {
    "Arii" : "081267888", "Dina" : "087677776"  
}
print("\nTampilkan kontak Arii :")
print(29*"=")
print(" {0:^2} |".format("Nama"), "Nomor Telepon")      
print("=============================")
#tampilkan kontak ari
print(" {0:^2} |".format("Arii") ,list["Arii"],"\n")
#tambahkan kontak baru
list["Riko"] = "087654544"
#ubah kontak dina dengan nomor baru
list["Dina"] = "088999776"
#tampilkan semua nama
print("Tampilan semua Nama :")
print("=============================")
#setelah diubah
print(" {0:^2} |".format("Nama"), "Nomor Telepon")
print("=============================")
for x in list.keys():
    print(" {0:^2} |".format(x))
print("\n")
#tampilkan semua nomor
print("Tampilan semua Nomor :")
print("=============================")
#setelah diubah
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




Menambahkan data input
list = {}
while True:
    c = input("\n(T)ambah, (U)bah, (H)apus, (C)ari, (L)ihat, (K)eluar: ")

    # Menambahkan data inputan 
    if c.lower() == 't':
        print("Tambah data :\n")
        nama    = input("Nama           : ")
        nim     = int(input("NIM            : "))
        uts     = int(input("Nilai UTS      : "))
        uas     = int(input("Nilai UAS      : "))
        tugas   = int(input("Nilai Tugas    : "))
        akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
        list[nama] = [nim, tugas, uts, uas, akhir]
if c.lower Berfungsi seperti or input bisa berjalan jika memasukan T/t

Mengubah data inputan
    
    # Mengubah data inputan
    elif c.lower() == 'u':
        print("Ubah Data :")
        nama = input("\nMasukkan Nama  : ")
        if nama in list.keys():
            nim     = int(input("NIM            : "))
            uts     = int(input("Nilai UTS      : "))
            uas     = int(input("Nilai UAS      : "))
            tugas   = int(input("Nilai Tugas    : "))
            akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
            list[nama] = [nim, tugas, uts, uas, akhir]
       else:
            print("NAMA {0} TIDAK ADA!".format(nama))



print("NAMA {0} TIDAK ADA!".format(nama)) memanggil variable nama
Menghapus Data yg sudah di input
    
    # Menghapus inputan Nama
    elif c.lower() == 'h':
        print("Hapus berdasarkan nama inputan :")
        nama = input("\nMasukkan Nama  : ")
        if nama in list.keys():
            del list[nama]
            print("\nData {0} berhasil di hapus".format(nama))
        else:
            print("NAMA {0} TIDAK ADA!".format(nama))

Mencari data yg sudah di input
    
    # Mencari data yg sudah di input
    elif c.lower() == 'c':
        print("Cari data berdasarkan nama inputan :")
        nama = input("\nMasukkan Nama : ")
        if nama in list.keys():
            print("\nNama        : {0}".format(nama))
            print("NIM         : {0}".format(nim))
            print("Nilai UTS   : {0}".format(uts))
            print("Nilai UAS   : {0}".format(uas))
            print("Nilai Tugas : {0}".format(tugas))                  
            print("Nilai Akhir : {0}".format(akhir)) 
        else:
            print("NAMA {0} TIDAK ADA!".format(nama))
Menanpilkan seluruh data
   
    # Menampilkan seluruh data 
    elif c.lower() == 'l':
        if list.items():
            print("-"*78)
            print("|                               Daftar Mahasiswa                             |")
            print("-"*78)
            print("|No. | Nama            |       NIM       |  UTS  |  UAS  |  Tugas  |  Akhir  |")
            print("="*78)
            i = 0
            for z in list.items():
                i += 1
                print("| {no:2d} | {0:15s} | {1:15d} | {2:5d} | {3:5d} | {4:7d} | {5:7.2f} |"
                      .format(z[0][:13], z[1][0], z[1][1], z[1][2], z[1][3], z[1][4], no=i))
            print("-"*78)
        else:
            print("-"*78)
            print("|                               Daftar Mahasiswa                             |")
            print("-"*78)
            print("|No. | Nama            |       NIM       |  UTS  |  UAS  |  Tugas  |  Akhir  |")
            print("-"*78)
            print("|                       TIDAK ADA DATA! Silakan tambah data                  |")
            print("-"*78)


for z in list.items():        
               
                i += 1
                print("| {no:2d} | {0:15s} | {1:15d} | {2:5d} | {3:5d} | {4:7d} | {5:7.2f} |"
                      .format(z[0][:13], z[1][0], z[1][1], z[1][2], z[1][3], z[1][4], no=i))
 
 
 
 list.items(): memanggil isi dari variable list, .format Digunakan untuk mengatur format string yang nantinya akan dicetak atau ditampilkan ke layar.



Keluar program
    
    # Keluar program
    elif c. lower() == 'k':
        break
        else:
        print("\n INPUT {} TIDAK ADA!, Silakan pilih [T/U/H/C/L] untuk menjalankan program!".format(c))
Hasil program



