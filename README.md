# PROGRAM KALKULATOR SEDERHANA


## Description

Program kalkulator ini dibuat dengan menggunakan Bootstrap 4.


## Getting Started

### Requirements

* Download Bootstrap 4 
`(https://getbootstrap.com/docs/4.3/getting-started/download)`
* Download Jquery.js
`(https://jquery.com/download)`
* Download Popper.js
`(https://cdnjs.cloudflare.com/ajax/libs/popper.js)`
* Browser
* Sistem Operasi Windows, etc.

### Installing

- Install Web Server (Xampp)
`(https://www.apachefriends.org/download.html)`
- Install Text Editor (Sublime Text 3)
`(https://www.sublimetext.com/3)`

### Executing Program

* Buka xampp
* Aktifkan Apache dan MySQL
* Buka folder C/xampp/htdocs/nama_folder_yang_dibuat
* Buat 2 folder dengan nama css dan js
* Buat file .php dengan nama kalkulator.php
 ```Code
  <!DOCTYPE html>
	<html>
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width,
		initial scale=1, shrink-to-fit=no">

		<link rel="stylesheet" href="assets/css/bootstrap.css"> 

		<title>Kalkulator Sederhana</title>
	</head>
	<body>

		<div class="jumbotron text-center bg-info" >
		 	<h3><b>PROGRAM KALKULATOR SEDERHANA</b></h3>
		</div>
		 
		<div class="container">

		<form method="POST" >
			<div class="form-group">
			 	<label for="bil">Bilangan 1 : </label>
			 	<input type="text" class="formcontrol" id="bil" name="bil1" placeholder="Masukkan Bilangan 1" required>
		 	</div>
		 	<div class="form-group">
			 	<label for="bil">Bilangan 2 : </label>
			 	<input type="text" class="formcontrol" id="bil" name="bil2" placeholder="Masukkan Bilangan 2" required>
		 	</div>
		
		 <button type="submit" name="submit" class="btn btn-primary">Hitung</button>
		 </form>

		 <hr>
		 <hr>
		 <?php
		 		if (isset($_POST['submit'])) {

			 	$bil1 = $_POST['bil1'];
				$bil2 = $_POST['bil2'];

				//pembuatan fungsi penjumlahan
				function hitungPenjumlahan($bil1, $bil2){
					$penjumlahan = $bil1 + $bil2;
					return $penjumlahan;
				}

				//pembuatan fungsi pengurangan
				function hitungPengurangan($bil1, $bil2){
					$pengurangan = $bil1-$bil2;
					return $pengurangan;
				}

				//pembuatan fungsi perkalian
				function hitungPerkalian($bil1, $bil2){
					$perkalian = $bil1*$bil2;
					return $perkalian;
				}

				//pembuatan fungsi pembagian
				function hitungPembagian($bil1, $bil2){
					$pembagian = $bil1/$bil2;
					return $pembagian;
				}
			
				//memanggil fungsi yang sudah dibuat diatas
				echo "Hasil penjumlahan adalah : " .hitungPenjumlahan($bil1,$bil2);
				echo "<br>";
				echo "Hasil pengurangan adalah : " .hitungPengurangan($bil1,$bil2);
				echo "<br>";
				echo "Hasil perkalian adalah : " .hitungPerkalian($bil1,$bil2);
				echo "<br>";
				echo "Hasil pembagian adalah : " .hitungPembagian($bil1,$bil2);
			}
		 ?>

		 </div>
		
		<script src="assets/js/jquery.js"></script>
		<script src="assets/js/popper.js"></script>
		<script src="assets/js/bootstrap.js"></script>	
  </body>
  </html>	
  ```
* File bootstrap yang sudah di download di extract dan disimpan di dalam folder css
* File jquery.js dan popper.js disimpan di dalam folder js
* Buka web browser, ketik: 
  ```
  localhost/nama_folder_yang_dibuat/kalkulator.php/
  ```
* Finally, program berhasil dijalankan


## Struktur File
```
|───README.md
|───assets
|    ├───css
|    |	 ├─── **/*.css
|    └───js
|		 ├─── **/*.js
|───kalkulator.php
```

## Credits
=======

Annisa Puspa Ranti
