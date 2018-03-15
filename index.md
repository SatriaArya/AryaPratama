# Program Python Menghitung Dan Menampilkan Sebuah Data

# Python
Python adalah bahasa pemrograman interpretatif multiguna dengan filosofi perancangan yang berfokus pada tingkat keterbacaan kode.
Python diklaim sebagai bahasa yang menggabungkan kapabilitas, kemampuan, dengan sintaksis kode yang sangat jelas,
dan dilengkapi dengan fungsionalitas pustaka standar yang besar serta komprehensif. Python juga didukung oleh komunitas yang besar.

# Yang Dibutuhkan Untuk Menjalankan Program Python ini :
1.Terlebih Dahulu install Python Untuk Windows di https://www.python.org ( Saya Memakai Python 3.6.4 ) 

2.Install PIP dan texttable Dahulu https://pypi.python.org/pypi/texttable & https://pypi.python.org/pypi/pip.
  Install melalui cmd ( Win+R >>> CMD >>> cd (masuk ke folder texttable yang sudah diextract yaa) >> jika sudah masuk Ketikan "python setup.py install" >>> lalu ketikan lagi "pip setup.py install pada folder PIP.rar yang sudah diextract 

3.Jika Sudah Terinstall Masuk Ke Idle Python ( Cari Di Pencarian Windows )

4.File >> New File >> Lalu Masuka Koding Sourcenya 

from texttable import Texttable

table = Texttable ()

jawab = "y"

no = 0

nama = []

nim = []

nilai_tugas = []

nilai_uts = []

nilai_uas = []

while( jawab == "y"):
    
		nama.append(input("Masukan Nama  :"))
    
		nim.append(input("Masukan Nim   :"))
    
		nilai_tugas.append(input("Nilai Tugas   :"))
    
		nilai_uts.append(input("Nilai UTS     :"))
    
		nilai_uas.append(input("Nilai UAS     :"))
    
		jawab = input("Tambah data (y/t)?")
    
		no += 1

for i in range(no):
    
		tugas = int(nilai_tugas[i])
    
		uts = int(nilai_uts[i])
    
		uas = int(nilai_uas[i])
    
		akhir = (tugas*30/100) + (uts*35/100) + (uas*35/100)
    
		table.add_rows([['No','Nama','Nim','Tugas','UTS','UAS','AKHIR'],
                    [i+1, nama[i],nim[i],nilai_tugas[i],nilai_uts[i],nilai_uas[i],akhir]])

print (table.draw())

# Saya akan menjelaskan sedikit tentang koding resourcenya 
1.from texttable import Texttable & table = Texttable (). ( perintah untuk melakukan pemanggilan module texttable yang akan ditampilkan di output table )

2.while( jawab == "y"): ( perintah untuk perintah mengulang sebuah pertanyaan )

3.jawab = input("Tambah data (y/t)?") ( perintah untuk menanyakan tambahan sebuah data yang akan di input ulang jika menjawab "y" akan menambahkan input data jika jawab "t" maka akan berhenti

4.append() ( perintah untuk menambakan data/item dari belakang )

5.input() ( perintah untuk digunakan untuk mengambil data angka )

6.int() ( perintah untuk bilangan bulat berbeda dengan float() yaitu pecahan )

7.for i in range(no): ( perintah untuk melakukan perlulangan sampai batas atau range yang di tentukan )

8.table.add_rows( perintah untuk menambakan baris pada table 

sekian dari saya terima kasih, terima kasih atas waktunya sudah mau membaca walaupun berantakan ( masih belajar ) next saya akan buat 
web saya akan lebih bagus dan menarik sekian.

