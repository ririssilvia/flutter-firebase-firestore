# flutter_firestore_firebase

A new Flutter project.

### Mendapatkan kode sampel
Kloning repositori GitHub 
```
git clone https://github.com/flutter/codelabs.git 
```
![Screenshoot firebase](images/01.png)
### Buat dan siapkan proyek Firebase
Aktifkan Cloud Firestore: Di bagian Build Firebase console, klik Cloud Firestore .
Klik Buat basis data .
![Screenshoot firebase](images/02.png)
![Screenshoot firebase](images/03.png)


### Konfigurasi Firebase
#### Konfigurasi dependensi
```
flutter pub add firebase_core 
flutter pub add firebase_auth
flutter pub add cloud_firestore
flutter pub add provider
```

#### Memasang flutterfire
```
dart pub global activate flutterfire_cli
```

#### Mengonfigurasi aplikasi Anda
```
flutterfire configure
```

### Tambahkan login pengguna (RSVP)
- Berikut adalah awal dari alur otentikasi, di mana pengguna dapat menekan tombol RSVP, untuk memulai formulir email.
![Screenshoot firebase](images/04.png)
- Setelah memasukkan email, sistem mengkonfirmasi jika pengguna sudah terdaftar, dalam hal ini pengguna dimintai kata sandi, atau jika pengguna tidak terdaftar, maka mereka pergi melalui formulir pendaftaran.
![Screenshoot firebase](images/09.png)
![Screenshoot firebase](images/10.png)
- ketika berhasil login
![Screenshoot firebase](images/11.png)

### Tulis pesan ke Cloud Firestore

- Untuk mengirim pesan pastikan sudah masuk ke akun 
![Screenshoot firebase](images/14.png)
- Coba untuk memasukkan pesan, disini saya mencoba memasukkan pesan "Hi!" 
![Screenshoot firebase](images/13.png)
![Screenshoot firebase](images/15.png)
- Pesan yang berhasil dikirimkan akan tersimpan pada cloyd firestore, seperti gambar berikut 
![Screenshoot firebase](images/12.png)

### Status RSVP Peserta
![Screenshoot firebase](images/16.png)
