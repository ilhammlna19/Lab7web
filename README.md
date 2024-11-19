# Lab7web
program sederhana
<!DOCTYPE html>
<html>
<head>
    <title>Form Input PHP</title>
</head>
<body>
    <h1>Form Input Data</h1>
    <form method="POST" action="">
        <label for="name">Nama:</label>
        <input type="text" id="name" name="name" required><br><br>

        <label for="birthdate">Tanggal Lahir:</label>
        <input type="date" id="birthdate" name="birthdate" required><br><br>

        <label for="job">Pekerjaan:</label>
        <select id="job" name="job" required>
            <option value="Programmer">Programmer</option>
            <option value="Desainer">Desainer</option>
            <option value="Manajer">Manajer</option>
        </select><br><br>

        <input type="submit" value="Submit">
    </form>

    <?php
    if ($_SERVER["REQUEST_METHOD"] == "POST") {
        // Mengambil data dari form
        $name = $_POST['name'];
        $birthdate = $_POST['birthdate'];
        $job = $_POST['job'];

        // Menghitung umur
        $birthDateObj = new DateTime($birthdate);
        $today = new DateTime();
        $age = $today->diff($birthDateObj)->y;

        // Menentukan gaji berdasarkan pekerjaan
        $salary = 0;
        switch ($job) {
            case "Programmer":
                $salary = 8000000;
                break;
            case "Desainer":
                $salary = 6000000;
                break;
            case "Manajer":
                $salary = 12000000;
                break;
        }

        // Menampilkan output
        echo "<h2>Hasil Input:</h2>";
        echo "Nama: $name<br>";
        echo "Tanggal Lahir: $birthdate<br>";
        echo "Umur: $age tahun<br>";
        echo "Pekerjaan: $job<br>";
        echo "Gaji: Rp " . number_format($salary, 0, ',', '.') . "<br>";
    }
    ?>
</body>
</html>
![image](https://github.com/user-attachments/assets/9b902353-7257-45b5-862c-bba52df46c88)

# menjalnkan web server
![image](https://github.com/user-attachments/assets/cbe0e3d1-d4b6-4114-8a3d-01d2d81da071)
# test server
![image](https://github.com/user-attachments/assets/be13eb63-0131-4121-974c-a3e284bec951)
# memulai php 
![image](https://github.com/user-attachments/assets/b200d664-c2c7-42d0-8764-4c332c58f130)
# akses file
![Screenshot (70)](https://github.com/user-attachments/assets/be9bde0b-9193-40f1-bc87-421972125888)
# php dasar
![Screenshot (71)](https://github.com/user-attachments/assets/688fda4b-9810-4033-8ad4-aa42c9155d17)
# variable php
![Screenshot (72)](https://github.com/user-attachments/assets/0025eaf9-4649-41ab-b1b2-efefd2b3dab1)
# predifine variable get
![Screenshot (73)](https://github.com/user-attachments/assets/46963868-2576-47ef-bc7d-25e3bfe1b754)
# form input
![image](https://github.com/user-attachments/assets/f27bfb0b-5664-4810-af4c-e3db89250771)

# operator
![image](https://github.com/user-attachments/assets/bc642451-736d-45a4-a947-171469cbc912)
# kondisi if
![image](https://github.com/user-attachments/assets/60e74f8a-c588-43b7-ab7b-de07a4e07e06)
# kondisi switch
![image](https://github.com/user-attachments/assets/9918a57e-5de0-4f5d-bf8e-f07bf1a86c19)
# perulangan for
![image](https://github.com/user-attachments/assets/191c6ff5-7811-4949-a5ba-51a8617cc2a2)
# perulangan while
![image](https://github.com/user-attachments/assets/dcaafab4-e3fb-48ea-b2fd-8025c690c1b7)
# perulangan dowile
![Uploading image.png…]()


Ilham Maulana
3121310514
TI 23 A1
