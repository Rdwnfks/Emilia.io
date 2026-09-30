# Emilia Tengil Batu — PWA + Login

Paket ini siap ditempatkan di **root** repository `Rdwnfks/faksi.github.io` untuk GitHub Pages.

## Isi
- PWA installable untuk iPhone/iPad, Android, Windows, macOS, dan browser desktop yang mendukung PWA.
- Login/register email + password menggunakan Supabase.
- Data aplikasi tersimpan per akun di Supabase dan memiliki cache lokal untuk penggunaan offline.
- Service worker + manifest + ikon sudah disiapkan.

## Sebelum upload
1. Buat project di Supabase.
2. Jalankan isi `supabase.sql` di Supabase → SQL Editor.
3. Buka `supabase-config.js`.
4. Isi `SUPABASE_URL` dan `SUPABASE_ANON_KEY` menggunakan Project URL dan anon/public key dari Supabase.
5. **Jangan** memasukkan `service_role` key ke file ini.

## Upload ke GitHub Pages
Upload isi folder ini langsung ke **root** repository `faksi.github.io`, sehingga `index.html` berada di root repository.

Di GitHub:
- Settings → Pages
- Build and deployment → Source: Deploy from a branch
- Branch: `main`
- Folder: `/ (root)`
- Save

Setelah aktif, situs user repository biasanya berada di `https://rdwnfks.github.io/`.

## Install di iPhone
1. Buka URL situs menggunakan **Safari**.
2. Tekan Share.
3. Pilih **Add to Home Screen**.
4. Buka aplikasi dari ikon Home Screen.

## Install di Android
1. Buka URL di Chrome.
2. Pilih **Install app / Add to Home screen** jika muncul.

## PC
Buka URL di Chrome/Edge dan pilih opsi **Install** pada browser jika tersedia.

## Penting
- GitHub Pages hanya menjadi hosting file statis; login dan sinkronisasi akun dilakukan oleh Supabase.
- Untuk login dan sinkronisasi lintas perangkat, perangkat harus online saat melakukan autentikasi/sinkronisasi.
- Data yang sudah tersimpan di cache lokal masih dapat ditampilkan ketika offline pada perangkat tersebut.
