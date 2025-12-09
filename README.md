**# Kelompok 9_Curse of the Forbidden Forest**

**Konsep Game**
Curse of the Forbidden Forest adalah sebuah game bergenre Third-Person Survival Mystery Horror yang berfokus pada eksplorasi, survival, dan moral choices. Pemain berperan sebagai Louis, seorang mahasiswa yang kembali ke desa terpencil setelah mengetahui bahwa adiknya, Lily, menghilang di dalam hutan larangan. Game ini menargetkan pemain berusia 18 tahun ke atas, terutama mereka yang menyukai cerita gelap, suasana mencekam, dan gameplay dengan tekanan psikologis. Platform pengembangan difokuskan pada PC (Windows) menggunakan Unity Engine.

**Core Mechanics dan Gameplay**
Gameplay utama dirancang untuk menciptakan pengalaman yang mendalam melalui eksplorasi lingkungan, sumber daya terbatas, dan interaksi dengan dunia yang misterius. Pemain menjelajah desa, hutan, dan katedral tua menggunakan perspektif third-person, dilengkapi dengan pistol dan senter sebagai alat survival. Amunisi sangat terbatas sehingga setiap tembakan menjadi keputusan penting. Pemain dapat menemukan clue berupa objek lingkungan yang memicu dialog naratif dan membantu membuka potongan cerita.

Musuh dalam game dapat dideteksi dari suara, siluet, atau jarak tertentu. Pemain dapat memilih untuk melawan musuh dengan risiko peluru habis, atau bersembunyi di balik objek di lingkungan. Tidak ada sistem healing item, sehingga setiap encounter membawa konsekuensi serius terhadap kelangsungan permainan.

**Story & Worldbuilding**
Cerita dimulai ketika Louis kembali ke desa kelahirannya setelah mendengar kabar hilangnya Lily. Saat malam dan badai tiba, ia memulai penyelidikan meskipun seorang penjaga hutan mencoba menghentikannya. Saat Louis memasuki hutan Blackveil, ia menemukan tanda-tanda kehadiran anak-anak yang hilang, termasuk benda-benda kecil yang dulu milik Lily. Semakin jauh ia masuk, semakin jelas bahwa makhluk yang mengejarnya dulunya adalah anak-anak tak berdosa yang dikorbankan dalam ritual gelap oleh sosok penyihir bernama Mora. Cerita mencapai puncaknya di reruntuhan katedral tua, tempat Mora menunggu. Pemain menentukan akhir cerita melalui tindakannya: menyelamatkan Lily dan semua anak yang hilang, atau mengakhiri kutukan dengan mengorbankan semuanya.

**Alur Cerita dan Implementasi Chapter:**
Game ini tidak menggunakan sistem level, melainkan menggunakan sistem chapter untuk mendukung alur cerita yang berkelanjutan. Setiap chapter merepresentasikan tahapan penting dalam perjalanan karakter Louis, sehingga progres permainan terasa lebih sinematik dan naratif.
- Awal Chapter 1: Interaksi dengan NPC Penjaga Hutan
  Pemain memulai permainan di depan gerbang desa dan bertemu dengan NPC Penjaga Hutan. Interaksi dilakukan menggunakan NPC Dialogue Script yang menampilkan dialog teks dengan tombol pilihan sebagai pembuka cerita.
- Chapter 2: Eksplorasi Hutan, Pertempuran Musuh, Health Bar, dan Implementasi SFX
  Pada chapter ini, Louis menjelajahi Hutan Blackveil untuk mencari adiknya. Di tengah perjalanan, pemain bertemu dengan musuh yang harus dikalahkan dengan menembak menggunakan pistol. Musuh telah dilengkapi
  dengan health bar berbasis script serta didukung oleh SFX pertempuran.
- Chapter 3: Pertarungan di Katedral Tua Melawan Mora
  Pada chapter terakhir, pemain memasuki katedral tua dan menghadapi boss Mora. Setelah Mora berhasil dikalahkan, akan muncul teks True Ending sebagai penanda bahwa pemain telah menyelesaikan seluruh rangkaian
  chapter dalam game.

**Visual & Audio Direction**
Atmosfer game dibentuk menggunakan palet warna gelap, kabut tebal, siluet pohon tinggi, dan lingkungan yang seakan menelan cahaya. Desain karakter dan lingkungan mengadopsi estetika gothic yang mendukung tema kesepian dan keputusasaan. Audio dibuat minimalis namun intens: suara ranting patah, napas Louis, hujan, dan bisikan samar anak-anak menjadi elemen horor utama. Musik hanya muncul di momen tertentu untuk memperkuat ketegangan.

**Arsitektur Teknis dan Sistem**
Game dikembangkan menggunakan arsitektur Component-Based dengan kombinasi model MVC/MVP. Script ditulis menggunakan C# (.cs) dalam folder-folder modular agar mudah dikembangkan. Sistem utama meliputi pengelolaan health, AI musuh dengan state chasing, sistem inventory tetap, clue trigger, dan sistem shooting yang mendukung raycast detection. Class seperti GameManager, PlayerStateSystem, AIManager, dan NarrativeManager bertanggung jawab terhadap logika inti permainan.

**Prototipe Playable**
Prototipe game telah mencakup:
- Movement karakter dan kamera third-person
- Sistem menembak dengan pistol
- AI musuh dengan perilaku mengejar
- Health system pemain dan musuh
- Clue trigger dan dialog NPC
- Boss Mora dan True Ending
- Implementasi SFX dan musik
- Prototipe sudah dapat dimainkan dari Chapter 1 hingga Chapter 3

**Sistem Menu dan User Interface (UI)**
Game memiliki Main Menu yang berfungsi sebagai tampilan awal sebelum permainan dimulai. Di dalam menu ini tersedia beberapa tombol utama, yaitu:
- Play untuk memulai permainan
- Settings untuk mengatur volume suara dan pengaturan dasar
- Credits untuk menampilkan informasi pengembang
- Quit untuk keluar dari game
Selain menu utama, game juga dilengkapi dengan HUD (Head-Up Display) yang menampilkan informasi health pemain, amunisi pistol, dan indikator senter. Tersedia pula Pause Menu dan tampilan Game Over ketika pemain mengalami kekalahan.
