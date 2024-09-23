---
layout: base
title: Nora's Homepage :3
description: Home Page
hide: true
---

<head>
  
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(3, 1fr); /* make 3 columns */
      gap: 10px; /* put gap between grid items */
      text-align: center; /* center text & images */
    }
    .grid-item img {
      width: 100%; /* Make image full width */
      height: auto; /* keep aspect ratio */
    }
    p {text-align: center;}
    .column {
    float: right;
    width: 100%;
    padding: 2px;
    }
    .row {
    display: flex;
    }
    .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
            gap: 10px;
        }
        .grid-item {
            text-align: center;
        }
        .grid-item img {
            width: 100%;
            height: 200px; 
            max-height: 200px;
            object-fit: contain; /* make image fit with fixed height */
        }
        .grid-item p {
            margin: 5px 0; 
        }
        .center {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 50%;
}
  </style>

</head>

<body>

<h2 style="text-align:center;">✧˖°  Welcome to Nora Ahadian's blog!!  °˖✧</h2>
<br>


<strong><p> Would you like a fruit? </p></strong>

<div class="grid-container" id="grid_container">
</div>

  <div class="grid-container">
  <div class="grid-item">
    <a href="https://youtu.be/ZWjR3d0WGBE">
      <img src="images/apple.png" alt="apple">
      <p>Yummy Apple</p>
    </a>
  </div>
  <div class="grid-item">
    <a href="https://youtu.be/kaIpvamevnc">
      <img src="images/grape.png" alt="grape">
      <p>Delicious Grapes</p>
    </a>
  </div>
  <div class="grid-item">
    <a href="https://youtu.be/GFaLrFe4w9g">
      <img src="images/orange.png" alt="orange">
      <p>Wow an orange</p>
    </a>
  </div>
  <div class="grid-item">
    <a href="https://youtu.be/-OmGLzgTa-4">
      <img src="images/cherrys.png" alt="cherry">
      <p>Cherry!</p>
    </a>
  </div>
  <div class="grid-item">
    <a href="https://youtu.be/V1VFy7S7GEU">
      <img src="images/pear.png" alt="pear">
      <p>Juicy pear</p>
    </a>
  </div>
</div>
<br>
<br>
<br>
<h2 style="text-align:center;"> Thanks for visiting my page </h2>

<img src="images/byeCat.gif" alt="Bye bye cat" class= "center"> 

</body>