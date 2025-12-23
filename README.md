# Ex.06 Restaurant Website
## Date:19/12/2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ember & Spice</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Segoe UI', sans-serif;
    }

    body{
      background:#fafafa;
      color:#222;
    }

    header{
      background:#1a1a1a;
      color:#fff;
      padding:20px 50px;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    header h1{
      font-size:30px;
      letter-spacing:2px;
    }

    nav a{
      color:#fff;
      margin-left:20px;
      text-decoration:none;
      font-weight:600;
    }

    nav a:hover{
      color:#ff5722;
    }

    .hero{
      height:85vh;
      background:url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092') center/cover no-repeat;
      display:flex;
      justify-content:center;
      align-items:center;
    }

    .hero h2{
      font-size:50px;
      color:#fff;
      background:rgba(0,0,0,0.65);
      padding:25px 40px;
      border-radius:12px;
    }

    section{
      padding:70px 50px;
    }

    .section-title{
      text-align:center;
      margin-bottom:45px;
    }

    .section-title h2{
      font-size:38px;
      color:#1a1a1a;
    }

    .about{
      display:flex;
      gap:40px;
      align-items:center;
    }

    .about p{
      font-size:18px;
      line-height:1.7;
    }

    .about img{
      width:100%;
      max-width:450px;
      border-radius:20px;
    }

    .menu{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
      gap:30px;
    }

    .menu-item{
      background:#fff;
      border-radius:18px;
      box-shadow:0 8px 20px rgba(0,0,0,0.12);
      overflow:hidden;
      transition:transform 0.3s;
    }

    .menu-item:hover{
      transform:translateY(-8px);
    }

    .menu-item img{
      width:100%;
      height:200px;
      object-fit:cover;
    }

    .menu-item div{
      padding:18px;
      text-align:center;
    }

    .menu-item h3{
      margin-bottom:8px;
    }

    .gallery{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
      gap:25px;
    }

    .gallery img{
      width:100%;
      border-radius:18px;
    }

    .contact{
      background:#1a1a1a;
      color:#fff;
      text-align:center;
    }

    .contact p{
      margin:12px 0;
      font-size:17px;
    }

    footer{
      background:#000;
      color:#aaa;
      text-align:center;
      padding:18px;
    }

    @media(max-width:768px){
      .about{
        flex-direction:column;
      }
      .hero h2{
        font-size:34px;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>EMBER & SPICE</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#menu">Menu</a>
    <a href="#gallery">Gallery</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero" id="home">
  <h2>Where Fire Meets Flavor</h2>
</div>

<section id="about">
  <div class="section-title">
    <h2>About Ember & Spice</h2>
  </div>
  <div class="about">
    <p>
      Ember & Spice is a modern restaurant inspired by bold flavors and
      slow-cooked perfection. Every dish is crafted with passion, blending
      classic recipes with a contemporary touch to create an unforgettable
      dining experience.
    </p>
    <img src="https://images.unsplash.com/photo-1528605248644-14dd04022da1" alt="Interior">
  </div>
</section>

<section id="menu">
  <div class="section-title">
    <h2>Signature Menu</h2>
  </div>
  <div class="menu">
    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1604908177225-6c6fca31b3c5">
      <div><h3>Smoked Grilled Chicken</h3><p>₹299</p></div>
    </div>

    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1540189549336-e6e99c3679fe">
      <div><h3>Fresh Garden Salad</h3><p>₹199</p></div>
    </div>

    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1598515214146-dab39da1243d">
      <div><h3>Classic Cheese Pizza</h3><p>₹349</p></div>
    </div>

    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1551024601-bec78aea704b">
      <div><h3>Chocolate Dessert</h3><p>₹179</p></div>
    </div>
  </div>
</section>

<section id="gallery">
  <div class="section-title">
    <h2>Moments & Dishes</h2>
  </div>
  <div class="gallery">
    <img src="https://images.unsplash.com/photo-1555396273-367ea4eb4db5">
    <img src="https://images.unsplash.com/photo-1525351484163-7529414344d8">
    <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836">
    <img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
  </div>
</section>

<section id="contact" class="contact">
  <h2>Contact Us</h2>
  <p>📍 Chennai, India</p>
  <p>📞 +91 7871392938</p>
  <p>✉️ contact@emberandspice.com</p>
  <p>M Sharan Kumar</p>
  <p>25005446</p>
</section>

<footer>
  <p>© 2025 Ember & Spice. All Rights Reserved.</p>
</footer>

</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot 2025-12-19 143702.png>) ![alt text](<Screenshot 2025-12-19 143741.png>) ![alt text](<Screenshot 2025-12-19 143414.png>) ![alt text](<Screenshot 2025-12-19 143420.png>) ![alt text](<Screenshot 2025-12-19 143648.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
