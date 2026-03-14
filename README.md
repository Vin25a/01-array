for i in range(10):
    n = int(input(f"Masukkan nilai mahasiswa ke-{i+1}: "))
    nilai.append(n)

for i in range(10) 
artinya perulangan sebanyak 10 kali (karena ada 10 mahasiswa)

input()
meminta pengguna memasukkan nilai mahasiswa dari keyboard

f"Masukkan nilai mahasiswa ke -{i+1}: "))
menampilkan teks seperti:
-Masukkan nilai mahasiswa ke-1
-Masukkan nilai mahasiswa ke-2

int()
mengubah input menjadi angka(integer)

nilai.append(n)
menyimpan nilai tersebut ke dalam list bernama nilai


nilai_tertinggi = max(nilai)
nilai_terendah = min(nilai)
rata_rata = sum(nilai) / len(nilai)

max(nilai)
mencari nilai terbesar

min(nilai)
mencari nilai terkecil

sum(nilai)
menjumlahkan semua nilai

len(nilai)
menghitung jumlah data

sum(nilai) / len(nilai)
menghitung rata-rata nilai


lulus = sum(1 for n in nilai if n >= 60)
tidak_lulus = len(nilai) - lulus

if n >= 60
mahasiswa lulus jika nilai ≥ 60

sum(1 for n in nilai if n >= 60)
menghitung berapa mahasiswa yang lulus


import matplotlib.pyplot as plt

plt.bar(["Tertinggi", "Terendah"], [nilai_tertinggi, nilai_terendah])
plt.title("Grafik Nilai Mahasiswa")
plt.show()

matplotlib.pyplot
library Python untuk membuat grafik

plt.bar()
membuat grafik batang


plt.pie(
    [lulus, tidak_lulus],
    labels=["Lulus", "Tidak Lulus"],
    autopct="%1.1f%%"
)

plt.title("Persentase Kelulusan")
plt.show()

plt.pie()
membuat diagram lingkaran

[lulus, tidak_lulus]
data yang ditampilkan

labels
memberi nama pada tiap bagian

autopct="%1.1f%%"
menampilkan persentase
