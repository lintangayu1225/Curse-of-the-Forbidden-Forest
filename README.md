# Kelompok 9_Curse of the Forbidden Forest

Konsep Game
Curse of the Forbidden Forest adalah sebuah game bergenre Third-Person Survival Mystery Horror yang berfokus pada eksplorasi, survival, dan moral choices. Pemain berperan sebagai Louis, seorang mahasiswa yang kembali ke desa terpencil setelah mengetahui bahwa adiknya, Lily, menghilang di dalam hutan larangan. Game ini menargetkan pemain berusia 18 tahun ke atas, terutama mereka yang menyukai cerita gelap, suasana mencekam, dan gameplay dengan tekanan psikologis. Platform pengembangan difokuskan pada PC (Windows) menggunakan Unity Engine.

Core Mechanics dan Gameplay
Gameplay utama dirancang untuk menciptakan pengalaman yang mendalam melalui eksplorasi lingkungan, sumber daya terbatas, dan interaksi dengan dunia yang misterius. Pemain menjelajah desa, hutan, dan katedral tua menggunakan perspektif third-person, dilengkapi dengan pistol dan senter sebagai alat survival. Amunisi sangat terbatas sehingga setiap tembakan menjadi keputusan penting. Pemain dapat menemukan clue berupa objek lingkungan yang memicu dialog naratif dan membantu membuka potongan cerita.

Musuh dalam game dapat dideteksi dari suara, siluet, atau jarak tertentu. Pemain dapat memilih untuk melawan musuh dengan risiko peluru habis, atau bersembunyi di balik objek di lingkungan. Tidak ada sistem healing item, sehingga setiap encounter membawa konsekuensi serius terhadap kelangsungan permainan.

Story & Worldbuilding
Cerita dimulai ketika Louis kembali ke desa kelahirannya setelah mendengar kabar hilangnya Lily. Saat malam dan badai tiba, ia memulai penyelidikan meskipun seorang penjaga hutan mencoba menghentikannya. Saat Louis memasuki hutan Blackveil, ia menemukan tanda-tanda kehadiran anak-anak yang hilang, termasuk benda-benda kecil yang dulu milik Lily. Semakin jauh ia masuk, semakin jelas bahwa makhluk yang mengejarnya dulunya adalah anak-anak tak berdosa yang dikorbankan dalam ritual gelap oleh sosok penyihir bernama Mora.

Cerita mencapai puncaknya di reruntuhan katedral tua, tempat Mora menunggu. Pemain menentukan akhir cerita melalui tindakannya: menyelamatkan Lily dan semua anak yang hilang, atau mengakhiri kutukan dengan mengorbankan semuanya.

Visual & Audio Direction
Atmosfer game dibentuk menggunakan palet warna gelap, kabut tebal, siluet pohon tinggi, dan lingkungan yang seakan menelan cahaya. Desain karakter dan lingkungan mengadopsi estetika gothic yang mendukung tema kesepian dan keputusasaan. Audio dibuat minimalis namun intens: suara ranting patah, napas Louis, hujan, dan bisikan samar anak-anak menjadi elemen horor utama. Musik hanya muncul di momen tertentu untuk memperkuat ketegangan.

Arsitektur Teknis dan Sistem
Game dikembangkan menggunakan arsitektur Component-Based dengan kombinasi model MVC/MVP. Script ditulis menggunakan C# (.cs) dalam folder-folder modular agar mudah dikembangkan. Sistem utama meliputi pengelolaan health, AI musuh dengan state chasing, sistem inventory tetap, clue trigger, dan sistem shooting yang mendukung raycast detection. Class seperti GameManager, PlayerStateSystem, AIManager, dan NarrativeManager bertanggung jawab terhadap logika inti permainan.

Prototipe Playable
Prototipe awal telah dikembangkan dan mencakup movement system, kamera third-person, flashlight toggle, shooting mechanic, AI yang mampu mendeteksi dan mengejar pemain, clue trigger dasar, serta health system untuk musuh. Saat ini, musuh belum dapat memberikan damage kepada pemain, namun sistem combat dan pengejaran sudah dapat diuji. Tahap ini fokus pada perwujudan mekanik inti sebelum pengembangan aset final dan balancing gameplay.
