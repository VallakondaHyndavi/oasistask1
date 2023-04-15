<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="menu.css">
  <title>Education Landing Page</title>
</head>
<body>
 <nav>
   <div class="logo">Education</div>
   <!-- toggle menu button -->
   <span class="menubtn" onclick="openNav()">&#9776;</span>
 
   <div class="navLinks">
     <ul>
       <li><a href="#">Home</a></li>
       <li><a href="#">About</a></li>
       <li><a href="#">Contact</a></li>
       <button type="button">Login</button>
     </ul>
   </div>
 </nav>
   <!-- responsive side navbar -->
   <div class="sideNav" id="sidenav">
     <a href="#" class="closeBtn" onclick="closeNav()"> &#10006;</a>
     <a href="#">Home</a>
     <a href="#">About</a>
     <a href="#">Contact</a>
     <a href="#"><button type="button">Login</button> </a>
   </div>
   
   <!-- Header content with banner image -->
   <div class="row">
     <div class="column1">
       <h1>Learning Spark</h1>
       <p>Education is the vaccine of violence..!</p>
       <button>Let's Begin...!</button>
     </div>
     <div class="column2">
       <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSjGlAXcOZHLzMkUEBwn8SSMOjnUAGxv7QJ-KJjH_K7Iw&usqp=CAU&ec=48665701" alt="banner" width="500px">
     </div>
   </div>
   
   <!-- javascript to make side menu appear -->
 <script>
   function openNav() {
     document.getElementById("sidenav").style.width = "50%";
   }
   function closeNav() {
     document.getElementById("sidenav").style.width = "0%";
   }
 </script>
 
</body>
</html>




*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  body {
    background-image: linear-gradient(to right, rgba(190, 181, 190, 0.75), rgba(105, 107, 112, 0.8)),url(https://contentstatic.timesjobs.com/img/64806753/Master.jpg);
    background-size: cover;
    background-attachment: fixed;
    color: rgb(19, 18, 18);
    font-family: 'Fira Sans', sans-serif;
  }
  nav {
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: space-between;
    padding: 35px 5%;
  }
  nav .logo{
    font-size: 30px;
    font-weight: 700;
  }
  nav ul{
    display: flex;
    list-style: none;
  }
  nav ul li{
    padding: 8px 15px;
    border-radius: 10px;
    transition: 0.2s ease-in;
  }
  nav ul li a{
    color: rgb(32, 31, 31);
    font-size: 20px;
    font-weight: 500;
    text-decoration: none;
  }
  nav .navLinks button{
    padding: 2px 20px;
    border-radius: 10px;
    color: rgb(10, 10, 10);
    font-size: 16px;
    border-style: none;
    font-weight: 700;
    margin-left: 10px;
  }
  nav ul li:hover{
    background-color: rgb(236, 235, 241);
  }
  nav .menubtn{
    font-size: 30px;
    font-weight: bolder;
    cursor: pointer;
    display: none;
  }
   
  /* responsive navbar css */
  @media screen and (max-width: 600px) {
    nav .menubtn{
      display: flex;
    }
    nav .navLinks{
      display: none;
    }
    .sideNav {
      display: block !important;
    }
  }
   
  .sideNav{
    height: 100%;
    position: fixed;
    top: 0;
    right: 0%;
    background-color: rgb(231, 230, 238);
    overflow-x: hidden;
    transition: 0.3s ease-in;
    padding-top: 60px;
    display: none;
  }
   
  .sideNav a{
    padding: 8px 8px 8px 40px;
    display: block;
    font-size: 25px;
    font-weight: 500;
    color: #0f0e0e;
    transition: 0.3s;
    text-decoration: none;
  }
  .sideNav a button {
    padding: 10px 20px;
    border-radius: 10px;
    color: rgb(13, 13, 14);
    font-size: 16px;
    border-style: none;
    font-weight: 700;
  }
  .sideNav a:hover{
    color: rgb(8, 8, 8);
  }
  .sideNav .closeBtn{
    position: absolute;
    top: 10px;
    right: 25px;
    font-size: 20px;
    margin-left: 50px;
  }
   
  .row{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 2% 5%;
  }
  .row .column1 {
    padding-right: 50px;
  }
  .column1 h1 {
    font-size: 60px;
    margin-bottom: 10px;
  }
  .column1 p {
    font-size: 25px;
    margin-bottom: 20px;
  }
  .column1 button {
    width: 150px;
    padding: 12px 20px;
    border-radius: 20px;
    border-style: none;
    color: rgb(10, 10, 10);
    font-size: 17px;
    font-weight: 600;
  }
  /* Header content responsive */
  @media screen and (max-width: 980px) {
    .column2 img {
      width: 350px;
    }
    .column1 h1 {
      font-size: 40px;
    }
    .column1 p{
      font-size: 17px;
    }
    .row {
      margin-top: 80px;
    }
  }
   
  @media screen and (max-width: 600px) {
   
    .column1 h1 {
      font-size: 35px;
    }
    .row {
      flex-direction: column;
   
    }
    .row .column1 {
      padding: 30px;
    }
  }
