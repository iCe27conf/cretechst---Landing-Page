website Cretechst.ct.ws yang dibangun menggunakan HTML, PHP, JavaScript, CSS, dan SCSS.
Fitur

    Desain responsif yang modern

    Animasi smooth menggunakan JavaScript

    Preprocessor CSS dengan SCSS

    Integrasi PHP untuk fungsionalitas dinamis

    Optimasi performa dan SEO

Prasyarat

Sebelum menginstal, pastikan Anda telah menginstal:

    Git

    Node.js dan npm (untuk build SCSS)

    PHP (versi 7.4 atau lebih baru)

    Docker (opsional, untuk instalasi dengan Docker)

Instalasi Menggunakan Console
1. Clone Repository
bash

git clone https://github.com/username/repository-name.git
cd repository-name

2. Install Dependencies
bash

# Install dependensi untuk build SCSS (jika diperlukan)
npm install

3. Build Assets (jika menggunakan SCSS)
bash

# Build SCSS ke CSS
npm run build-css

# Atau untuk watch mode selama development
npm run watch-css

4. Menjalankan Website
bash

# Jika menggunakan server PHP built-in
php -S localhost:8000

# Atau jika menggunakan Apache, pastikan file ditempatkan di directory htdocs

5. Akses Website

Buka browser dan kunjungi http://localhost:8000
Instalasi Menggunakan Docker
1. Clone Repository
bash

git clone https://github.com/username/repository-name.git
cd repository-name

2. Build Docker Image
bash

docker build -t cretechst-website .

3. Menjalankan Container
bash

docker run -d -p 8080:80 --name cretechst-site cretechst-website

4. Menggunakan Docker Compose (Alternatif)

Buat file docker-compose.yml:
yaml

version: '3'
services:
  cretechst-website:
    build: .
    ports:
      - "8080:80"
    volumes:
      - .:/var/www/html

Kemudian jalankan:
bash

docker-compose up -d

5. Akses Website

Buka browser dan kunjungi http://localhost:8080
Struktur Proyek
text

├── index.php           # Versi PHP halaman utama
├── css/                # File CSS yang telah dikompilasi
├── scss/               # File SCSS sumber
├── js/                 # File JavaScript
└── images/             # Gambar dan ikon
├── includes/          # File PHP includes
├── Dockerfile         # Konfigurasi Docker
└── package.json       # Dependencies untuk build process

Script NPM yang Tersedia

    npm run build-css : Kompilasi SCSS ke CSS

    npm run watch-css : Watch perubahan SCSS dan kompilasi otomatis

Konfigurasi

File konfigurasi utama dapat ditemukan di:

   scss/_variables.scss untuk variabel styling

  js/config.js untuk konfigurasi JavaScript

Dukungan Browser

Website ini mendukung browser modern terbaru termasuk:

    Chrome (versi terbaru)

    Firefox (versi terbaru)

    Safari (versi terbaru)

    Edge (versi terbaru)

Berkontribusi

    Fork repository

    Buat feature branch (git checkout -b feature/amazing-feature)

    Commit perubahan (git commit -m 'Add amazing feature')

    Push ke branch (git push origin feature/amazing-feature)

    Buat Pull Request

Lisensi

Proyek ini dilisensikan di bawah Lisensi MIT - lihat file LICENSE untuk detail lebih lanjut.
Dukungan

Jika Anda memiliki pertanyaan atau masalah, silakan buat issue di repository GitHub atau hubungi kami melalui email support@cretechst.ct.ws.
