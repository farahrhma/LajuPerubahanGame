# ⚔️ Laju Perubahan Battle – Kelas VII (TGT)

Game kuis kelompok: papan 50 kotak bernomor, tiap kotak berisi satu soal pilihan ganda.
Murni HTML/CSS/JavaScript, tanpa internet. Sudah disesuaikan dengan dokumen **Aturan Bermain**.

| File | Fungsi |
|------|--------|
| `index.html` | Halaman game |
| `style.css` | Tampilan |
| `script.js` | Logika permainan |
| `soal.js` | 50 soal + kunci + pembahasan + poin kategori (`pts`: 10/20/30) |

## Penerapan aturan

| Aturan | Di dalam game |
|---|---|
| 1. Pilih nomor maks 10 detik | Timer "🎯 Pilih nomor" di atas papan; habis → soal dipilih acak. Tombol **🎲 Acak** untuk memilih acak manual |
| 2. Timer per kategori; hanya ketua menjawab, final | 10 poin = 30 dtk, 20 poin = 45 dtk, 30 poin = 60 dtk (bisa dimatikan di menu).  Guru klik jawaban ketua lalu **Kunci Jawaban** |
| 3. Benar / salah / waktu habis | Benar: poin kategori + nyawa +1 (maks 3). Salah: nyawa −1, poin tetap, soal dilempar. Waktu habis: tanpa pengurangan, soal dilempar |
| 4. Angkat tangan, spin | Pada soal lemparan, klik kelompok yang angkat tangan; bila ≥2 muncul tombol **🎡 Spin** |
| 5. Lemparan 15 detik | Timer otomatis 15 detik, poin penuh. Salah → nyawa −1, dilempar lagi ke kelompok yang belum mencoba |
| 6. Soal selesai | Ada yang benar, atau **Tidak ada yang mau menjawab** → pembahasan tampil |
| 7. Nyawa 0 | Dilewati saat giliran memilih, tetap bisa ikut lemparan |
| 8. Waktu habis | Durasi permainan diatur di menu; pemenang = poin tertinggi, seri → nyawa terbanyak |
| 9–10 | Tombol **📜 Aturan** menampilkan semua aturan; guru bisa koreksi poin/nyawa dengan tombol −/+ di papan skor |

Catatan: setiap kelompok mulai dengan 3 nyawa. Bila durasi habis saat soal sedang dibuka, soal itu diselesaikan dulu,
lalu hasil akhir tampil. Tombol **⏸ Jeda** menghentikan semua timer. Permainan tersimpan otomatis di browser.

Pintasan: `A`–`D` = pilih jawaban, `Enter` = kunci / lanjut, `Esc` = tutup soal.

## Upload ke GitHub Pages
Unggah keempat file + `soal.js` ke satu folder (mis. `laju-game/`), commit, lalu aktifkan **Settings → Pages**.
