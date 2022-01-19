Tajuk Pertama | Tajuk Kedua
--- | ---
Sel Konten | Sel Konten
Sel Konten | Sel Konten

Tajuk Pertama | Tajuk Kedua
--- | ---
Sel Konten | Sel Konten
Sel Konten | Sel Konten

![Benteng](https://vignette.wikia.nocookie.net/masseffect/images/d/d7/MassEffect2Citadel.jpg/revision/latest?cb=20100721191415)

Rata Kiri | Rata tengah | Rata Kanan
:-- | :-: | --:
kolom 3 adalah | beberapa teks bertele-tele | **$1600**
kolom 2 adalah | terpusat | $12
garis-garis zebra | rapi | ~~$1~~

Dillinger adalah editor HTML5 Markdown yang didukung oleh cloud, siap untuk seluler, penyimpanan offline, AngularJS.

- Ketik beberapa penurunan harga di sebelah kiri
- Lihat HTML di sebelah kanan
- Sihir

# benar

- Impor file HTML dan saksikan secara ajaib dikonversi ke penurunan harga
- Seret dan lepas gambar (mengharuskan akun Dropbox Anda ditautkan)

Anda juga bisa:

- Impor dan simpan file dari GitHub, Dropbox, Google Drive, dan One Drive
- Seret dan jatuhkan penurunan harga dan file HTML ke Dillinger
- Ekspor dokumen sebagai Penurunan harga, HTML, dan PDF

Markdown adalah bahasa markup yang ringan berdasarkan konvensi pemformatan yang biasanya digunakan orang dalam email. Seperti yang ditulis [John Gruber] di [situs penurunan harga][df1]

> Tujuan desain utama untuk sintaks pemformatan Markdown adalah membuatnya semudah mungkin dibaca. Idenya adalah bahwa dokumen berformat penurunan harga harus dapat diterbitkan apa adanya, sebagai teks biasa, tanpa terlihat seperti telah ditandai dengan tag atau instruksi pemformatan.

Teks yang Anda lihat di sini *sebenarnya* ditulis dalam penurunan harga! Untuk merasakan sintaks Markdown, ketik beberapa teks ke jendela kiri dan lihat hasilnya di kanan.

### Salah

Dillinger menggunakan sejumlah proyek sumber terbuka untuk bekerja dengan baik:

- [AngularJS] - HTML ditingkatkan untuk aplikasi web!
- [Ace Editor] - editor teks berbasis web yang mengagumkan
- [markdown-it] - Pengurai penurunan harga dilakukan dengan benar. Cepat dan mudah untuk diperpanjang.
- [Twitter Bootstrap] - boilerplate UI yang bagus untuk aplikasi web modern
- [node.js] - event I/O untuk backend
- [Ekspres] - kerangka aplikasi jaringan node.js cepat [@tjholowaychuk]
- [Gulp] - sistem pembuatan streaming
- [Breakdance](https://breakdance.github.io/breakdance/) - Pengonversi HTML ke Penurunan Harga
- [jQuery] - duh

Dan tentu saja Dillinger sendiri adalah open source dengan [repositori publik][dill] di GitHub.

### Instalasi

![Ilos](https://lh3.googleusercontent.com/proxy/DDV8a7sLIWurhJtW8Ego9bq-JlwpfFFoR0tkLJQKKYXEXoWHB6ZUP5jGKD2VcYt3z1QVsgcn6L3GoU1ns8m9fvi3U51GzddA70ZUMHgzHvjl4-i7YOJY9cShBPrfjUhMQhxaJ97WFBp612XmjMXVGypfGkiBarN4PWxhiHkiYYNW7HGbtTpOcyt9GQ4Q23C2noxLTWFXZMcQZhRpQA_qzu2n6_H6CPViBnhSHpEl4JZAPaGCSJqgZg)

Dillinger membutuhkan [Node.js](https://nodejs.org/) v4+ untuk dijalankan.

Instal dependensi dan devDependencies dan mulai server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

Untuk lingkungan produksi...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugin

Dillinger saat ini diperluas dengan plugin berikut. Petunjuk tentang cara menggunakannya dalam aplikasi Anda sendiri ditautkan di bawah.

plugin | Baca aku
--- | ---
Dropbox | [plugins/dropbox/README.md][PlDb]
GitHub | [plugins/github/README.md][PlGh]
google Drive | [plugins/googledrive/README.md][PlGd]
OneDrive | [plugins/onedrive/README.md][PlOd]
Sedang | [plugins/medium/README.md][PlMe]
Google Analytics | [plugins/googleanalytics/README.md][PlGa]

### Perkembangan

Ingin berkontribusi? Besar!

Dillinger menggunakan Gulp + Webpack untuk pengembangan cepat. Buat perubahan pada file Anda dan lihat pembaruan Anda secara instan!

Buka Terminal favorit Anda dan jalankan perintah ini.

Tab Pertama:

```sh
$ node app
```

Tab Kedua:

```sh
$ gulp watch
```

(opsional) Ketiga:

```sh
$ karma test
```

#### Bangunan untuk sumber

Untuk rilis produksi:

```sh
$ gulp build --prod
```

Menghasilkan arsip zip yang dibuat sebelumnya untuk distribusi:

```sh
$ gulp build dist --prod
```

### Buruh pelabuhan

Dillinger sangat mudah dipasang dan disebarkan dalam wadah Docker.

Secara default, Docker akan mengekspos port 8080, jadi ubah ini di dalam Dockerfile jika perlu. Jika sudah siap, cukup gunakan Dockerfile untuk membuat image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```

Ini akan membuat gambar dillinger dan menarik dependensi yang diperlukan. Pastikan untuk menukar `${package.json.version}` dengan versi Dillinger yang sebenarnya.

Setelah selesai, jalankan gambar Docker dan petakan port ke apa pun yang Anda inginkan di host Anda. Dalam contoh ini, kita cukup memetakan port 8000 dari host ke port 8080 dari Docker (atau port apa pun yang terbuka di Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verifikasi penerapan dengan menavigasi ke alamat server Anda di browser pilihan Anda.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

Lihat [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

### Todo

Untuk melakukannya, pertama-tama <strong>ubah</strong> <code>type</code> <a href="../../../../documentation/components/reference/amp-carousel.md"><code>amp-carousel</code></a> dari <code>carousel</code> ke <code>slides</code> , <strong>ubah</strong> <code>layout</code> menjadi <code>responsive</code> dan <strong>atur</strong> <code>width</code> menjadi 300 (pastikan <code>height</code> dan <code>width</code> sudah ditentukan). <strong>Tambahkan</strong> atribut <code>"layout=responsive"</code> ke <a href="../../../../documentation/components/reference/amp-img.md"><code>amp-img</code></a> dari <a href="../../../../documentation/components/reference/amp-carousel.md"><code>amp-carousel</code></a>
