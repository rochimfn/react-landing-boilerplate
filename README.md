# `react-spa-boilerplate`

## Tentang
Boilerplate landing page dengan stack `react`, `react-router-dom`, `parcel`, `tailwindcss`, dan `purgecss`.

## Pemasangan
Boilerplate ini dibangun menggunakan runtime nodejs dan yarn package manager. Pastikan telah memasang nodejs dan yarn (atau npm) sebelum memasang. Lalu gunakan perintah berikut untuk memasang:

```bash
# Clone repository
git clone https://github.com/rochimfn/react-spa-boilerplate.git

# Pasang dependency
yarn #jika menggunakan `yarn` (disarankan)
npm install #jika menggunakan `npm`
```

## Perintah
Terdapat 3(tiga) perintah yang didaftarkan pada `package.json` yaitu `start`, `build`, dan `watch`. Untuk menjalankan perintah tersebut gunakan awalan `yarn` atau `npm run`, tergantung dengan package manager yang digunakan.

### `start`
Perintah untuk menjalankan bundler `parcel` sekaligus web server. Perintah ini tidak melakukan proses _minifying_ dan _purging_. Sangat cocok digunakan saat proses development. Tapi tidak cocok untuk production karena bundle yang dihasilkan masih berukuran besar.

```bash
yarn start
# atau
npm run start
```

### `watch`
Perintah `watch` mirip dengan `start`, melakukan bundling tanpa proses _minifying_ dan _purging_. Bedanya, `watch` tidak menjalankan web server. Sehingga perlu didampingi program web server tersendiri seperti `serve`. Perintah `watch` cocok digunakan untuk proses development  saat web server bawaan parcel tidak lagi "cukup". 

```bash
yarn watch
# atau
npm run watch
```

### `build`
Perintah `build` digunakan untuk proses deployment. Parcel akan melakukan _bundling_, _minifying_ dan _purging_.  Bundle yang dihasilakan berukuran kecil, cocok untuk production. Hasil build akan tersedia pada direktori `dist`.

```bash
yarn build
# atau
npm run build
```