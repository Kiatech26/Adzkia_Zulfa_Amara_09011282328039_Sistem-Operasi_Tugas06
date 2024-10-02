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






