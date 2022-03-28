# Lab3Web
## Langkah Langkah pembuatan
- Pertama,Membuat Tag html dasar dengan dinamai file lab 3 list,dengan bertujuan menggunakan list sebagai berikut. Lalu buatlah nama order list ada 3.
![image](https://user-images.githubusercontent.com/83681139/160327501-aa31f719-a375-4238-ae27-455fd66baf10.png)
- Kedua,Membuat kata unordered list pada section berikut.
![image](https://user-images.githubusercontent.com/83681139/160327548-87572684-15f1-46fa-9efd-3289036ba3a8.png)
- Lalu membuat Deskripsi list pada bagian berikut. 
![image](https://user-images.githubusercontent.com/83681139/160327583-f022707a-810f-43a1-88f8-de293029a28f.png)
- Lalu membuat file baru yang isinya terdapat tabel pada gambar berikut.
![image](https://user-images.githubusercontent.com/83681139/160327635-5c77ab37-ad2b-49d9-b821-c194a5eccc1c.png)
- Menambahkan style rospawn agar tulisan teknik menjadi 1 pada tabel berikut.
![image](https://user-images.githubusercontent.com/83681139/160327674-92faa01d-0d1d-4418-beb1-ad72d091d705.png)
- Lalu membuat form tabel pada modul yang suda diajarkan.
![image](https://user-images.githubusercontent.com/83681139/160327714-d61fd028-93a1-49a8-83ce-5a157c68f84e.png)
## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
![image](https://user-images.githubusercontent.com/83681139/160327775-6329af03-70cf-44ee-9486-c76d0b2fbe27.png)
## Berikut Codinganya:
```
<html>
<head>
    <title>Drop-down Menu</title>
    <link rel="stylesheet" href="Style.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>
<div class="menu-bar">
<ul>
<li class="active"><a href="#"><i class="fa fa-home"></i>Home</a>
</li>
<li><a href="#"><i class="fa fa-user"></i>About us</a>
    <div class="sub-menu-1">
        <ul>
            <li><a href="#">Mission</a></li>
            <li><a href="#">Vision</a></li>
            <li><a href="#">Team</a></li>
        </ul>
    </div>
</li>
<li><a href="#"><i class="fa fa-clone"></i>Services</a>
<div class="sub-menu-1">
<ul>
<li><a href="#">Web Design</a></li>
<li class="hover-me"><a href="#">Marketing</a><i class="fa fa-angle-right"></i>
    <div class="sub-menu-2">
        <ul>
            <li><a href="#">SEO</a></li>
            <li><a href="#">Social Media</a></li>
            <li><a href="#">Email Marketing</a></li>
        </ul>
    </div>
</li>
<li><a href="#">Mobile app</a><i class="fa fa-angle-right"> </i></li>
</ul>
</div>
</li>
<li><a href="#"><i class="fa fa-users"></i>Clients</a></li>
<li><a href="#"><i class="fa fa-angellist"></i>Investers</a></li>
<li><a href="#"><i class="fa fa-inr"></i>pricing</a></li>
<li><a href="#"><i class="fa fa-edit"></i>Training</a></li>
<li><a href="#"><i class="fa fa-phone"></i>Contact</a></li>
</ul>
</div>
</body>
</html>
```
## Style.css
```
*
{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body
{
    background-image: url(alam.jpg);
    background-size: cover;
    background-position: center;
    font-family: sans-serif;
}
.menu-bar
{
    background: rgb( 0,100,0);
    text-align: center;
}
.menu-bar ul
{
    display: inline-flex;
    list-style: none;
    color: #fff;
}
.menu-bar ul li
{
    width: 120px;
    margin: 15px;
    padding: 15px;
}
.menu-bar ul li a
{
    text-decoration: none;
    color: #fff;
}
.active, .menu-bar ul li:hover
{
    background: #2bad0d;
    border-radius: 3px;
}
.menu-bar .fa
{
    margin-right: 8px;
}
.sub-menu-1
{
    display: none;
}
.menu-bar ul li:hover .sub-menu-1
{
    display: block;
    position: absolute;
    background: rgb( 0,100,0);
    margin-top: 15px;
    margin-left: -15px;
}
.menu-bar ul li:hover .sub-menu-1 ul
{
    display: block;
    margin: 10px;
}
.menu-bar ul li:hover .sub-menu-1 ul li
{
    width: 150 px;
    padding: 10px;
    border-bottom: 1px dotted #fff;
    background: transparent;
    border-radius: 0;
    text-align: left;
}
.menu-bar ul li:hover .sub-menu-1 ul li:last-child
{
    border-bottom: none;
}
.menu-bar ul li:hover .sub-menu-1 ul li a:hover
{
    color: #b2ff00;
}
.fa-angle-right
{
    float: right;
}
.sub-menu-2
{
    display: none;
}
.hover-me:hover .sub-menu-2
{
    position: absolute;
    display: block;
    margin-top: -40px;
    margin-left: 140px;
    background: rgba(0,100,0);
}
```
