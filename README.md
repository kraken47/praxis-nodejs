# :dart: Challange of The Week 
<p>Lucinta adalah seorang staff TU Fakultas Teknik Universitas Muhmmad Fattah di Jakarta Selatan. Dalam kesehariannya Lucinta berurusan dengan banyak data yang berkaitan dengan mahasiswa, dosen, mata kuliah, dan nilai. Suatu hari Lucinta memiliki ide untuk membuat Sistem Informasi Akademis Kampus (SIAK) untuk memudahkan pekerjaanya. 

Ayo bantu Lucinta untuk membuat SIAK dengan ketentuan sebagai berikut:
1. *Database* memiliki *collection* Users, Roles, Reset_Passwords, Subjects, dan Credits.
2. *Collection* Users akan digunakan untuk menampung data mahasiswa, dosen, dan staff adminisitrasi kampus. memiliki atribut seperti berikut:<br>
		- name (string, required)<br>
		- email (string, required, unique)<br>
		- username (string, required, unique)<br>
		- role_id (string, required)<br>
		- password (string, required)<br>
		- handphone (string)<br>
		- created_at (date)<br>
		- updated_at (date)<br>
		- deleted_at (date)<br>
3. *Collection* Roles akan digunakan untuk menampung hak akses dengan ketentuan: <br>
		- Role Mahasiswa: hanya bisa login dan melihat (*listing)* jadwal mata kuliah dan nilai.<br>
		- Role Dosen: bisa melakukan CRUD mata kuliah dan nilai.<br>
		- Role Staff_admin: Hanya bisa membuat CRUD user untuk dosen dan mahasiswa.<br>
4. Collection* Reset_Passwords akan digunakan untuk data sementara yang dibutuhkan untuk keperluan reset password dengan ketentuan: <br>
		- Forgot password membutuhkan user menginput emailnya untuk meminta token reset.<br>
		- Token dikirimkan ke email (disarankan memakai mailtrap.io) user untuk dipakai menguah password.<br>
		- Setelah password dirubah, user akan diperlihatkan password barunya.<br>
5. Collection* Subjects akan digunakan untuk menampung informasi terkait mata kuliah. *Collection* tersebut memiliki ketentuan sebagai berikut: <br>
		- name (string, required)<br>
		- code (string, misal: Interaksi Manusia & Komputer ada di semester 4 :arrow_right: IMK4 )<br>
		- semester (number)<br>
		- lecturer_id (string)<br>
		- sks (number)<br>
		- credit_id (string)<br>
6.  Collection* Credits akan digunakan untuk data nilai mata kuliah yang diperoleh mahasiswa dengan ketentuan: <br>
		- subject_id (string)<br>
		- user_id (string, berisi ObjectId user yang memiliki role sebagai mahasiswa)<br>
		- score_uas (number)<br>
		- score_uts (number)<br>
		- score_final (string)<br>
</p>

## :dancer: Let's get the things done, have fun! :man_dancing: 


Hasil project dikumpulkan melalui repo ini dengan branch nama masing-masing. 
<br><sup>* *Disclaimer:* nama tokoh atau instanasi hanya fiktif belaka</sup>

<p align="center">  <img src="https://media.tenor.com/images/5df2ae103bd507ca686e7c267bc27a38/tenor.gif">  </p>


