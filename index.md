<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://use.fontawesome.com/releases/v5.0.7/css/all.css" rel="stylesheet">
    <link rel="stylesheet" href="styles/style.css">
<link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">
    <title>Melissa K. Jeremie</title>
  </head>

<header>
  <div id="myNav" class="overlay">

    <!-- Button to close the overlay navigation -->
    <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>

    <!-- Overlay content -->
    <div class="overlay-content">
      <a href="#about" onclick="closeNav()">About</a>
      <a href="#work"onclick="closeNav()">Work</a>
      <a href="#skills"onclick="closeNav()">Skills</a>
      <a href="#contact"onclick="closeNav()">Contact</a>
    </div>

  </div>
  <span onclick="openNav()"><i class="fas fa-bars" id="bars"></i></span>
</header>

<body style="">

<div id="home" style="font-size: 70px;">
hello there. <br>i'm <span class="name">melissa jeremie</span>,<br> a <span class="title">web developer</span> in <br> new york city. take a <br>look at some of my <br> <a href="#work" class="scroll">work</a>, read a bit  <a href="#about" class="scroll">about</a> me, <br> and feel free to <a href="#contact" class="scroll">reach out.</a>
</div>

<div id="about">

<h2>about me section will go here</h2>


</div>

<div id="work">

<h2>projects will go here</h2>


</div>

<div id="skills">

<h2>skills icons here</h2>


</div>

<div id="contact">

<h2>contact me will go here</h2>


</div>

<script src="js/main.js"></script>




  </body>
</html>

/* The Overlay (background) */
.overlay {
  /* Height & width depends on how you want to reveal the overlay (see JS below) */
  height: 100%;
  width: 0;
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  left: 0;
  top: 0;
  background-color: rgb(0,0,0); /* Black fallback color */
  background-color: rgba(0,0,0, 0.95); /* Black w/opacity */
  overflow-x: hidden; /* Disable horizontal scroll */
  transition: 0.5s; /* 0.5 second transition effect to slide in or slide down the overlay (height or width, depending on reveal) */
}

/* Position the content inside the overlay */
.overlay-content {
  position: relative;
  top: 25%; /* 25% from the top */
  width: 100%; /* 100% width */
  text-align: center; /* Centered text/links */
  margin-top: 30px; /* 30px top margin to avoid conflict with the close button on smaller screens */
}

/* The navigation links inside the overlay */
.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 75px;
  font-weight: bold;
  color: #818181;
  display: block; /* Display block instead of inline */
  transition: 0.35s; /* Transition effects on hover (color) */
}

/* When you mouse over the navigation links, change their color */
.overlay a:hover, .overlay a:focus {
  color: hotpink;
}

/* Position the close button (top right corner) */
.overlay .closebtn {
  position: absolute;
  top: 20px;
  right: 45px;
  font-size: 60px;
}

/* When the height of the screen is less than 450 pixels, change the font-size of the links and position the close button again, so they don't overlap */
@media screen and (max-height: 450px) {
  .overlay a {font-size: 20px}
  .overlay .closebtn {
    font-size: 40px;
    top: 15px;
    right: 35px;
  }
}

 #bars {
color: #986172;
font-size: 40px;
position: fixed;
right: 0;
}

#bars:hover {
  color: hotpink;
}

body {
background: #ffffff;
font-family: 'Montserrat', sans-serif;
font-weight: 100;
}

.name {
  font-size: 75px;
  font-weight: 400;
  color: gray;
}

.scroll {
  text-decoration: none;
  color: #986172;
  font-family: 'Montserrat', sans-serif;
  font-weight: 100;
}

.scroll:hover {
  color: hotpink;
  font-weight: bold;
}

#work {
height: 175px;
}

#skills {
height: 175px;
}

#about {
height: 175px;
}

#contact {
height: 175px;
}


/* Open when someone clicks on the span element */
function openNav() {
  document.getElementById("myNav").style.width = "100%";
}

/* Close when someone clicks on the "x" symbol inside the overlay */
function closeNav() {
  document.getElementById("myNav").style.width = "0%";
}
