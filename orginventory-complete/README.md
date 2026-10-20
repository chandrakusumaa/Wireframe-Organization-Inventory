# OrgInventory — Frontend Prototype

Paket ini adalah prototipe frontend HTML/CSS/JavaScript berdasarkan alur OrgInventory yang dibahas. Halaman sudah dipisah supaya mudah dibuka dan diedit.

## Cara menjalankan

1. Ekstrak folder `orginventory-complete`.
2. Cara paling praktis: buka folder di VS Code, lalu jalankan `index.html` dengan ekstensi **Live Server**. Alternatifnya, jalankan server lokal dari folder tersebut: `python -m http.server 8000`, kemudian buka `http://localhost:8000`.
3. Klik **Masuk** dan gunakan akun demo berikut:
   - Email: `demo@orginventory.id`
   - Password: `demo123`
4. Untuk mencoba sebagai pengguna baru, pilih **Daftar**. Setelah terdaftar, buat organisasi dari menu **Organisasiku**.

## Halaman yang tersedia

- Publik: Landing Page, Explore Organizations, halaman organisasi, detail aset.
- Akun: Login, Register, Forgot Password, Beranda Pengguna, Organisasiku, Buat Organisasi, Peminjamanku, Notifikasi, Profil.
- Workspace: Dashboard, Inventory, form tambah/edit aset, Peminjaman, detail peminjaman, Laporan Kerusakan, Maintenance, Kategori, Lokasi, Anggota, Laporan, Pengaturan.

## Fitur demo yang aktif

- Akun demo dan registrasi lokal.
- Membuat organisasi; pembuat otomatis menjadi OWNER.
- Mengganti organisasi aktif dan melihat data tiap workspace.
- Tambah/edit/hapus aset; tambah/hapus kategori dan lokasi; serta pengaturan organisasi.
- Pengajuan peminjaman dari halaman aset, persetujuan/penolakan, dan pencatatan pengembalian.
- Laporan kerusakan dan jadwal maintenance.
- Ekspor daftar inventaris ke CSV dan cetak laporan.
- Filter pencarian untuk organisasi, inventaris, dan peminjaman.
- Data disimpan di `localStorage` browser. Gunakan tombol **Reset seluruh data demo** pada halaman Profil untuk mengembalikan data awal.

## Batasan penting

Ini belum merupakan aplikasi produksi. Tidak ada backend, database server, email reset password, email undangan, upload file, sesi aman, atau otorisasi server. Password demo disimpan lokal hanya untuk simulasi; jangan pakai password sungguhan. Dalam aplikasi sebenarnya, otentikasi, izin per organisasi/role, validasi ketersediaan aset, dan transaksi peminjaman harus dilakukan serta diverifikasi di backend.

## Struktur

- `*.html` — halaman-halaman yang dapat diedit.
- `style.css` — gaya visual responsif.
- `app.js` — renderer halaman, interaksi, dan penyimpanan data demo.
