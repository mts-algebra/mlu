# Math Level Up (MLU) — MTs Sains Algebra

Platform sertifikasi kemampuan matematika untuk siswa MTs Sains Algebra.
Siswa menuntaskan 10 level (tiap level 40 soal, waktu 1 jam, lulus jika benar
minimal 30) dan memperoleh sertifikat ber-QR yang dapat diverifikasi guru.

## Isi repo ini (situs publik)

- `index.html` — aplikasi siswa.
- `scanner.html` — aplikasi guru untuk memverifikasi keaslian sertifikat.

Pembuatan soal, penilaian, dan penandatanganan sertifikat dilakukan oleh sebuah
fungsi serverless (Cloudflare Worker) sehingga kunci jawaban tidak pernah berada
di halaman ini. Kode generator soal dan Worker disimpan terpisah, tidak di repo
publik ini.

## Konfigurasi

- `index.html`: isi `CFG.workerUrl` dengan URL Worker.
- `scanner.html`: isi `PUBLIC_KEY_JWK` dengan kunci publik.

Dipublikasikan melalui GitHub Pages.
