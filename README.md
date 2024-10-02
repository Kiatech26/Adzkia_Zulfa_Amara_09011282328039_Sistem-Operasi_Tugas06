# Adzkia_Zulfa_Amara_09011282328039_Sistem-Operasi_Tugas06

# Job Control

# 1. Eksekusi seluruh profile yang ada :
# a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
# echo “Profile dari /etc/profile”
# Perintahnya

<img width="315" alt="Perintah 1" src="https://github.com/user-attachments/assets/4bea88f0-70c1-4002-9afa-185af573914f">


# 2. b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
#/home/stD02001/.bash_profile
#/home/. stD02001/.bash_login
#/home/mahasiswa/.profile
#/home/mahasiswa/.bashrc
#Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
#file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
#echo “Profile dari .bash_profile”
#Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang
#bersangkutan. 

<img width="401" alt="echo bash profile" src="https://github.com/user-attachments/assets/0fd4908f-a3b9-4e8f-bfaa-865473911f83">

<img width="271" alt="perintah 2a" src="https://github.com/user-attachments/assets/b6446b5c-0fb5-4a8d-97b7-19426791eb5d">

<img width="350" alt="perintah 2b" src="https://github.com/user-attachments/assets/8318451b-2f9c-46c5-a1ee-beed21741637">

<img width="268" alt="perintah 2a2" src="https://github.com/user-attachments/assets/aae3b6d2-c97b-4f95-92a2-867e2d6d421d">

<img width="424" alt="perintah 2b2" src="https://github.com/user-attachments/assets/1d0e4f54-c771-443c-9ac6-45f10e9113b5">

<img width="260" alt="perintah 2a3" src="https://github.com/user-attachments/assets/bc3b9ef7-9739-4701-ac49-ae0da69daabd">

<img width="394" alt="perintah 2b3" src="https://github.com/user-attachments/assets/bf658a05-b1a6-4352-b5d6-4bc628b61aac">

# bash_profile adalah file konfigurasi di shell Bash yang digunakan untuk menginisialisasi lingkungan pengguna saat melakukan login shell. 
# bash_login adalah file skrip yang dijalankan secara otomatis saat seorang pengguna masuk (login) ke sistem menggunakan shell Bash.
# profile : File ini digunakan untuk menetapkan variabel lingkungan, fungsi, dan perintah yang akan dieksekusi setiap kali Anda membuka sesi shell baru (seperti terminal).
# ~/.bashrc adalah file konfigurasi untuk shell Bash yang dijalankan setiap kali pengguna membuka shell interaktif non-login, seperti saat membuka terminal baru di dalam sesi yang sedang berlangsung.

# c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
# $ su mahasiswa
# $ exit
# kemudian gunakan opsi – sebagai berikut :
# $ su – mahasiswa
# $ exit
# Jelaskan perbedaan kedua utilitas tersebut. 
su mahasiswa: Hanya mengganti pengguna tanpa mengubah lingkungan (variabel lingkungan tetap sama seperti pengguna sebelumnya).

<img width="187" alt="Perintah 3a" src="https://github.com/user-attachments/assets/dd0cb780-78dc-4bef-939d-f414ddef3766">

<img width="161" alt="perintah 3b" src="https://github.com/user-attachments/assets/24df4456-5fcb-4ae4-8b8c-4a431c04d5f5">

su - mahasiswa: Mengganti pengguna sekaligus memuat lingkungan pengguna yang dituju, seolah-olah Anda baru login sebagai pengguna tersebut.

<img width="178" alt="perintah 3a2" src="https://github.com/user-attachments/assets/afbb0423-5fd2-4631-a782-85d00b413d09">

<img width="168" alt="perintah 3b2" src="https://github.com/user-attachments/assets/1b045bdd-325c-4e26-aaf7-8f89bbf22e9a">


2. Prompt String (PS)
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
PS1=‟> „
export PS1

<img width="276" alt="Perintah 4a" src="https://github.com/user-attachments/assets/e358fdf8-83aa-4f1b-ac1a-e056aa3e4c5c">

<img width="226" alt="perintah 4b" src="https://github.com/user-attachments/assets/61f21f23-a12d-41f2-bf90-906fcff65c10">

