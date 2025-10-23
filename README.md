Perograman WEB Pertemuan 6

Nama    : RAFLI ANUGRAH RAMADHAN

Nim     : 312410351

Kelas   : TI.24.A4

1. Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut:

<img width="444" height="201" alt="image" src="https://github.com/user-attachments/assets/c32cca19-ec46-4fde-80bb-119a22b07ae1" />

2. Pemakaian Alert sebagai property window.

<img width="317" height="167" alt="image" src="https://github.com/user-attachments/assets/cc860736-6ac0-4bd0-9600-c7460080c9a4" />

3. Pemakaian method dalam objek

<img width="122" height="74" alt="image" src="https://github.com/user-attachments/assets/7673f3ce-15ea-4401-8d7b-37d685c6f9bf" />

4. Pemakaian Prompt

<img width="197" height="145" alt="image" src="https://github.com/user-attachments/assets/3276f675-9353-496f-8fa8-44dd5d656944" />

5. pembuatan fungsi dan cara pemanggilannya

<img width="1916" height="931" alt="image" src="https://github.com/user-attachments/assets/ddb383ef-f5d4-4d3b-80ee-dab900f0e7c9" />

6. Dasar Pemrograman Di Javascript Operasi dasar aritmatika

<img width="158" height="253" alt="image" src="https://github.com/user-attachments/assets/6316ca38-c906-4bce-8d51-31f7ef822458" />

<img width="332" height="274" alt="image" src="https://github.com/user-attachments/assets/e7b8ce26-093a-4a38-b80d-be260d8162a0" />

7. Seleksi kondisi (if..else)

<img width="353" height="134" alt="image" src="https://github.com/user-attachments/assets/9dba8cd6-4674-4f22-90b1-f0a2be154032" />

Masukan angka yang anda inginkan >60 lulus 

<img width="129" height="46" alt="image" src="https://github.com/user-attachments/assets/7ac89071-bd78-4689-bb77-d2dd69e3c37d" />

8. Penggunaan operator switch untuk seleksi kondisi

<img width="76" height="44" alt="image" src="https://github.com/user-attachments/assets/b92694cc-b771-41d7-9402-1555dd50acb0" />

masukaan angka yang anda inginkan (1-5) : contoh 4

<img width="94" height="41" alt="image" src="https://github.com/user-attachments/assets/d22942a7-86e9-4f6c-ab0a-90ef859287fd" />

apabila lebih dari : 6 sampai seterusnya

<img width="494" height="340" alt="image" src="https://github.com/user-attachments/assets/61361c18-0e1f-47e3-a4ed-52b81c218684" />

9. Pembuatan Form Form Input

<img width="550" height="252" alt="image" src="https://github.com/user-attachments/assets/585606fc-5e58-4b9d-81ea-f6e714772132" />

apabila angka 1 (ganjil) akan terisi otomatis : bilangan ganjil

apabila angka 2 (genap) akan terisi otomatis : bilangan genap

10. Form Button

<img width="1354" height="582" alt="image" src="https://github.com/user-attachments/assets/64b9b9bc-b54a-4cc8-a923-df28e5f214cb" />

dia akan berubah sesuai tombol yang diinginkan

11. HTML DOM Pilihan menggunakan checkBox dengan perhitungan otomatis

<img width="672" height="371" alt="image" src="https://github.com/user-attachments/assets/d53f467c-c66c-4a1b-a426-3ea2194a1ab5" />

ketika kamu milih menu dia akan otomatis tertotal harganya sendiri

# Soal Dan Pertanyaan

<img width="521" height="83" alt="image" src="https://github.com/user-attachments/assets/058ece84-ebbe-41ee-b111-8c658e6e48fb" />

KODE PROGRAM:

~~~ html
<!DOCTYPE html>
<html>
<head>
<title>Validasi Form</title>
<script>
function validasiForm() {
    var nama = document.forms["formData"]["nama"].value;
    var email = document.forms["formData"]["email"].value;
    var umur = document.forms["formData"]["umur"].value;

    // Validasi nama tidak boleh kosong
    if (nama == "") {
        alert("Nama tidak boleh kosong!");
        return false;
    }

    // Validasi email dengan pola sederhana
    var polaEmail = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!polaEmail.test(email)) {
        alert("Format email tidak valid!");
        return false;
    }

    // Validasi umur harus angka dan minimal 17 tahun
    if (isNaN(umur) || umur < 17) {
        alert("Umur harus berupa angka dan minimal 17 tahun!");
        return false;
    }

    alert("Form berhasil dikirim!");
    return true;
}
</script>
</head>

<body>
<h2>Formulir Pendaftaran</h2>
<form name="formData" onsubmit="return validasiForm()">
    Nama: <input type="text" name="nama"><br><br>
    Email: <input type="text" name="email"><br><br>
    Umur: <input type="text" name="umur"><br><br>
    <input type="submit" value="Kirim">
</form>
</body>
</html>
~~~

HASIL:

<img width="1061" height="372" alt="image" src="https://github.com/user-attachments/assets/2ffc6517-5520-4aa6-a940-8df7fdac8301" />

harus diisi seperti, contoh jika benar :

<img width="959" height="538" alt="image" src="https://github.com/user-attachments/assets/0aebf545-060b-4ad2-94db-b58e21187dc0" />

document.forms["formData"]["nama"].value mengambil nilai input.

alert() menampilkan pesan kesalahan jika ada isian yang tidak valid.

return false mencegah form dikirim jika validasi gagal.

return true hanya dijalankan jika semua isian valid.



