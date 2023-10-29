# lab5web
# Nama : Muhammad Din Al Ayubi
# Kelas : TI 22 A3
# NIM : 312210293

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama ```lab5_javascript```.
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org
## Langkah-langkah Praktikum
* Persiapan membuat dokumen HTML dengan nama file ```lab5_javascript.html```seperti berikut.
```python
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mengenal JavaScript</title>
</head>
<body>
    
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>

</body>
</html>
```
* Hasil Output
![gambar](tugas5/1.png)
## Javascript Dasar
* Pemakaian ```Alert``` sebagai property window.
```python
<html>
    <head>
        <title>alert box</title>
    </head>
    <body>
        <script language = "javascript">
        <!--
            window.alert("ini merupakan pesan untuk anda");
            //-->
        </script>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/2.png)
* Pemakaian ```method``` dalam objek.
```python
<html>
    <head>
        <title>skrip javascript</title>
    </head>
    <body>
        percobaan memakai javascript:<br>
        <script language = "javascript">
            <!--
                document.write("selamat mencoba javascript<br>");
                document.write("semoga sukses!");
                //-->
        </script>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/3.png)
* Pemakaian ```Prompt```
```python
<html>
    <head>
        <title>pemasukan data</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nama = prompt("siapa nama anda?","masukkan nama anda");
                document.write("hai, "+ nama);
                //-->
        </script>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/4.png)
![gambar](tugas5/5.png)
* Pembuatan ```fungsi``` dan cara pemanggilannya
```python
<html>
    <head>
        <title>contoh program javascript</title>
        <script language="javascript">
            function pesan(){
                alert ("memanggil javascript lewat body onload")
            }
        </script>
    </head>
    <body onload="pesan"()>
    </body>
</html>
```
## Dasar Pemrograman Di Javascript
* Operasi dasar ```aritmatika```
```python
<html>
    <head>
        <title>contoh program javascript</title>
        <script language="javascript">
            function test (val1,val2)
            {
                document.write("<br>"+"perkalian : val1*val2 "+"<br>")
                document.write(val1*val2)
                document.write("<br>"+"pembagian : val1/val2 "+"<br>")
                document.write(val1/val2)
                document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
                document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
                document.write(val1-val2)
                document.write("<br>"+"modulus : val1%val2 "+"<br>")
                document.write(val1%val2)
            }
        </script>
    </head>
    <body>
        <h3>contoh program javascript</h3>
        <input type="button" name="button1" value="aritmetic" onclick=test(9,4)>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/6.png)
* Seleksi ```kondisi``` (if..else)
```python
<html>
    <head>
        <title>contoh if-else</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nilai = prompt("nilai (0-100): ",0);
                var hasil = "";
                if (nilai >= 60)
                hasil = "lulus";
                else
                hasil = "tidak lulus";
                document.write("hasil: " + hasil);
                //-->
        </script>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/7.png)
![gambar](tugas5/8.png)
![gambar](tugas5/9.png)
![gambar](tugas5/10.png)
* Penggunaan ```operator switch``` untuk seleksi kondisi
```python
<html>
    <head>
        <title>contoh program javascript</title>
        
        <script language="javascript">
            function test ()
            {
                val1=window.prompt("input nilai (1-5):")
                switch (val1)
                {
                case "1" :
                    document.write("bilangan satu")
                    break
                case "2" :
                    document.write("bilangan dua")
                    break
                case "3" :
                    document.write("bilangan tiga")
                    break
                case "4" :
                    document.write("bilangan empat")
                    break
                case "5" :
                    document.write("bilangan lima")
                    break
                default :
                    document.write("bilangan lainnya")
            }
        }
        </script>
    </head>
    <body>
        <h3>contoh program javascript</h3>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/11.png)
![gambar](tugas5/12.png)
![gambar](tugas5/13.png)
![gambar](tugas5/14.png)
## Pembuatan Form
* Form ```Input```
```python
<html>
    <head>
        <script language="javascript">
            function test () {
                var val1=document.kirim.T1.value
                if (val1%2==0)
                    document.kirim.T2.value="bilangan genap"
                else
                    document.kirim.T2.value="bilangan ganjil"
            }
        </script>
    </head>
    <body>
        <form method="POST" name="kirim">
            <p>BIL <input type="text" name="T1" size="20">
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
        </form>
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/15.png)
![gambar](tugas5/16.png)
* Form ```Button```
```python
<html>
    <head>
        <title>objek document</title>
    </head>
    <body>
        <script language="javascript">
            <!--
                function ubahWarnaLB(warna) {
                    document.bgColor = warna;
                }
                function ubahWarnaLD(warna) {
                    document.fgColor = warna;
                }
                //-->
        </script>

        <h1>tes</h1>
        <form>
            <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
            <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
            <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
            <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
        </form>
        <script language="javascript">
            <!--
                document.write("Dimodifikasi terakhir pada " +
                document.lastModified);
                //-->
        </script>
        
    </body>
</html>
```
* Hasil Output
![gambar](tugas5/17.png)
## HTML ```DOM```
* Pilihan menggunakan ```checkBox``` dengan perhitungan otomatis
![gambar](tugas5/dom.png)
* Hasil Output
![gambar](tugas5/20.png)
## Pertanyaan dan Tugas
1. ```Buat script untuk melakukan validasi pada isian form.```
![gambar](tugas5/code.hd.png)
![gambar](tugas5/codehome.png)
![gambar](tugas5/css.png)
* Hasil Output
![gambar](tugas5/18.png)
![gambar](tugas5/19.png)
## Laporan Praktikum
1. Buatlah repository baru dengan nama ```Lab5Web```.
2. Kerjakan semua latihan yang diberikan sesuai urutannya.
3. Screenshot setiap perubahannya.
4. Buatlah file README.md dan tuliskan penjelasan dari setiap langkah praktikum beserta
screenshotnya.
5. Commit hasilnya pada repository masing-masing.
6. Kirim URL repository pada e-learning ecampus