# Perintah PS1="> " digunakan untuk mengubah tampilan prompt di shell Bash.
# PS1: Merupakan singkatan dari Prompt Statement 1, variabel ini mendefinisikan apa yang ditampilkan oleh shell saat menunggu input dari pengguna.
# "> ": Adalah string yang menentukan tampilan prompt. Di sini, prompt hanya menampilkan tanda > tanpa informasi tambahan

b. Eksperimen hasil PS1 : 

$ PS1=“\! > “
69 > PS1=”\d > “
Mon Sep 23 > PS1=”\t > “
10:10:20 > PS1=”Saya=\u > “
Saya=mahasiswa > PS1=”\w >”
~ > PS1=\h >” 

# PS1=“\! > “ = Perintah ini akan menampilkan nomor urut perintah (histori) setiap kali Anda mengetik sesuatu
<img width="233" alt="perintah21" src="https://github.com/user-attachments/assets/0f5a3b91-77e3-41bd-87eb-12aad6ea94cf">

# PS1=”\d > “ = menampilkan tanggal saat ini di prompt
<img width="104" alt="perintah22" src="https://github.com/user-attachments/assets/ab29014b-2fd5-436b-afdb-ea110a27a960">


# PS1=”\t > “ = Untuk menampilkan waktu dalam format 24 jam:
<img width="111" alt="perintah23" src="https://github.com/user-attachments/assets/c45fd137-aaa1-43b5-a6cf-df14da6b987f">

# PS1=”Saya=\u > “ =  menampilkan nama pengguna (misalnya Adzkia)

<img width="118" alt="perintah24" src="https://github.com/user-attachments/assets/b14149f6-e11d-4535-b6d1-adf5ec2c92da">

# PS1=”\w >” = ingin menampilkan direktori kerja saat ini

<img width="117" alt="perintah25" src="https://github.com/user-attachments/assets/85e50490-f543-45fd-81c7-8496ef43acde">

#  > PS1=\h >” = Untuk menampilkan nama host (hostname) sistem
<img width="114" alt="perintah 26" src="https://github.com/user-attachments/assets/4e2e05f0-b3c4-4921-93a7-840c8dff5210">

# 3. Logout
# Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
# Echo “Terima kasih atas sesi yang diberikan”
# Sleep 5
# clear 

# perintah berikut untuk membuka atau membuat file .bash_logout:
<img width="232" alt="perintah31" src="https://github.com/user-attachments/assets/3340f72f-603c-4ad1-b77f-00452b51d207">

# Tambahkan Perintah 
# echo: Menampilkan pesan "Terima kasih atas sesi yang diberikan".
# sleep 5: Menunda selama 5 detik sebelum melanjutkan ke perintah berikutnya.
# clear: Membersihkan layar terminal sebelum keluar.

<img width="459" alt="perintah 32" src="https://github.com/user-attachments/assets/fbea43a4-6b9f-4817-b3fc-cd7a81895583">

# Ketika Anda mengetik logout, terminal akan menampilkan pesan "Terima kasih atas sesi yang diberikan", 
# menunggu selama 5 detik, kemudian membersihkan layar dan menutup sesi.

<img width="209" alt="perintah 33" src="https://github.com/user-attachments/assets/58cda68f-334f-40c6-acf3-69aa0eb8f899">

# 4. Bash script
# script itu adalah daftar perintah-perintah yang kita tulis agar komputer tahu apa yang harus dikerjakannya, dan komputer akan mengikuti perintah-perintah itu secara berurutan.
# a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
# p1.sh

<img width="225" alt="perintah 4a1" src="https://github.com/user-attachments/assets/a9010bf4-7693-4753-8208-ea9defd010de">

# ##! /bin/bash
# echo “Program p1”
# ls –l

<img width="390" alt="perintah 4a2" src="https://github.com/user-attachments/assets/7c582e75-fb33-4547-aa42-7f5f92274872">

# p2.sh

<img width="196" alt="perintah 4a3" src="https://github.com/user-attachments/assets/2b078a9c-8e56-44a5-a29a-342998740470">


# #! /bin/bash
# echo “Program p2”
# who

<img width="429" alt="perintah 4a4" src="https://github.com/user-attachments/assets/8f844fc3-3141-45a7-b36f-e6759e95ba86">

