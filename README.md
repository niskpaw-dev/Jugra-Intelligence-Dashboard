🏫 SMK Jugra Intelligence Dashboard (JID)

SMK Jugra Intelligence Dashboard (JID) adalah sebuah sistem berkonsepkan Public-Facing Dashboard berasaskan Google Apps Script (GAS) dan Google Sheets. Ia direka khusus untuk pengurusan evidens kepimpinan sekolah selaras dengan standard SKPM (1.1 hingga 1.6).

Sistem ini membolehkan pelawat awam melihat statistik dan senarai dokumen (bertaraf umum) tanpa perlu log masuk, manakala Pengetua atau Pentadbir mempunyai akses pintu belakang yang selamat (secure backend) untuk mengemas kini data.

✨ Ciri-Ciri Utama (Features)

Papan Pemuka Awam & Selamat: Pemisahan antara paparan pelawat awam (Tatapan Umum) dan paparan sulit berpandukan Role-Based Access Control (RBAC).

Pengurusan Standard Kepimpinan: Pengkategorian evidens mengikut 6 standard utama:

1.1 Hala Tuju Sekolah

1.2 Pengurusan Organisasi

1.3 Kepimpinan Instruksional

1.4 Pengurusan Perubahan dan Inovasi

1.5 Jaringan dan Jalinan

1.6 Kepimpinan Berintegriti

UI/UX Futuristik (Glassmorphism): Reka bentuk Baby Blue berkonsepkan kaca separa lutsinar dengan kesan animasi scroll dan particle effects menggunakan kanvas HTML5.

Responsif Sepenuhnya: Dioptimumkan untuk penggunaan di telefon pintar, tablet (iPad), dan komputer meja (Desktop).

Pengkalan Data Percuma: Menggunakan Google Sheets sebagai pangkalan data utama tanpa sebarang kos pelayan (server-less).

🛠️ Panduan Instalasi (Deployment)

Sistem ini sangat mudah untuk dipasang. Hanya perlukan akaun Google (Gmail/Workspace/MOE).

1. Persediaan Pangkalan Data (Google Sheets)

Buat satu fail Google Sheets baharu di Google Drive anda.

Namakan fail tersebut Database JID.

Klik menu Extensions > Apps Script.

2. Memasukkan Kod

Di dalam paparan Apps Script, anda akan melihat fail Code.gs. Padam semua kod di dalamnya dan salin kandungan dari fail Code.gs dari repositori ini.

Tambah satu fail HTML baharu dengan klik ikon (+) dan pilih HTML. Namakannya sebagai Index (huruf I besar, tanpa .html).

Salin keseluruhan kandungan dari fail Index.html repositori ini dan tampal ke dalamnya.

Klik Save (Ikon Disket).

3. Menjana Pangkalan Data Secara Automatik

Di dalam fail Code.gs, lihat pada bar alat bahagian atas (dropdown menu bersebelahan butang "Run").

Tukar pilihan dari doGet kepada setupDatabase.

Klik Run. (Google akan meminta kebenaran/akses. Klik 'Review Permissions' > Pilih Akaun > Klik 'Advanced' > Go to Untitled Project).

Setelah selesai, semak semula Google Sheets anda. Tiga (3) helaian (sheets) iaitu Dokumen, Users, dan AuditLog akan dijana secara automatik dengan tema warna biru.

4. Terbitkan ke Web (Deploy)

Klik butang biru Deploy di bucu atas kanan > Pilih New deployment.

Klik ikon gear (⚙️) dan pastikan Web app ditanda.

Tetapkan:

Execute as: Me (emelanda@gmail.com)

Who has access: Anyone (Penting supaya pelawat awam dapat melihat papan pemuka)

Klik Deploy dan salin pautan Web app URL yang diberikan. Selesai!

🔐 Maklumat Log Masuk Lalai (Default Credentials)

Untuk log masuk sebagai Pentadbir bagi mula memasukkan data, skrol ke bahagian paling bawah sidebar sebelah kiri dan klik Akses Pentadbir.

ID Pengguna: admin

Kata Laluan: Admin@2026

(Sila tukar kata laluan ini atau tambah akaun baharu melalui menu "Senarai Pengguna" selepas log masuk).

👨‍💻 Penghargaan & Pembangun

Dibina dan dijana oleh Niskala Pawaka Dev

Sila bintang (⭐) repositori ini jika ia bermanfaat untuk sekolah anda!
