# index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulir Pendaftaran Komunitas Teknologi</title>
</head>
<body>
   <h1 align="center">Formulir Pendaftaran Komunitas Teknologi</h1>
 <!-- form action untuk ke tujuan setelah form disubmit -->
    <form action="submit.html" method="post">
        <ul>
        <h3><li>Silahkan isi tabel dengan diperhatikan secara seksama, dan diisi dengan tempo yang sesingkat-singkatnya.</h3></li>
        </ul>
        <!-- fieldset untuk membuat kotak -->
         <!-- legend untuk membuat tulisan diatas kotak -->
        <fieldset>
            <legend>Nama</legend>
            <label for="nama">Nama Depan</label>
            <input type="text" name="nama" id="nama" placeholder="Muhammad" required maxlength="10" autocomplete="on"><br>
            <br>
            <label for="namatengah">Nama Tengah</label>
            <input type="text" name="namatengah" id="namatengah" placeholder="William" maxlength="10" autocomplete="on"><br>
            <br>
            <label for="namabelakang">Nama Belakang</label>
            <input type="text" name="namabelakang" id="namabelakang" placeholder="Fadly" maxlength="10" autocomplete="on"><br>
        </fieldset>
        <br> 
        <!-- br untuk break -->
        <fieldset>
            <legend>Kontak</legend>
            <label for="email">Email</label>
            <input 
                type="email" 
                name="email" 
                id="email" 
                placeholder="william@gmail.com"
                pattern="[a-z]@'.{5-20}"
                title="Email harus terdiri dari 5-12 huruf kecil saja."
                required
            >
            <!-- label digunakan untuk membuat nama dan memudahkan kalimat ditekan dan langsung menuju input -->
            <br><br>
            <label for="password">Kata Sandi</label>
            <!-- input untuk membuat tabel pengisian -->
            <input 
                type="password" 
                name="password" 
                id="password" 
                placeholder="masukkan kata sandi"
            >
            <br><br>
            <label for="telepon">Telepon</label>
            <input 
                type="tel" 
                name="telepon" 
                id="telepon" 
                pattern="[0-9]{10,14}"
                title="Harus Angka" 
                placeholder="08123456789" 
                autocomplete="on" 
                required
            >
            <!-- type untuk tipe pengisian form -->
             <!-- pattern untuk pola yang harus ditaati pada tabel form -->
            <br>  
        </fieldset>
        <br>
        <label for="usia">Usia</label>
        <input
            type="number" 
            name="usia"
            id="usia"
            max="50" 
            min="13"
        >
        <br><br>
        <label for="tanggallahir">Tanggal Lahir</label>
        <input 
            type="date" 
            name="tanggallahir" 
            id="tanggallahir"
            >
        <br><br>
        <label for="Laki-laki">Laki-laki</label>
        <input
            type="radio" 
            name="kelamin"
            id ="Laki-laki" 
            value="Laki-laki" 
            style="margin-right: 50px;"
        >
        <label for="Perempuan">Perempuan</label>
        <input
            type="radio" 
            name="kelamin" 
            id="Perempuan" 
            value="Perempuan"
        >
        <!-- untuk membuat hanya satu yang bisa dicentang maka name dari kedua input harus sama -->
        <br><br>
        <fieldset>
            <legend>Minat Komunitas</legend>
            <input type="checkbox" name="minat1" id="minat1" value="web development">
            <label for="minat1">Web Development</label><br>
            <input type="checkbox" name="minat2" id="minat2" value="data science">
            <label for="minat2">Data Science</label><br>
            <input type="checkbox" name="minat3" id="minat3" value="cyber security">
            <label for="minat3">Cyber Security</label><br>
            <input type="checkbox" name="minat4" id="minat4" value="mobile development">
            <label for="minat4">Mobile Development</label> <br>
        </fieldset> <br><br>
        <label for="website">Link Portofolio</label>
        <input 
            type="url"
            pattern="https?://.+"
            title="harus dimulai dengan https"
            required
        >
        <!-- required artinya form tersebut wajib diisi -->
        <br><br>
        <label for="file">Foto Formal</label>
        <input
            type="file" 
            name="file" 
            id="file"
        >
        <br><br>
        <div style="text-align:center;">
            <input type="submit" value="Kirim">
            <input type="reset" value="ulangi">
        </div>
    </form>
</body>
</html>
