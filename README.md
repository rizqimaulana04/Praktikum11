# Praktikum11
# **Exception-Handling**

Python Exception handling adalah suatu mekanisme penanganan flow normal program karena terjadi exception dengan melanjutkan flow ke code block lainnya.
<br>                                            |

**Kenapa harus menangani exception?**

- Karena terjadi exception dan kita tidak tangani, maka program akan berhenti.

- Object exception mengandung informasi dimana dan kenapa exception terjadi. Jadi kita dapat melakukan tindakan tepat agar program tetap berjalan semestinya.

## **raise.py**

Untuk melempar pengecualian, gunakan kata kunci raise.

```sh
raise #Exception("# pesan eror")
```

## **tryexeception.py**

```sh
try:
       # kode yang ingin di tangani....

except:
       # blok opsional
       # Penanganan

```

- Try: Blok ini akan menguji kesalahan yang dikecualikan terjadi
- except: Di ​​sini Anda dapat menangani kesalahan

## **exceptionfull.py**

- Try: Blok ini akan menguji kesalahan yang dikecualikan terjadi
- except: Di ​​sini Anda dapat menangani kesalahan
- else: Jika tidak ada pengecualian maka blok ini akan dieksekusi
- finally:blok selalu dieksekusi baik pengecualian dihasilkan atau tidak

```sh
try:
       # kode yang di tangani....

except:
       # blok opsional
       # Penanganan (if di perlukan)

else:
       # jalankan if tidak ada exception

finally:
      # kode yang di tangani .....(selalu dieksekusi)
```

## **Standard Exceptions**

| Nama                | Penjelasan                                                                                                                                                 |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Exception           | Kelas dasar untuk semua pengecualian / exception                                                                                                           |
| StopIteration       | Dibesarkan ketika metode (iterator) berikutnya dari iterator tidak mengarah ke objek apa pun.                                                              |
| SystemExit          | Dibesarkan oleh fungsi sys.exit ().                                                                                                                        |
| StandardError       | Kelas dasar untuk semua pengecualian built-in kecuali StopIteration dan SystemExit.                                                                        |
| ArithmeticError     | Kelas dasar untuk semua kesalahan yang terjadi untuk perhitungan numerik.                                                                                  |
| OverflowError       | Dibesarkan saat perhitungan melebihi batas maksimum untuk tipe numerik.                                                                                    |
| FloatingPointError  | Dibesarkan saat perhitungan floating point gagal.                                                                                                          |
| ZeroDivisonError    | Dibesarkan saat pembagian atau modulo nol dilakukan untuk semua tipe numerik.                                                                              |
| AssertionError      | Dibesarkan jika terjadi kegagalan pernyataan Assert.                                                                                                       |
| AttributeError      | Dibesarkan jika terjadi kegagalan referensi atribut atau penugasan.                                                                                        |
| EOFError            | Dibesarkan bila tidak ada input dari fungsi raw_input () atau input () dan akhir file tercapai.                                                            |
| ImportError         | Dibesarkan saat sebuah pernyataan impor gagal.                                                                                                             |
| KeyboardInterrupt   | Dibesarkan saat pengguna menyela eksekusi program, biasanya dengan menekan Ctrl + c.                                                                       |
| LookupError         | Kelas dasar untuk semua kesalahan pencarian.                                                                                                               |
| IndexError          | Dibesarkan saat sebuah indeks tidak ditemukan secara berurutan.                                                                                            |
| KeyError            | Dibesarkan saat kunci yang ditentukan tidak ditemukan dalam kamus.                                                                                         |
| NameError           | Dibesarkan saat pengenal tidak ditemukan di namespace lokal atau global.                                                                                   |
| UnboundLocalError   | Dibesarkan saat mencoba mengakses variabel lokal dalam suatu fungsi atau metode namun tidak ada nilai yang ditugaskan padanya.                             |
| EnvironmentError    | Kelas dasar untuk semua pengecualian yang terjadi di luar lingkungan Python.                                                                               |
| IOError             | Dibesarkan saat operasi input / output gagal, seperti pernyataan cetak atau fungsi open () saat mencoba membuka file yang tidak ada.                       |
| OSError             | Dibangkitkan untuk kesalahan terkait sistem operasi.                                                                                                       |
| SyntaxError         | Dibesarkan saat ada kesalahan dengan sintaks Python.                                                                                                       |
| IndentationError    | Dibesarkan saat indentasi tidak ditentukan dengan benar.                                                                                                   |
| SystemError         | Dibesarkan saat penafsir menemukan masalah internal, namun bila kesalahan ini ditemui juru bahasa Python tidak keluar.                                     |
| SystemExit          | Dibesarkan saat juru bahasa Python berhenti dengan menggunakan fungsi sys.exit (). Jika tidak ditangani dalam kode, menyebabkan penafsir untuk keluar.     |
| TypeError           | Dibesarkan saat operasi atau fungsi dicoba yang tidak valid untuk tipe data yang ditentukan.                                                               |
| ValueError          | Dibesarkan ketika fungsi bawaan untuk tipe data memiliki jenis argumen yang valid, namun argumen tersebut memiliki nilai yang tidak valid yang ditentukan. |
| RuntimeError        | Dibesarkan saat kesalahan yang dihasilkan tidak termasuk dalam kategori apa pun.                                                                           |
| NotImplementedError | Dibesarkan ketika metode abstrak yang perlu diimplementasikan di kelas warisan sebenarnya tidak dilaksanakan.  