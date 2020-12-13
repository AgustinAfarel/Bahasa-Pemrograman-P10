# Bahasa-Pemrograman-P10
Dibuat untuk memenuhi tugas Bahasa Pemrograman pertemuan 10

<br>NAMA        : AGUSTIN AFAREL
<br>NIM         : 312010081
<br>Kelas       : TI.20.B.1
<br>Mata Kuliah : Bahasa Pemrograman

 # TUGAS LATIHAN
``` python
def a(x):
    return x ** 2


a2 = lambda x: x ** 2


print("1. Mengubah function menggunakan lambda \n \t return x ** 2")


def b(x, y):
    return math.sqrt(x * + y * 2)


b2 = lambda x, y: math.sqrt(x * + y * 2)

print("_____________")
print("2. Mengubah function menggunakan lambda \n def b(x, y): \n \t return math.sqrt(x * 2 + y * 2)")
print("  Hasil : b2 = lambda x, y: math.sqrt(x * 2 + y * 2)")


def c(*args):
    return sum(args) / len(args)


c2 = lambda *args: sum(args) / len(args)

print("_____________")
print("2. Mengubah function menggunakan lambda \n  def c(*args): \n \t return sum(args) / len(args)")
print("  Hasil : c2 = lambda *args: sum(args) / len(args)")


def d(s):
    return "".join(set(s))


d2 = lambda s: "".join(set(s))

print("_____________")
print("4. Mengubah function menggunakan lambda \n def d(s): \n \t return "".join(set(s)")
print(" Hasil : d2 =lambda s: "".join(set(s))")

```
* HASIL SOURCE CODE DI ATAS SEBAGAI BERIKUT
![Gambar](PictureP10/Gambar1.PNG)

# TUGAS PRAKTIKUM

