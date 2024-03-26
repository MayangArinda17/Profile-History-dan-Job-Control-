# Profile-History-dan-Job-Control-




1. Eksekusi seluruh profile yang ada :



    a. Edit file  profile  /etc/profile  dan  tampilkan pesan  sebagai berikut  :    echo  “Profile dari /etc/profile”





   ![2024-03-25_11-05](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/56bf5068-442e-4d5b-a714-91edfddb6620)







   ![2024-03-25_11-04](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/23313947-7b8b-405d-9460-a502009a98bb)





   ![2024-03-25_11-07](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/af133d3a-b96c-465f-8148-e82169d5ec50)





   b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :




      /home/stD02001/.bash_profile






   ![2024-03-25_11-10](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/adddbafc-90ef-4b75-891d-a48a717a0909)






    /home/stD02001/.bash_login







   ![2024-03-25_11-11](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/ac42c257-67cb-41c2-8977-5a200ae56ff5)






    /home/stD02001/.profile






   ![2024-03-25_11-13](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/917e9562-cf9a-4f8e-86cf-451dd1d8e2ba)






  /home/stD02001/.bashrc







  ![2024-03-25_11-17_1](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/c29aa8f9-f20a-4823-8e2c-4b4db4025a81)







Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap 
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
echo “Profile dari .bash_profile” 
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang 
bersangkutan. 








![2024-03-25_11-09](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/d37f5d66-d014-4062-a5e8-eaa3bdaafdd1)







![2024-03-25_11-12](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/b8bc6450-ecb2-4d77-808b-cc7835dd46f6)







![2024-03-25_11-15](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/b0088343-5ba8-4f91-a9f3-efe290151771)







![2024-03-25_11-17](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/26ed8faf-5d6d-4e82-b486-8f76cd70cfb0)






![2024-03-25_11-17_1](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/d64c65d5-215d-4986-a43b-99474de19ca6)






![2024-03-25_11-20](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/57f8d3d1-fadb-4656-833b-1f30b1558fbf)







![2024-03-25_11-23](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/f28be599-7186-4452-8ab7-ccf9276fc343)










c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut: 
$ su mahasiswa 
$ exit








![2024-03-25_11-24](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/512ce705-646d-4423-aa74-e105352bee84)









Jelaskan perbedaan kedua utilitas tersebut. 
2. Prompt String (PS) 
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan 
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell 
PS1=‟> „ 
export PS1 
b. Eksperimen hasil PS1 :
$ PS1=“\! > “ 
69 > PS1=”\d > “ 
Mon Sep 23 > PS1=”\t > “ 
10:10:20 > PS1=”Saya=\u > “ 
Saya=mahasiswa > PS1=”\w >” 
~ > PS1=\h >”





![2024-03-25_11-33](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/ed9a209a-3d20-43f3-9184-e78d538a0fd4)









3. Logout 
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout 
Echo “Terima kasih atas sesi yang diberikan”
Sleep 5 
clear







![2024-03-25_11-39_1](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/2ce12fd3-8d5d-45da-9855-81e1ac3331cf)







![2024-03-25_12-10](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/e77c2898-caa7-4c4e-b50e-3f855dd0aece)






![2024-03-25_12-11](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/53ff3eac-ba41-4e5b-9c6a-130c926d39d7)








4. Bash script 
a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing : 
p1.sh 
#! /bin/bash 
echo “Program p1” 
ls –l 
p2.sh 
#! /bin/bash 
echo “Program p2” 
who 
p3.sh 
#! /bin/bash 
echo “Program p3” 
ps x









![2024-03-25_12-16_1](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/d3979238-6b1d-4d36-a359-4403169c5602)










![2024-03-25_12-16](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/b39b2319-b132-4986-a69b-c2986f74b923)










![2024-03-25_12-18](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/f5a481d3-989c-4a5c-bd55-f576ee2e84c9)










![2024-03-25_12-23](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/37fb5361-416e-4416-8a76-c1cf0eae6215)







![2024-03-25_12-23](https://github.com/MayangArinda17/Profile-History-dan-Job-Control-/assets/150981696/2b43a4db-fc4e-40a9-b75f-a5a5831ca682)






















  

 






   






   




   









   
