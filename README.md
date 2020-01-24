# :dart: Challange of The Week 
Lucinta adalah seorang staff TU Fakultas Teknik Universitas Muhmmad Fattah di Jakarta Selatan. Dalam kesehariannya Lucinta berurusan dengan banyak data yang berkaitan dengan mahasiswa, dosen, mata kuliah, dan nilai. Suatu hari Lucinta memiliki ide untuk membuat Sistem Informasi Akademis Kampus (SIAK) untuk memudahkan pekerjaanya. 

Ayo bantu Lucinta untuk membuat SIAK dengan ketentuan sebagai berikut:
1. *Database* memiliki *collection* Users, Roles, Reset_Passwords, Subjects, dan Credits.
2. *Collection* Users akan digunakan untuk menampung data mahasiswa, dosen, dan staff adminisitrasi kampus. memiliki atribut seperti berikut:
		- name (string, required)
		- email (string, required, unique)
		- username (string, required, unique)
		- role_id (string, required)
		- password (string, required)
		- handphone (string)
		- created_at (date)
		- updated_at (date)
		- deleted_at (date)
3. *Collection* Roles akan digunakan untuk menampung hak akses dengan ketentuan: 
		- Role Mahasiswa: hanya bisa login dan melihat (*listing)* jadwal mata kuliah dan nilai.
		- Role Dosen: bisa melakukan CRUD mata kuliah dan nilai.
		- Role Staff_admin: Hanya bisa membuat CRUD user untuk dosen dan mahasiswa.
4. Collection* Reset_Passwords akan digunakan untuk data sementara yang dibutuhkan untuk keperluan reset password dengan ketentuan: 
		- Forgot password membutuhkan user menginput emailnya untuk meminta token reset.
		- Token dikirimkan ke email (disarankan memakai mailtrap.io) user untuk dipakai menguah password.
		- Setelah password dirubah, user akan diperlihatkan password barunya.
5. Collection* Subjects akan digunakan untuk menampung informasi terkait mata kuliah. *Collection* tersebut memiliki ketentuan sebagai berikut: 
		- name (string, required)
		- code (string, misal: Interaksi Manusia & Komputer ada di semester 4 :arrow_right: IMK4 )
		- semester (number)
		- lecturer_id (string)
		- sks (number)
		- credit_id (string)
6.  Collection* Credits akan digunakan untuk data nilai mata kuliah yang diperoleh mahasiswa dengan ketentuan: 
		- subject_id (string)
		- user_id (string, berisi ObjectId user yang memiliki role sebagai mahasiswa)
		- score_uas (number)
		- score_uts (number)
		- score_final (string)


## :dancer: Let's get the things done, have fun! :man_dancing: 


Hasil project dikumpulkan di melalui repo ini dengan branch nama masing-masing. 
<sup>* *Disclaimer:* nama tokoh atau instanasi hanya fiktif belaka</sup>

<p align="center">  <img src="https://media.tenor.com/images/5df2ae103bd507ca686e7c267bc27a38/tenor.gif">  </p>


