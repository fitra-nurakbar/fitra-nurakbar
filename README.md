## Development Setup
### Prerequisites
- Pertama, pastikan kalian sudah punya [PHP](https://php.net).
- Kedua, mempunyai [nodejs](https://nodejs.org) beserta [Node Package Manager](https://www.npmjs.com/get-npm) atau [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/)
- Ketiga, jangan lupa kalian sudah terinstall juga [Composer](https://getcomposer.org)
- Terakhir, pastikan kalian juga sudah punya database relasional seperti [MySQL](https://www.mysql.com/downloads/), [PostgreSQL](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) atau [SQLite](https://www.sqlite.com/download.html)

### Setting Up Project

Silahkan fork terlebih dahulu repository ini, kemudian clone repository yang udah kalian fork ya (Inget repository yang kalian fork, bukan repository ini). 
Bisa gunakan command berikut:
```bash
git clone git@github.com:{username github kalian}/laract9.git
# atau kalo kalian pake https (bukan ssh)
git clone https://github.com/{username github kalian}/laract9.git
```
Kemudian, buka terminal seperti bash, zsh, command prompt atau powershell dan nstall dependency composer dengan command berikut
```bash
composer install && composer update
```
Lanjut, copy file `.env.example` dengan nama `.env` sebagai berikut:
```bash
cp .env.example .env
```
Kemudian, silahkan ganti credentials database di file .env nya seperti
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=xxx
DB_USERNAME=root
DB_PASSWORD=
```
untuk panduan atau dokumentasi mengenai setup database pada file `.env` bisa kalian baca pada dokumentasi resmi laravelnya ya cui, [klik disini.](https://laravel.com/docs/9.x/database)

Kemudian, silahkan migrate semua database di project ini dengan menggunakan artisan command:
```bash
php artisan migrate
```
Lanjut, generate aplikasi key untuk keamanan pada project laravel dengan menggunakan artisan command berikut:
```bash
php artisan key:generate
# atau 
php artisan key:generate --show
```
Install dependencies nodejs didalam folder `node_modules` menggunakan Npm atau Yarn:
```bash
npm install && npm run dev
# atau menggunakan Yarn
yarn && yarn dev
# atau menggunakan pnpm
pnpm i && pnpm dev
```
Langkah Terakhir, silahkan jalankan local development server Laravel dengan menggunakan artisan command sebagai berikut:
```bash
php artisan serve
```
```bash
Project ini akan berjalan di `https://localhost:8080`.
[stackshare](https://stackshare.io/fitra-nurakbar)
[DEV](https://dev.to/fitranurakbar)
[Medium](https://medium.com/@fitranurakbar)
```
