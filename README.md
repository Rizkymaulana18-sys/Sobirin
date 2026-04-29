<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portofolio Profesional</title>

<!-- Bootstrap -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- AOS Animation -->
<link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">

<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
body {
  font-family: 'Segoe UI', sans-serif;
  transition: 0.3s;
}

.dark-mode {
  background: #121212;
  color: white;
}

.navbar {
  transition: 0.3s;
}

.navbar.scrolled {
  background: #000 !important;
}

.hero {
  height: 100vh;
  background: linear-gradient(135deg, #0d6efd, #6f42c1);
  color: white;
  display: flex;
  align-items: center;
}

.profile {
  width: 160px;
  border-radius: 50%;
  border: 5px solid white;
}

.section {
  padding: 80px 0;
}

.project-card {
  border: none;
  overflow: hidden;
  transition: 0.3s;
}

.project-card:hover {
  transform: translateY(-10px);
}

.project-card img {
  transition: 0.3s;
}

.project-card:hover img {
  transform: scale(1.1);
}

.skill-bar {
  height: 8px;
  background: #ddd;
  border-radius: 10px;
}

.skill-fill {
  height: 100%;
  background: #0d6efd;
  border-radius: 10px;
}

footer {
  background: #000;
  color: white;
}
</style>

</head>

<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark fixed-top">
  <div class="container">
    <a class="navbar-brand" href="#">Rizky</a>
    <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#nav">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="nav">
      <ul class="navbar-nav ms-auto">
        <li><a class="nav-link" href="#home">Home</a></li>
        <li><a class="nav-link" href="#about">About</a></li>
        <li><a class="nav-link" href="#project">Project</a></li>
        <li><a class="nav-link" href="#contact">Contact</a></li>
      </ul>
      <button onclick="toggleDark()" class="btn btn-outline-light ms-3">🌙</button>
    </div>
  </div>
</nav>

<!-- Hero -->
<section id="home" class="hero">
  <div class="container text-center" data-aos="fade-up">
    <img src="https://via.placeholder.com/150" class="profile mb-3">
    <h1 class="fw-bold">Rizky Maulana</h1>
    <p class="lead">Web Developer | GIS Enthusiast | Freelancer</p>
    <a href="#project" class="btn btn-light mt-3">Lihat Project</a>
  </div>
</section>

<!-- About -->
<section id="about" class="section">
  <div class="container">
    <div class="row align-items-center">
      
      <div class="col-md-6" data-aos="fade-right">
        <h2>Tentang Saya</h2>
        <p>Saya fokus pada pengembangan website modern dan sistem berbasis GIS. Berpengalaman dalam membangun aplikasi berbasis web yang responsif dan interaktif.</p>
      </div>

      <div class="col-md-6" data-aos="fade-left">
        <p>HTML</p>
        <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>

        <p class="mt-3">CSS</p>
        <div class="skill-bar"><div class="skill-fill" style="width:85%"></div></div>

        <p class="mt-3">JavaScript</p>
        <div class="skill-bar"><div class="skill-fill" style="width:75%"></div></div>
      </div>

    </div>
  </div>
</section>

<!-- Project -->
<section id="project" class="section bg-light">
  <div class="container">
    <h2 class="text-center mb-5">Project</h2>

    <div class="row">

      <div class="col-md-4" data-aos="zoom-in">
        <div class="card project-card">
          <img src="https://via.placeholder.com/400">
          <div class="card-body">
            <h5>GIS Mangrove</h5>
            <p>Sistem pemetaan area konservasi berbasis GIS.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4" data-aos="zoom-in">
        <div class="card project-card">
          <img src="https://via.placeholder.com/400">
          <div class="card-body">
            <h5>Website Toko</h5>
            <p>E-commerce modern menggunakan Bootstrap.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4" data-aos="zoom-in">
        <div class="card project-card">
          <img src="https://via.placeholder.com/400">
          <div class="card-body">
            <h5>Portfolio</h5>
            <p>Website personal branding profesional.</p>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- Contact -->
<section id="contact" class="section text-center">
  <div class="container" data-aos="fade-up">
    <h2>Kontak</h2>
    <p>Email: rizky@email.com</p>
    <p>
      <i class="fab fa-instagram me-3"></i>
      <i class="fab fa-github me-3"></i>
      <i class="fab fa-linkedin"></i>
    </p>
  </div>
</section>

<!-- Footer -->
<footer class="text-center p-3">
  © 2026 Rizky Maulana
</footer>

<!-- Script -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
<script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>

<script>
AOS.init();

window.addEventListener("scroll", function() {
  document.querySelector(".navbar").classList.toggle("scrolled", window.scrollY > 50);
});

function toggleDark() {
  document.body.classList.toggle("dark-mode");
}
</script>

</body>
</html>