``` python
from PrettyTable import PrettyTable

print("=============================")
print("NAMA : AGUSTIN AFAREL")
print("NIM : 312010081")
print("Kelas : TI.20.B.1")
print("Mata Kuliah : Bahasa Pemrograman")
print("Tugas : Praktikum lab 6 - Pertemuan 10")
print("=============================")

tampunglist = {}
x = prettytable


def tambah():
    print("========= TAMBAH DATA NILAI MAHASISWA ===========")
    tnama = imput("Masukkan Nama Mahasiswa  : ")
    tnim = imput("Masukkan NIM Masahasiswa : ")
    ttugas = int(input("Masukkan Nilai Tugas Mahasiswa : "))
    tuts = int(input("Masukkan Nilai UTS Mahasiswa : "))
    tuas = int(input("Masukkan Nilai UAS Mahasiswa :"))
    takhir = 0.3 * float(ttugas) + 0.35 * float(tuas) + 0.35 *float(tuas)
    tampunglist[tnama] = tnim, ttugas, tuts, tuas, takhir


def tampilkan():
    print("======== LIHAT DATA NILAI MAHASISWA ========")
    no = 0
    x.flield_names = ["NO", "NAMA", "NIM", "TUGAS", "UTS", "UAS", "AKHIR"]
    for tdata in tampunglist():
        no +=1
        x.add_row([no, tdata[0], tdata[1][1], tdata[1][2], tdata[1][3], tdata[1][4]])
        print(x)


def hapus(hxsiapa):
    print("======== Hapus Data Nilai Mahasiswa =========")
    if hxsiapa in tampunglist.keys():
        print(f"DATA {hxsiapa} BERHASIL DIHAPUS")
        mhs = int(input(" 1. NIM \n 2. Tugas Nilai \n 3. Nilai UAS\n pilih dengan angka (1/2/3/4) : "))
        if mhs == 1:
            ubahnim = input("Silahkan masukkan NIM yang bener : ")
            i = 0
            vtug = tampunglist[xsiapa][1]
            vuts = tampunglist[xsiapa][2]
            vuas = tampunglist[xsiapa][3]
            vakh = tampunglist[xsiapa][4]
            tampunglist[xsiapa] = ubahnim, vtug, vuts, vuas, vakh
            x.field_names = ["No", "NAMA", "NIM", "TUGAS", "UTS", "UAS", "AKHIR"]
            for tdata in tampunglist.items():
                i += 1
                x.add_row([i,  tdata[0], tdata[1][0], tdata[1][1], tdata[1][2], tdata[1][3], tdata[1][4]])
            print(x)
        elif mhs == 2:
            ubahtugas = int(input("Masukkan Nilai TUGAS Yang Benar"))
            i = 0
            vnim = tampunglist[xsiapa][0]
            vuts = tampunglist[xsiapa][2]
            vuas = tampunglist[xsiapa][3]
            vakh = tampunglist[xsiapa][4]
            tampunglist[xsiapa] = vnim, ubahtugas, vuts, vuas, vakh
            x.field_names = ["No", "NAMA", "NIM", "TUGAS", "UTS", "UAS", "AKHIR"]
            for tdata in tampunglist.items():
                i +=  1
                x.add_row([i, tdata[0], tdata[1][0], tdata[1][1], tdata[1][2], tdata[1][3], tdata[1][4]])
            print(x)
        elif mhs == 3:
            ubahuts = int(input("Masukkan Nilai UTS yang benar : "))
            i = 0
            vnim = tampunglist[xsiapa][0]
            vtug = tampunglist[xsiapa][1]
            vuas = tampunglist[xsiapa][3]
            vakh = tampunglist[xsiapa][4]
            tampunglist[xsiapa] = vnim, vtug, ubahuts, vuas, vakh
            x.field_names = ["No", "NAMA", "NIM", "TUGAS", "UTS", "UAS", "AKHIR"]
            for tdata in tampunglist.items():
                i = 1
                x.add_row([i, tdata[0], tdata[1][0], tdata[1][1], tdata[1][2], tdata[1][3], tdata[1][4]])
            print(x)
        elif mhs == 4:
            ubahuas = int(input("Masukkan Nilai UAS yang benar : "))
            i = 0
            vnim = tampunglist[xsiapa][0]
            vtug = tampunglist[xsiapa][1]
            vuts = tampunglist[xsiapa][2]
            vakh = tampunglist[xsiapa][4]
            tampunglist[xsiapa] = vnim,  vtug, vuts, ubahuas, vakh
            x.field_names = ["No", "NAMA", "NIM", "TUGAS", "UTS", "UAS", "AKHIR"]
            for tdata in tampunglist.items():
                i += 1
                x.add_row([i, tdata[0], tdata[1][0], tdata[1][1], tdata[1][2], tdata[1][3], tdata[1][4]])
            print(x)
        else:
            print("!!! === ERROR! Anda Memasukkan pilihan yang Salah === !!!")
    else:
        print("!!! === ERROR! DATA TIDAK TERSEDIA === !!!")


print("===== APLIKASI PENGOLAHAN DATA NILAI MAHASISWA =====")
while True:
    print("MENU : \n 1. Tanbah Data \n 2. Lihat Data \n 3. Ubah Data \n 4. Hapus Data \n 5. Keluar Aplikasi")
    pilih = int(input("Pilih Menu (1/2/3/4/5) : "))
    if pilih == 1:
        tambah()
    elif pilih == 2:
        tampilkan()
    elif pilih == 2:
        tampilkan()
    elif pilih == 3:
        print("========== UBAH DATA NILAI MAHASISWA ==========")
        print("Data siapa yang akan diubah ?")
        siapa = input("Masukkan Nama Mahasiswa yang akan diubah : ")
        ubah(siapa)
    elif pilih == 4:
        print("========== HAPUS DATA NILAI MAHASISWA ==========")
        print("Data siapa yang akan diubah ?")
        hsiapa = input("Masukkan Nama Mahasiswa yang akan diubah : ")
        hapus(hsiapa)
    elif pilih == 5:
        break
    else:
        print("!!! === ERROR! Anda Memasukkan Pilihan yang Salah === !!!")
```