# p3.sh

<img width="191" alt="perintah 4a5" src="https://github.com/user-attachments/assets/f60ba33a-8721-487b-b155-3306d0956aea">


# #! /bin/bash
# echo “Program p3”
# ps x

<img width="390" alt="perintah 4a6" src="https://github.com/user-attachments/assets/e0491929-bd67-4f46-bb38-057623c95f74">


# b. Jalankan script tersebut sebagai berikut :
# $ ./p1.sh ; ./p3.sh ; ./p2.sh
# Jalankan semua script secara berurutan satu per satu
<img width="350" alt="perintah 4b1" src="https://github.com/user-attachments/assets/00de7fb9-ca9e-49d0-9324-83abbf07e1cc">
# Perintah ini akan menjalankan p1.sh, kemudian p3.sh, lalu p2.sh secara berurutan. Setiap script akan dijalankan setelah script sebelumnya selesai.

# $ ./p1.sh &
# untuk menjalankan script p1.sh di background (berjalan tanpa menunggu)
<img width="288" alt="perintah 4b2" src="https://github.com/user-attachments/assets/1fcf71e7-70bc-4649-9f8c-ec05e360b3b8">
# Tanda & di akhir perintah menunjukkan bahwa script tersebut akan dijalankan di background, sehingga terminal tetap bisa digunakan untuk perintah lain.

# $ ./p1.sh $ ./p2.sh & ./p3.sh &
# Untuk menjalankan beberapa script secara bersamaan di background
<img width="329" alt="perintah 4b3" src="https://github.com/user-attachments/assets/8da433a4-6fd6-4412-9deb-4b2fe010f426">
# Semua script akan berjalan secara paralel di background.

# $ ( ./p1.sh ; ./p3.sh ) & 
#  menjalankan p1.sh dan p3.sh secara berurutan, tetapi keduanya di background

<img width="278" alt="perintah 4b4" src="https://github.com/user-attachments/assets/0eb91184-38a0-4658-b8ec-ec666ab4d73f">

# Dengan tanda kurung (), p1.sh dan p3.sh dijalankan secara berurutan, dan setelah keduanya selesai, mereka akan tetap di background karena adanya &.

# 5. Jobs
# a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh,
# Buat file baru bernama pwaktu.sh dengan editor teks, misalnya nano
<img width="199" alt="perintah 5a1" src="https://github.com/user-attachments/assets/96820e7a-4b2d-4182-8e7d-8bb27343d749">

# setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil. 
# #!/bin/bash
# while [ true ]
# do
# date >> hasil
# sleep 10
# done 
Masukkan isi berikut ke dalam file
<img width="159" alt="perintah 5a2" src="https://github.com/user-attachments/assets/e20bf916-8549-4e4a-9c2c-0ca4ecada54c">


b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background
sebagai berikut :
# Tanda & berarti script akan berjalan di background, sehingga terminal tidak akan terkunci dan bisa digunakan untuk perintah lain.
# $ jobs

<img width="213" alt="perintah 5b1" src="https://github.com/user-attachments/assets/ecfa94e8-4e08-4f02-8d60-98e09ef5c75f">

# Untuk melihat proses yang sedang berjalan di background

# $ find / -print > files 2>/dev/null &

<img width="283" alt="perintah 5b2 benar" src="https://github.com/user-attachments/assets/e25e5233-df72-475d-86f7-25ec2ff2595c">
# find untuk mencari file di sistem dan menyimpan hasilnya ke file files
# $ jobs 

<img width="277" alt="perintah 5b3 benar" src="https://github.com/user-attachments/assets/3dec1ec4-c64d-42a3-a28f-5953fc899987">

# Jobs kedua digunakan untuk menjalankan proses atau program lain di background, sekaligus memanage beberapa pekerjaan (jobs) yang berjalan di background.

# c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

<img width="206" alt="perintah 5c1" src="https://github.com/user-attachments/assets/97bef848-d894-4d99-a4fc-f2a7597b5b85">

# Untuk melihat proses yang sedang berjalan di background

