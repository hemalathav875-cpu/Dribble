# Project Responsive Web Design using Bootstrap
## Date:15.10.25

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
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble-Inspired Design Gallery</title>
  <!-- Bootstrap 5 CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      background-color: #f8f9fa;
      font-family: 'Segoe UI', sans-serif;
    }
    .navbar {
      background-color: #212529;
    }
    .navbar-brand, .nav-link, .navbar-text {
      color: white !important;
    }
    .gallery-card {
      border: none;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .gallery-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
    .footer {
      background-color: #212529;
      color: white;
      padding: 15px 0;
      text-align: center;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">dribbble</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="#">Shots</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Community</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
        </ul>
      </div>
      <span class="navbar-text">Sign up</span>
    </div>
  </nav>

  <!-- Gallery Section -->
  <div class="container py-5">
    <h2 class="text-center mb-4 fw-bold">Popular Shots</h2>
    <div class="row g-4">
      <!-- Card 1 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=1" class="card-img-top" alt="Design 1">
          <div class="card-body">
            <h6 class="card-title">Famous</h6>
            <p class="card-text text-muted mb-0">👁️ 4,044 &nbsp; ❤️ 290</p>
          </div>
        </div>
      </div>
      <!-- Card 2 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=2" class="card-img-top" alt="Design 2">
          <div class="card-body">
            <h6 class="card-title">Balkan Brothers</h6>
            <p class="card-text text-muted mb-0">👁️ 2,404 &nbsp; ❤️ 236</p>
          </div>
        </div>
      </div>
      <!-- Card 3 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=3" class="card-img-top" alt="Design 3">
          <div class="card-body">
            <h6 class="card-title">Jan Losert</h6>
            <p class="card-text text-muted mb-0">👁️ 3,386 &nbsp; ❤️ 264</p>
          </div>
        </div>
      </div>
      <!-- Card 4 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=4" class="card-img-top" alt="Design 4">
          <div class="card-body">
            <h6 class="card-title">Mattias Johansson</h6>
            <p class="card-text text-muted mb-0">👁️ 2,502 &nbsp; ❤️ 166</p>
          </div>
        </div>
      </div>
      <!-- Card 5 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=5" class="card-img-top" alt="Design 5">
          <div class="card-body">
            <h6 class="card-title">Artify</h6>
            <p class="card-text text-muted mb-0">👁️ 1,841 &nbsp; ❤️ 158</p>
          </div>
        </div>
      </div>
      <!-- Card 6 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=6" class="card-img-top" alt="Design 6">
          <div class="card-body">
            <h6 class="card-title">Range Studio</h6>
            <p class="card-text text-muted mb-0">👁️ 2,179 &nbsp; ❤️ 158</p>
          </div>
        </div>
      </div>
      <!-- Card 7 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=7" class="card-img-top" alt="Design 7">
          <div class="card-body">
            <h6 class="card-title">Techwave</h6>
            <p class="card-text text-muted mb-0">👁️ 1,872 &nbsp; ❤️ 148</p>
          </div>
        </div>
      </div>
      <!-- Card 8 -->
      <div class="col-md-3 col-sm-6">
        <div class="card gallery-card">
          <img src="https://picsum.photos/300/200?random=8" class="card-img-top" alt="Design 8">
          <div class="card-body">
            <h6 class="card-title">FourPlus Studio</h6>
            <p class="card-text text-muted mb-0">👁️ 1,371 &nbsp; ❤️ 127</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer class="footer">
    © 2025 Saraswati | Designed with Bootstrap
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
~~~

## OUTPUT:
<img width="628" height="413" alt="Screenshot 2025-10-15 102058" src="https://github.com/user-attachments/assets/185c7b76-9d14-4ef4-8e6e-7f17a715ea1f" />



## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
