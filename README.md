# Tugas-TIK-Mengajar
## Ragil Ayu Palupi 
## Kelompok 6
## TI-1B

Prompt engineering: cara "ngomong" ke AI

Bayangkan kamu pesan makanan. Kalau cuma bilang "satu makanan", kamu dapat apa saja. Kalau bilang "nasi goreng pedas, tanpa telur, bungkus", kamu dapat yang kamu mau. AI juga begitu: makin jelas instruksimu, makin pas hasilnya.

Instruksi yang jelas biasanya punya empat bagian:
- Role: kamu ingin AI berperan sebagai siapa (misalnya guru atau desainer).
- Task: apa yang harus dikerjakan.
- Context: latar belakang, supaya AI paham situasinya.
- Format: hasilnya dalam bentuk apa (daftar, esai 500 kata, dan sebagainya).

Contoh: bukan "jelaskan komputasi kuantum", tapi "jelaskan komputasi kuantum dengan bahasa sederhana untuk orang yang bukan dari bidang teknik, maksimal 3 paragraf".

Git: buku catatan perubahan untuk filemu

Pernah punya file bernama "tugas_final", "tugas_final_revisi", "tugas_final_revisi_beneran"? Git menyelesaikan itu. Git mencatat siapa mengubah apa dan kapan, jadi kamu bisa kembali ke versi lama kapan saja tanpa menyimpan banyak salinan file.

GitHub: Google Drive-nya Git

Git bekerja di komputermu sendiri. GitHub adalah situs tempat menyimpan hasil kerja Git itu secara online, supaya aman dan bisa dikerjakan bersama orang lain. Singkatnya: Git itu alatnya, GitHub itu tempat penyimpanannya.

Tiga tempat di dalam Git

Analoginya mengemas barang untuk dikirim:
1. Working directory: meja kerjamu, tempat kamu mengedit file.
2. Staging area: kardus tempat kamu memilih barang apa yang mau dikirim.
3. Git directory: gudang tempat semua versi disimpan permanen.

Perintah-perintah dasar

- `git init`: mulai melacak sebuah folder.
- `git add .`: masukkan semua perubahan ke "kardus".
- `git commit -m "pesan"`: tutup kardus dan simpan sebagai satu versi, dengan catatan singkat tentang apa yang berubah.
- `git remote add origin <alamat>`: beri tahu Git alamat GitHub-mu.
- `git push origin main`: kirim hasilnya ke GitHub.
- `git pull origin main`: ambil perubahan terbaru dari GitHub ke komputermu.

Persiapan sebelum mulai

Instal Git dan VS Code (editor untuk menulis kode). Lalu beri tahu Git namamu dan emailmu, supaya setiap perubahan ada nama pemiliknya.

SSH key: kunci pintu ke GitHub

Tanpa SSH, GitHub akan meminta password terus-menerus. Dengan SSH, kamu membuat sepasang kunci: satu kunci publik yang kamu titipkan ke GitHub (seperti gembok), dan satu kunci pribadi yang tetap di komputermu (seperti anak kuncinya). Begitu cocok, GitHub langsung percaya itu kamu. Jenis kunci yang dipakai namanya Ed25519, yang aman dan cepat. Setelah dipasang, tes dengan `ssh -T git@github.com`; kalau muncul pesan "successfully authenticated", berarti berhasil.

Latihan: Student Task Planner

Ini gabungan semuanya, yaitu membuat aplikasi pencatat tugas mahasiswa:
1. Buka AI (Claude, ChatGPT, atau Antigravity).
2. Minta AI membuatkan aplikasinya dengan prompt yang jelas.
3. Di folder proyek, jalankan `git init`.
4. Commit dan push ke GitHub.
5. Ubah atau tambah sesuatu di aplikasinya.
6. Commit dan push lagi.

Setelah dua kali push, di GitHub kamu bisa melihat dua versi tersimpan. Itulah yang disebut *version control*.

Intinya

Tulis prompt yang jelas supaya AI memberi hasil yang bagus, lalu simpan hasil kerjamu dengan Git, dan taruh di GitHub supaya aman dan bisa dikerjakan bersama.