# $ fg %1
# Menggunakan fg %1 untuk membawa job pertama ke foreground.
<img width="216" alt="perintah 5c2" src="https://github.com/user-attachments/assets/be0fbba1-6741-485d-9084-ab7db7f9512f">
# Menggunakan Ctrl + Z untuk menghentikan sementara job yang berjalan di foreground.

# $ bg 

<img width="183" alt="perintah 5c3 benar" src="https://github.com/user-attachments/assets/8abe4e45-f478-4397-81c1-c2d29dd5cbf1">
# Perintah bg dalam sistem operasi berbasis Unix/Linux digunakan untuk melanjutkan proses yang sebelumnya dihentikan (suspended) dan menjalankannya kembali di background. 
# Perintah bg %1 digunakan untuk melanjutkan job pertama (job dengan nomor ID 1) yang sebelumnya dihentikan (suspended) dan menjalankannya kembali di background.


# d. Stop program background dengan utilitas kil
# $ ps x
<img width="221" alt="perintah 5d1" src="https://github.com/user-attachments/assets/42863eba-0d75-4329-be13-cb9a4fc2aee2">
# ps x Untuk melihat semua proses yang sedang berjalan, gunakan perintah:

# $ kill [Nomor PID] 
cari nomor PID dari program yang ingin duhentikan.

# Untuk melihat proses serta melihat Nomor PID yang telah dihapus dengan #PX
<img width="220" alt="perintah 5d2" src="https://github.com/user-attachments/assets/100c4753-b7e1-4dc2-9c7e-408468f652e8">

# Untuk menghentikan (stop) program yang berjalan di background menggunakan perintah kill
Hentikan Proses dengan kill: Setelah mengetahui PID, Anda dapat menghentikan proses tersebut . Disisni saya kill ID 25209

# Untuk melihat proses serta melihat Nomor PID yang telah dihapus dengan px
<img width="238" alt="perintah 5d3 memeriksa px" src="https://github.com/user-attachments/assets/24b5f572-7b83-4779-b7f1-7e5306b56b79">



# 6. History
# a. Ganti nilai HISTSIZE dari 1000 menjadi 20
# $ HISTSIZE=20
# HISTSIZE adalah variabel lingkungan dalam Bash yang menentukan jumlah maksimum perintah yang akan disimpan dalam riwayat (history) sesi terminal Secara default, nilai ini biasanya lebih besar, seperti 1000. kenapa 20 karena menyimpan riwayat perintah yang lebih kecil dapat membantu mengurangi penggunaan memori dan meningkatkan kinerja terminal.
HISTSIZE=20: Mengubah ukuran history menjadi 20 perintah.
<img width="176" alt="perintah 6a1" src="https://github.com/user-attachments/assets/db65eaef-6c87-4bc2-8a57-435e8c6441ed">


# $ h

<img width="190" alt="perintah 6a2" src="https://github.com/user-attachments/assets/6d2ccdb5-c222-49ae-9c72-209b51593eca">

# perintah history (atau hanya h jika sudah ada alias) digunakan untuk menampilkan daftar perintah yang telah Anda jalankan sebelumnya dalam sesi terminal. 

# b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir
# dilakukan

# # $ !-5
<img width="152" alt="perintah 6b" src="https://github.com/user-attachments/assets/aea26a20-bf27-448b-95ba-156885ebb1d3">

#Ulangi perintah kelima terakhir

# c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
# $ !!
# Ulangi perintah terakhir
<img width="159" alt="perintah 6c" src="https://github.com/user-attachments/assets/7b97729f-9605-4cb7-bab4-67e811a4e772">


# d. Ulangi instruksi pada history bufer nomor 150
# $ !150
# Ulangi perintah nomor 150
<img width="147" alt="perintah 6d" src="https://github.com/user-attachments/assets/73548127-9bd5-4aa5-8df6-6e9cbba4b119">


# e. Ulangi instruksi dengan prefix “ls”
# $ !ls 
#Ulangi perintah yang dimulai dengan ls
<img width="386" alt="perintah 6e" src="https://github.com/user-attachments/assets/e206c4b0-72be-468f-a630-c6d15abeb46e">
# !: Tanda seru (!) digunakan untuk mengakses riwayat perintah
# Dengan menuliskan !ls, meminta shell untuk mencari perintah terakhir dalam riwayat yang dimulai dengan ls.







