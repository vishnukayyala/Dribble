# Project Responsive Web Design using Bootstrap
## Date: 19.11.24

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
# HTML
```
<!DOCTYPE html>
 <html lang="en">
 <head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Simplified Dribbble Clone</title>
 <link
 href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.
 css" rel="stylesheet"
 integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2
 QvZ6jIW3" crossorigin="anonymous">
 <link rel="stylesheet" href="style.css">
 </head>
 <body>
 <!--Navigation Bar-->
 <nav class="navbar navbar-expand-lg navbar-light bg-light">
 <div class="container-fluid">
 <a class="navbar-brand" href="#">Dribbble</a>
 <button class="navbar-toggler" type="button"
 data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
 aria-controls="navbarSupportedContent" aria-expanded="false"
 aria-label="Toggle navigation">
 <span class="navbar-toggler-icon"></span>
 </button>
 <div class="collapse navbar-collapse" id="navbarSupportedContent">
 <ul class="navbar-nav me-auto mb-2 mb-lg-0">
 <li class="nav-item"><a class="nav-link active"
 aria-current="page" href="#">Home</a></li>
 <li class="nav-item"><a class="nav-link"
 href="#">Discover</a></li>
 <li class="nav-item"><a class="nav-link"
 href="#">Community</a></li>
 </ul>
 <form class="d-flex">
 <input class="form-control me-2" type="search"
 placeholder="Search" aria-label="Search"
<button class="btn btn-outline-success"
 type="submit">Search</button>
 </form>
 <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
 <li class="nav-item"><a class="nav-link" href="#">Sign
 Up</a></li>
 <li class="nav-item"><a class="nav-link" href="#">Log
 In</a></li>
 </ul>
 </div>
 </div>
 </nav>
 <!--Hero Section-->
 <section class="hero-section bg-image" style="background-image:
 url('one.jpg'); height: 500px; background-size: cover;
 background-position: center;">
 <div class="container h-100">
 <div class="row h-100 align-items-center justify-content-center
 text-white">
 <div class="col-md-10 text-center">
 <h1 class="display-3">Showcase Your Work</h1>
 <p class="lead">Join the community to share, discover, and
 get inspired by the best designs.</p>
 <button class="btn btn-light btn-lg">Get Started</button>
 </div>
 </div>
 </div>
 </section>
 <!--Featured Works Section-->
 <section class="py-5 featured-works">
 <div class="container">
 <h2 class="mb-4">Featured Works</h2>
 <div class="row g-4">
 <div class="col-md-4">
 <div class="card">
 <img src="two.jpg" class="card-img-top" alt="Hand
 Bag">
 <div class="card-body">
<h5 class="card-title">Hand Bag</h5>
 <p class="card-text">Stay Cool And Stylish With
 Our Women's Bags Starting At Rs.699.00. Explore Our Latest Collection.
 Shop Online Today, Convenient & Flexible.</p>
 </div>
 </div>
 </div>
 <div class="col-md-4">
 <div class="card">
 <img src="three.jpg" class="card-img-top"
 alt="Sunglasses">
 <div class="card-body">
 <h5 class="card-title">Sunglasses</h5>
 <p class="card-text">New sunglass styles for men.
 Aviator sunglasses for men; one of the newest mens sunglasses
 available.</p>
 </div>
 </div>
 </div>
 <div class="col-md-4">
 <div class="card">
 <img src="four.jpg" class="card-img-top" alt="Sling
 Bags">
 <div class="card-body">
 <h5 class="card-title">Sling Bags</h5>
 <p class="card-text">Shop from a wide range of
 sling bags and handbags for women, men, and kids at Dribbble.</p>
 </div>
 </div>
 </div>
 </div>
 </div>
 </section>
 <!--Footer-->
 <footer class="footer">
 <div class="container">
 <p>&copy; 2023 Dribbble Clone. All Rights Reserved.</p>
 </div>
 </footer>
<script
 src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle
 .min.js"
 integrity="sha384-ka7Sk0Gln4+2m6D02300fdO3uMB5y3bZi4E1bkpbz0IEYtv3oBNjtmM6
 E8bD1zdh" crossorigin="anonymous"></script>
 </body>
 </html>
```

# CSS
```
/* Global Styles */
 * {
 box-sizing: border-box;
 margin: 0;
 padding: 0;
 }
 body {
 font-family:-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
 Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
 line-height: 1.6;
 color: #333;
 background-color: #f9f9f9;
 }
 .container {
 max-width: 1200px;
 margin: 0 auto;
 padding: 0 20px;
 }
 /* Navigation Bar Styles */
 .navbar-light {
 box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
 }
.navbar-brand {
 font-weight: bold;
 color: #0065BD;
 }
 .navbar-nav .nav-link {
 color: #333;
 transition: color 0.2s ease;
 }
 .navbar-nav .nav-link:hover,
 .navbar-nav .nav-link.active {
 color: #0065BD;
 }
 /* Hero Section Styles */
 .hero-section {
 display: flex;
 justify-content: center;
 align-items: center;
 color: #fff;
 background-position: center;
 background-size: cover;
 background-repeat: no-repeat;
 }
 .hero-section .display-3 {
 font-weight: bold;
 font-size: 48px;
 margin-bottom: 16px;
 }
 .hero-section .lead {
 font-size: 24px;
 margin-bottom: 32px;
 }
 .hero-section .btn-light {
 background-color: #fff;
 color: #0065BD;
border: none;
 padding: 12px 32px;
 font-size: 18px;
 cursor: pointer;
 }
 .hero-section .btn-light:hover {
 background-color: #f0f0f0;
 }
 /* Featured Works Section Styles */
 .featured-works {
 background-color: #fff;
 padding: 40px 0;
 }
 .featured-works .card {
 border: none;
 border-radius: 8px;
 box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
 overflow: hidden;
 transition: transform 0.3s ease, box-shadow 0.3s ease;
 }
 .featured-works .card:hover {
 transform: translateY(-10px) scale(1.05); /* Moves up and scales
 slightly */
 box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* Adds a more pronounced
 shadow */
 }
 .featured-works .card-img-top {
 object-fit: cover;
 width: 100%;
 height: 200px;
 }
 .featured-works .card-body {
 padding: 20px;
 }
.featured-works .card-title {
 font-weight: bold;
 font-size: 18px;
 margin-bottom: 8px;
 }
 .featured-works .card-text {
 color: #666;
 font-size: 16px;
 }
 /* Footer Styles */
 .footer {
 background-color: #333;
 color: #fff;
 text-align: center;
 padding: 20px 0;
 margin-top: 40px;
 }
 .footer p {
 margin-bottom: 8px;
 }
 /* Media Queries for Responsiveness */
 @media (max-width: 768px) {
 .hero-section .display-3 {
 font-size: 36px;
 }
 .hero-section .lead {
 font-size: 18px;
 }
 .featured-works .card-img-top {
 height: 150px;
 }
 }
 @media (max-width: 576px) {
 .hero-section {
height: auto;
 padding: 40px 0;
 }
 .hero-section .display-3 {
 font-size: 28px;
 }
 .hero-section .lead {
 font-size: 16px;
 }
 .featured-works .card {
 margin-bottom: 20px;
 }
 .featured-works .card-img-top {
 height: 100px;
 }
 }

```


## OUTPUT:

![image](https://github.com/user-attachments/assets/40d9157d-cf74-4601-858e-39065268f368)



## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
