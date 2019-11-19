# Praktikum-4

##Langkahnya

1. membuat list
- nilai = []
- ulang = True
2. Akan terus terjadi looping apabila menginput 'y'
- while ulang:
3. Memasukkan nama mahasiswa
-  nama = input("Masukkan Nama: ")
4. Memasukkan NIM mahasiswa
- nim = input("Masukkan NIM: ")
5. Memasukkan nilai tugas
- tugas = int(input("Masukkan Nilai Tugas: "))
6. Memasukkan nilai uts
- uts = int(input("Masukkan Nilai UTS: "))
7. Memasukkan nilai uas
- uas = int(input("Masukkan Nilai UAS: "))
8. Menghitung jumlah dari nilai tugas, uts, dan uas
- akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
9. akan masuk ke dalam list 'nama, tugas, uts, dan uas'
- nilai.append([nama, nim, int(tugas), int(uts), int(uas), int(akhir)])
10. Mengontrol looping, 'y' untuk lanjut dan 't' untuk berhenti
-  if (input("Tambah data (y/t)?") == 't'):
11. Cetak hasil
- print("\nDaftar Nilai Mahasiswa")
- print("====================================================================")
- print("|No. |     Nama     |    NIM    |  Tugas  |  UTS  |  UAS  |  Akhir |")
- print("====================================================================")
- i = 0
12. len digunakan untuk menghitung panjang suatu list
- for item in nilai:
-     i += 1
-     print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:7d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"
-           .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))
- print("====================================================================")
