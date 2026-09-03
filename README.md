Nama : Ahmad Nurikhsan
Nim   : 2225250042

Menentukan Bilangan Habis Dibagi 3 atau Tidak

1. Deskripsi Masalah
   
Diberikan sebuah bilangan bulat nn. Tentukan apakah bilangan tersebut habis dibagi 3 atau tidak. Suatu bilangan dikatakan habis dibagi 3 apabila hasil pembagian bilangan tersebut dengan 3 memiliki sisa 0. Program akan menerima sebuah bilangan sebagai input, kemudian memeriksa sisa pembagiannya dengan 3 dan menampilkan hasil berupa “Habis dibagi 3” atau “Tidak habis dibagi 3”.

2. Identifikasi input, Proses dan output

| Komponen | Keterangan |
|---|---|
| **Input** | Bilangan bulat `n` |
| **Proses** | Menghitung sisa pembagian `n` dengan 3 menggunakan `n MOD 3`, kemudian memeriksa apakah sisanya 0 |
| **Output** | "Habis dibagi 3" atau "Tidak habis dibagi 3" |

3. Pseudocode

```text
INPUT n

IF n MOD 3 = 0 THEN
    OUTPUT "Habis dibagi 3"
ELSE
    OUTPUT "Tidak habis dibagi 3"
END IF
```
 

4. Flowchart

 Flowchart Menentukan Bilangan Habis Dibagi 3 atau Tidak

```mermaid
flowchart TD
    A([Mulai]) --> B[/Input bilangan n/]
    B --> C{Apakah n MOD 3 = 0?}
    C -->|Ya| D[/Output: "Habis dibagi 3"/]
    C -->|Tidak| E[/Output: "Tidak habis dibagi 3"/]
    D --> F([Selesai])
    E --> F
```


5. Tes Case dan Verifikasi


| No | Input | Perhitungan | Hasil yang Diharapkan |
|---:|---:|---|---|
| 1 | 12 | `12 MOD 3 = 0` | Habis dibagi 3 |
| 2 | 10 | `10 MOD 3 = 1` | Tidak habis dibagi 3 |
| 3 | 21 | `21 MOD 3 = 0` | Habis dibagi 3 |

6. Implementasi Python

```python
n = int(input("Masukkan bilangan: "))

if n % 3 == 0:
    print("Habis dibagi 3")
else:
    print("Tidak habis dibagi 3")
```


 7. Hasil Pengujian

<img width="1920" height="1080" alt="Screenshot 2026-09-02 175834" src="https://github.com/user-attachments/assets/8d02c672-2f6f-424e-b69d-077e21132e5d" />


# 🧮 Logika Matematika – Menentukan Jenis Segitiga

## 📝 Deskripsi Masalah

Dalam pembelajaran matematika SMP, siswa mempelajari materi bangun datar, salah satunya adalah segitiga. Segitiga dapat dibedakan berdasarkan panjang sisinya menjadi segitiga sama sisi, segitiga sama kaki, dan segitiga sembarang.

Program akan menerima panjang ketiga sisi sebuah segitiga sebagai input. Kemudian, program menggunakan logika kondisi untuk menentukan jenis segitiga berdasarkan kesamaan panjang sisi-sisinya.

- Jika ketiga sisi memiliki panjang yang sama → Segitiga sama sisi.
- Jika hanya dua sisi yang sama → Segitiga sama kaki.
- Jika ketiga sisinya berbeda → Segitiga sembarang.

## 📥 Input – Proses – Output

### Input

- Panjang sisi pertama
- Panjang sisi kedua
- Panjang sisi ketiga

### Proses

Program membandingkan panjang ketiga sisi menggunakan kondisi logika:

- `sisi1 == sisi2 and sisi2 == sisi3` → Segitiga sama sisi
- `sisi1 == sisi2 or sisi1 == sisi3 or sisi2 == sisi3` → Segitiga sama kaki
- Jika semua sisi berbeda → Segitiga sembarang

### Output

Jenis segitiga berdasarkan panjang sisi.

## 💻 Pseudocode

```text
INPUT sisi1
INPUT sisi2
INPUT sisi3

IF sisi1 = sisi2 AND sisi2 = sisi3 THEN
    OUTPUT "Segitiga sama sisi"
ELSE IF sisi1 = sisi2 OR sisi1 = sisi3 OR sisi2 = sisi3 THEN
    OUTPUT "Segitiga sama kaki"
ELSE
    OUTPUT "Segitiga sembarang"
END IF


