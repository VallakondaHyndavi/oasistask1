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




