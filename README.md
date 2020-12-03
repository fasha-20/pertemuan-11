# pertemuan-11

Soal Latihan 1

![1.png](/gmbr1/1.png)

Source Code

print("________________________________________")
# mengubah function menggunakan lambda


def a(x):
	   return x ** 2


lambda x: x ** 2


print("1. Mengubah function menggunakan Lambda \n   def a(x): \n \t   return x ** 2")
print("   Hasil : lambda x: x ** 2")


def b(x, y):
        return math.sqrt(x ** 2 + y ** 2)


lambda x, y: math.sqrt(x ** 2 + y ** 2)


print("________________________________________")
print("2. Mengubah function menggunakan Lambda \n   def b(x, y): \n \t   return math.sqrt(x ** 2 + y ** 2)")
print("   Hasil : lambda x, y: math.sqrt(x ** 2 + y ** 2))")


def c(*args):
        return sum(args) / len(args)


lambda *args: sum(args) / len(args)


print("________________________________________")
print("3. Mengubah function menggunakan Lambda \n   def c(*args): \n \t   return sum(args) / len(args)")
print("   Hasil : lambda *args: sum(args) / len(args))")


def d(s):
        return "".join(set(s))


lambda s: "".join(set(s))


print("________________________________________")
print("4. Mengubah function menggunakan Lambda \n   def d(s): \n \t   return "".join(set(s))")
print("   Hasil : lambda s: "".join(set(s)))")

Hasil ouputnya

![2.png](/gmbr1/2.png)

Praktikum 6

![3.png](/gmbr1/3.png)

Source Code

print("==================================")
print("======> Program Input Data <======")
print("==================================")

data = {}

def tambah():
	    print("Tambah Data")
	    nama = input("Nama\t\t: ")
	    nim = int(input("NIM\t\t: "))
	    tugas = int(input("NIlai Tugas\t: "))
	    uts = int(input("Nilai UTS\t: "))
	    uas = int(input("Nilai UAS\t: "))
	    nilaiakhir = (tugas * 0.30 + uts * 0.35 + uas * 0.35)
	    data[nama] = nim, tugas, uts, uas, nilaiakhir
    
    
def tampilkan():
        print("----- DAFTAR NILAI -----")
        print("=================================================================")
        print("| NO |    NIM        |  TUGAS | UTS | UAS | AKHIR|")
        print("=================================================================")
        i = 0
        for x in data.items():
            i += 1
            print("|  1 |{0:9}   |{1:9}     |{2:9} |{3:9}  |{4:9}   |{5:9}  |" .format(x[0],
            x[1][1], x[1][2], x[1][3], x[1][4], i))
            
        else:
            print("=============================================================")
            
def hapus():
        print("----- Menghapus Data Mahasiswa -----")
        nama = input("Nama                : ")
        if nama in data.keys():
            del data[nama]
            print()
        else:
            print("Data {0} tidak ada".format(nama))
            
        
def ubah():
        print("----- Ubah Data Mahasiswa -----")
        nama = input("Nama  : ")
        if nama in data.keys():
            nim = input("Nim  : ")
            tugas = int(input("Nilai Tugas Baru : "))
            uts = int(input("Nilai UTS Baru : "))
            uas = int(input("Nilai UAS Baru : "))
            akhir = (int(tugas)* .30) + (int(uts)* .35) + (int(uas)* .35)
            data[nama] = nim, tugas, uts, uas, akhir
            print()
        else:
            print("Data Nilai {0} tidak ada ".format(nama))
            
            
while True:
    print("======================>>> Data Mahasiswa <<<===========================")
    print("=======================================================================")
    print("| NO |    Nama    |      Nim      |  Tugas  |  UTS  |  UAS  |  Akhir  |")
    print("=======================================================================")
    print(">>>>>>>>>>>>>>>>>>>>>>>>> TIDAK ADA DATA <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<")
    m = input("=====>> (1)Lihat, (2)Tambah, (3)Ubah, (4)Hapus, (0)Keluar : <<=====")
    if m.lower() == "1":
        tampilkan()
    elif m.lower() == "2":
        tambah()
    elif m.lower() == "3":
        ubah()
    elif m.lower() == "4":
        hapus()
    elif m.lower() == "0":
        print()
        break
    
    else:
        print()
        print(35*"=")
        print("== Terjadi Kesalahan ==")
        print("==      Coba Lagi    ==")
        print(35*"=")

Menambah Data Mahasiswa

![4.png](/gmbr1/4.png)

Mengubah Data Mahasiswa

![5.png](/gmbr1/5.png)

Menghapus Data Mahasiswa

![6.png](/gmbr1/6.png)


FLOWCHART

![7.png](/gmbr/7.png)

SEKIAN