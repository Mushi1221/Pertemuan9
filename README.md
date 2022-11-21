# Pertemuan9
Nama : Muhammad Shiddiq <br>
NIM : 312210125<br>
Kelas : TI.22.B1<br>

1. Soal Latihan pada Pertemuan 9
```python
# membuat list
print("Buat sebuah list sebanyak 5 elemen dengan nilai bebas")
list = [111, 222, 133, 3214, 45]
print(list)
# mengakses list
print("Menampilkan elemen 3")
print(list[2])
print("ambil nilai elemen 2 sampai ke 4")
print(list[1:4])
print("ambil elemen terakhir")
print(list[-1])
# mengubah elemen list
print("ubah elemen 4 dengan nilai lainnya")
list[4]=10
print(list[3])
print("ubah elemen 4 sampai dengan elemen terakhir")
list[4:5]=[20,11]
print(list)
# Tambah elemen list
print("Ambil 2 bagian dari list pertama(A) dan jadikan list ke 2(B)")
list_pertama=list[3:5]
print(list_pertama)
print("tambah list B dengan nilai string")
list_pertama.append("harlem")
print(list_pertama)
print("Tambah list B dengan 3 nilai")
list_pertama.append(["harlem",79,48])
print(list_pertama)
print("Menggabungkan list B dengan list A")
gabung=list_pertama+list
```
![Screenshot (64)](https://user-images.githubusercontent.com/115475520/202987033-5abf3030-1393-40a0-a938-87ddb17cc3d3.png)


2. Praktikum 4 
```Python
    # import package tabulate
    from tabulate import tabulate
    # membuat list kosong untuk menampung data
    dataMahasiswa = []
    no = 0
    # melakukan perulangan input sesuai keinginan sampai pertanyaan tambah data dimunculkan kembali
    while(True):
    # membuat variable untuk menampung inputan
    no += 1
    nama = input("Masukan Nama : ")
    nim = input("Masukan NIM : ")
    kelas = input("Masukan Kelas : ")
    matkul = input("Masukan Mata Kuliah : ")
    # mengkonversi string ke integer
    tugas = int(input("Masukan Nilai Tugas : "))
    uts = int(input("Masukan Nilai UTS : "))
    uas = int(input("Masukan Nilai UAS : "))
    # menjumlahkan nilai dari tugas,uts dan uas
    nilai_akhir = (tugas * 30 / 100) + (uts * 35 / 100) + (uas * 35 / 100)
    # lakukan pengecekan jika nilai_akhir lebih besar dari 50 maka Lulus selain itu tidak lulus dan mengulang mata kuliah
    if (nilai_akhir > 50):
        keterangan = "Lulus"
    else:
        keterangan = "Tidak Lulus, Mengulang Mata kuliah"
    # menambahkan data input ke list dataMahasiswa
    dataMahasiswa.append(
        [no, nama, nim, kelas, matkul, tugas, uts, uas, nilai_akhir, keterangan])
    # input tambah data jika tekan y maka input kembali, selain itu berhenti dan tampilkan data
    tambah_data_lagi = input("Tambah Data lagi ? (y/t) : ")
    if(tambah_data_lagi == "t"):
        break
    # tampilkan dataMahasiswa menggunakan tabulate package agar tampilan berbentuk table
    print(tabulate(dataMahasiswa, headers=[
          "No", "Nama", "Nim", "Kelas", "Mata Kuliah", "Tugas", "UTS", "UAS", "Nilai Akhir", "Keterangan"], tablefmt="fancy_grid"))
```
 

![pic praktikum4](https://user-images.githubusercontent.com/115475520/202988650-785e3262-686b-43ac-b5ec-9c5060bfc7e5.png)

3. Flowchart
 
 ![Screenshot (66)](https://user-images.githubusercontent.com/115475520/202988049-08069ff3-bcc3-45b9-a5cb-641eb9f8c357.png)
