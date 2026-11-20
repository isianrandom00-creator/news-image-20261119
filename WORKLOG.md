# WORKLOG — `news-image-20261119`

## Ringkasan bounty

Bounty Make.fun meminta satu gambar yang merangkum berita dunia pada Kamis, 19 November 2026. Program entry harus berada di root repo sebagai `main.ts` untuk Node 22 dan menulis `/output/entry.png`. Gambar harus PNG/JPEG dengan nama `entry.png`, maksimal 1024×1024 piksel dan 1 MiB; program harus deterministik, tanpa jaringan, dan berjalan dalam batas sandbox bounty. Deadline yang tercatat dalam percakapan adalah Sabtu, 21 November 2026 pukul 07.00 WIB.

## Prompt dan keputusan penting

- Firt meminta entry dibuat untuk bounty `news-image-20261119`, memakai Cue saja dan tidak memakai LLM, akun, atau sesi di luar Cue.
- Entry dimaksudkan orisinal, faktual, mencakup beberapa kawasan, dan terbaca pada lebar sekitar 300 px. Warden diminta meninjau akurasi, cakupan, hierarki visual, dan keterbacaan setelah build, maksimal dua putaran.
- Transcript bounty harus memakai bundle biasa, bukan `record`.
- Jangan membaca atau menyalin starter/kode lama. Jangan mulai menulis kode sebelum `bundle --dry-run` menemukan log sesi Cue asli. Jangan membuat atau mengubah transcript.
- Jangan menandatangani atau mengirim submission; keputusan submit milik Firt.
- Repo GitHub publik baru dibuat setelah bounty dibuka.

## Langkah yang sudah dilakukan

1. Membaca petunjuk Make.fun, halaman/requirements bounty, aturan, leaderboard dan entry teratas yang disebut dalam percakapan sebelumnya.
2. Mengunduh kit resmi dan memeriksa `RULES.txt` serta CLI kit; hash CLI dibandingkan dengan manifest kit.
3. Membuat repo GitHub publik `isianrandom00-creator/news-image-20261119` dan menyiapkan repo lokal di `/workspace/bounty-work/news-image-20261119`.
4. Menjalankan `bundle --dry-run` beberapa kali. CLI tidak menemukan sesi di folder lokal Cue yang dicari Make.fun, `~/.cue/agents/*/sessions`.
5. Atas permintaan Firt, membuat `WORKLOG.md` berdasarkan percakapan yang tersedia. Ini catatan kerja, bukan log sesi atau pengganti transcript asli.
6. Membuat commit lokal `375d40d` (`Add bounty worklog`). Percobaan push pertama melalui shell Git biasa gagal karena shell tersebut tidak memiliki kredensial GitHub untuk autentikasi non-interaktif.

## Ketentuan transcript yang ditemukan

`RULES.txt` bagian “Transcripts” dan “Transcript gate” (baris 83–98), serta bagian “Before you submit” (baris 181–199), meminta transcript sesi AI coding-agent yang membangun entry. Bundle biasa mencari sesi harness yang tersimpan; `--dry-run` hanya melaporkan file yang ditemukan. Aturan melarang menulis ulang, membangun ulang, atau merangkum sesi dari ingatan sebagai transcript. Jika harness memang tidak menyimpan sesi yang bisa diunggah, aturan mengizinkan sesi handed-over dalam format JSON, dengan alasan satu baris dan hanya timestamp/usage yang memang terlihat. Requirements bounty menyatakan entry handed-over tetap dapat dinilai tetapi tidak berhak menerima hadiah.

Karena itu, WORKLOG ini tidak menggantikan sesi asli dan bukan transcript handed-over. Copy-paste teks chat ke berkas juga belum otomatis memenuhi syarat rekaman harness, usage, run record, dan gerbang transcript.

## Hasil saat catatan ini dibuat

- Repo lokal berisi catatan kerja ini saja; `main.ts` dan gambar entry belum dibuat.
- Nama output yang diwajibkan nantinya adalah `/output/entry.png`; file itu belum dihasilkan.
- Belum ada build, pengujian determinisme, pemeriksaan akhir kit, ulasan Warden, atau submission. Isi repo yang dikerjakan di sini adalah catatan kerja; entry bounty belum dibuat.
- `bundle --dry-run` belum menemukan log sesi lokal. Ini hanya menggambarkan folder yang diperiksa pada komputer kerja, bukan bukti bahwa riwayat chat Cue Android hilang atau disalahgunakan.
- Repo GitHub: https://github.com/isianrandom00-creator/news-image-20261119
