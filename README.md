

## Cara Penggunaan 
------------------

#### 1. Menapilkan pesan help.

   Menampilkan text help sangatlah mudah,
   cukup ketik ini di command prompt:
   ```bash
   smsid
   ```
   Atau juga bisa dengan:
   ```bash
   smsid --help
   ```
   bisa juga dengan POSIX style:
   ```bash
   smsid -h
   ```

#### 2. Mengirim pesan tunggal.


   ```bash
   smsid send [phone-number] [message]
   ```
   **[phone-number]** harus berupa angka,
   dan jumlanya harus 9 sampai dengan 13 angka, 
   harus di awali dengan 08 dan **bukan** 62
   jika nomor tidak valid akan muncul input prompt
   intuk memasukan ulang nomor.

   **[message]** harus valid, dimana character
   ("@"  "/" "\" ":"") akan dihapus otomatis (jika ada).
   jumlah character **[message]** harus lebih besar
   dari 0 dan lebih kecil dari 122.
   Jika ingin menyertakan pesan text pada parameter
   command, harus menggunakan tanda kutip pada pesan,
   agar pesan yang di kirim tidak terpotong.

   contoh:


   ```bash
   smsid send 081234567890 "Ini pesan saya"
   ```

   Bisa juga mengosongkan parameter **[message]**
   seperti:

   ```bash
   smsid send 081234557890
   ```

untuk selengkap nya tutorial nya cek di 

https://www.kumpulanremaja.com/2019/08/cara-sms-gratis-di-termux.html
#termux #sms
