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


# LATIHAN 1
# OUTPUT

![codingan latihan 1](https://github.com/lutpi9/praktikum5/assets/147919251/c4dc71db-b7b2-4302-a2b4-1a6c92679281)
![codingan latihan 1](https://github.com/lutpi9/praktikum5/assets/147919251/e01304a4-e40e-4c5f-b1d6-31e9ce5480e0)
![codingan latihan 1](https://github.com/lutpi9/praktikum5/assets/147919251/d42a2751-1bf2-41dc-9804-fbba92b3f54d)

# INPUT

![latihan1](https://github.com/lutpi9/praktikum5/assets/147919251/33c11623-ce70-4790-b0e1-8c9861314c29)
![latihan 1](https://github.com/lutpi9/praktikum5/assets/147919251/c177475f-903c-4af3-8c48-ad79763df12d)



# PRALTIKUM

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

# hasil untuk (T)
![tambah](https://github.com/lutpi9/praktikum5/assets/147919251/82e945da-7fc0-49f3-b257-c86596fe2ecf)
# hasil untuk (U)
![ubah](https://github.com/lutpi9/praktikum5/assets/147919251/9c378a70-67ea-4620-95f9-d39f8171ab43)
# hasil untuk (L)
![lihat](https://github.com/lutpi9/praktikum5/assets/147919251/1de703c0-2a6a-4999-a7a6-71389bdf562b)
# hasil untuk (C)
![cari](https://github.com/lutpi9/praktikum5/assets/147919251/b764188a-5afa-4bb5-b119-891920780692)
# hasil untuk (H)
![hapus](https://github.com/lutpi9/praktikum5/assets/147919251/6ecca55e-04ce-46be-8cda-bd8fdad4d354)






