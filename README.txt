NAMM MONEY (PWA)

Isi:
  index.html            -> aplikasi
  manifest.webmanifest  -> nama app, ikon, warna
  sw.js                 -> service worker (bisa dipakai offline)
  icons/                -> logo (192, 512, maskable, apple-touch, favicon)

CARA PAKAI
PWA harus dibuka lewat HTTPS (tidak jalan kalau cuma klik file index.html).
Upload SEMUA isi folder ini ke root hosting, misalnya:
  - GitHub Pages (repo -> Settings -> Pages -> Deploy from branch -> main / root)
  - Netlify / Cloudflare Pages (drag & drop folder)

Lalu buka URL-nya di Chrome HP -> menu ⋮ -> "Instal aplikasi" / "Tambahkan ke layar utama".

Catatan:
  - Data tersimpan di browser/app (localStorage, kunci "catuang"), jadi data lama
    di URL yang sama tetap aman. Beda alamat hosting = data terpisah -> pakai Ekspor/Impor.
  - Kalau update file, ubah CACHE = 'namm-money-v1' di sw.js jadi v2, v3, dst.
