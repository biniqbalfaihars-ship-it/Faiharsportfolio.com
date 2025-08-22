# faiharsportfolio.com
Portfolio of Faihars Bin Iqbal showcasing creative graphic design, branding, social media content, print layouts, and presentation designs. Highlighting skills and projects visually.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Faihars bin Iqbal - Portfolio</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap');

:root{
  --primary:#2563eb;
  --primary-dark:#1d4ed8;
  --bg:#f1f5f9;
  --card:#ffffff;
  --text:#1e293b;
  --muted:#64748b;
  --shadow:0 10px 25px rgba(0,0,0,.08);
}
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Poppins',sans-serif;background:var(--bg);color:var(--text);line-height:1.6;}

header{text-align:center;padding:60px 20px 40px;background:linear-gradient(135deg, var(--primary), var(--primary-dark));color:white;border-bottom-left-radius:60px;border-bottom-right-radius:60px;box-shadow:var(--shadow);}
header img{width:180px;height:180px;border-radius:50%;object-fit:cover;border:5px solid white;box-shadow:0 6px 20px rgba(0,0,0,.2);margin-bottom:20px;}
header h1{font-size:34px;font-weight:700;}
header h2{font-size:18px;font-weight:400;margin-top:6px;color:#e0f2fe;}
nav{margin-top:20px;display:flex;justify-content:center;gap:14px;flex-wrap:wrap;}
nav a{text-decoration:none;padding:10px 20px;border-radius:30px;font-weight:600;font-size:14px;color:var(--primary);background:white;transition:.3s;box-shadow:var(--shadow);}
nav a:hover{background:var(--primary-dark);color:white;transform:translateY(-2px);}
section{max-width:1000px;margin:60px auto;padding:30px;background:var(--card);border-radius:20px;box-shadow:var(--shadow);}
section h3{font-size:24px;font-weight:700;margin-bottom:18px;color:var(--primary-dark);text-align:center;}
section p{color:var(--muted);margin-bottom:14px;text-align:center;}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:20px;margin-top:20px;}
.card{background:var(--bg);border-radius:16px;padding:20px;transition:.3s;box-shadow:0 6px 16px rgba(0,0,0,.06);text-align:center;cursor:pointer;}
.card:hover{transform:translateY(-5px);box-shadow:0 12px 24px rgba(0,0,0,.12);}
.chip{display:inline-block;font-size:13px;background:var(--primary);color:white;padding:5px 12px;border-radius:999px;margin-bottom:12px;}
.card-content{display:none;margin-top:10px;text-align:center;}
.card-content img{width:100px;height:auto;margin:5px;cursor:pointer;transition:0.3s;}
.card-content img:hover{transform:scale(1.1);}
.card-content p{margin-bottom:12px;color:var(--muted);font-size:14px;font-weight:600;}

/* Skills two columns with black dots */
.skills-list{
  display:grid;
  grid-template-columns:repeat(2, 1fr);
  gap:10px 60px; /* row-gap, column-gap */
  list-style:none;
  padding:0;
}
.skills-list li{
  font-weight:bold;
  position:relative;
  padding-left:15px;
  margin-bottom:6px;
}
.skills-list li::before{
  content:"•";
  position:absolute;
  left:0;
  color:black;
}

.contact p{margin:8px 0;font-size:15px;}
.contact a{color:var(--primary-dark);text-decoration:none;font-weight:600;}
.contact a:hover{text-decoration:underline;}
footer{text-align:center;padding:25px 10px;color:var(--muted);}

/* Lightbox Styles */
#lightbox{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:rgba(0,0,0,0.9);
  display:none;
  justify-content:center;
  align-items:center;
  z-index:9999;
}
#lightbox img{
  max-width:90%;
  max-height:90%;
  border-radius:10px;
  box-shadow:0 0 20px rgba(0,0,0,0.5);
  animation:fadeIn 0.3s ease;
}
@keyframes fadeIn{
  from {opacity:0;transform:scale(0.8);}
  to {opacity:1;transform:scale(1);}
}
</style>
</head>
<body>

<header>
<img src="faihars.png" alt="Faihars Bin Iqbal">
<h1>Faihars bin Iqbal</h1>
<h2>Graphic Design & Data Entry Specialist</h2>
<nav>
  <a href="#about">About</a>
  <a href="#works">Works</a>
  <a href="#skills">Skills</a>
  <a href="#contact">Contact</a>
</nav>
</header>

<!-- About Me -->
<section id="about">
<h3>About Me</h3>
<p>Hi, I'm <b>Faihars Bin Iqbal</b> — a passionate <b>Graphic Designer</b>. I create clean, modern and conversion-focused designs that help brands tell their story visually. Since 2022, I’ve been consistently delivering high-quality results with attention to detail and client satisfaction.</p>
<p>Services I love: logo & branding, social media creatives, posters/banners, thumbnails, print layouts, and presentation design.</p>
</section>

<!-- Works -->
<section id="works">
<h3>My Works</h3>
<p>Some categories I work on:</p>
<div class="grid">

  <!-- Logo Design -->
  <div class="card" onclick="toggleContent('logo')">
    <span class="chip">Logo Design</span>
    <div class="card-content" id="logo">
      <p>Clean, memorable logos for brands and businesses.</p>
      <img src="logo1.png" alt="Logo 1" onclick="openLightbox(this.src)">
      <img src="logo2.png" alt="Logo 2" onclick="openLightbox(this.src)">
      <img src="logo3.png" alt="Logo 3" onclick="openLightbox(this.src)">
      <img src="logo4.png" alt="Logo 4" onclick="openLightbox(this.src)">
      <img src="logo5.png" alt="Logo 5" onclick="openLightbox(this.src)">
      <img src="logo6.png" alt="Logo 6" onclick="openLightbox(this.src)">
      <img src="logo7.png" alt="Logo 7" onclick="openLightbox(this.src)">
    </div>
  </div>

  <!-- Social Media -->
  <div class="card" onclick="toggleContent('social')">
    <span class="chip">Social Media</span>
    <div class="card-content" id="social">
      <p>Posters, banners, ad creatives optimized for reach.</p>
      <img src="social1.png" alt="Social Media 1" onclick="openLightbox(this.src)">
      <img src="social2.png" alt="Social Media 2" onclick="openLightbox(this.src)">
      <img src="social3.png" alt="Social Media 3" onclick="openLightbox(this.src)">
      <img src="social4.png" alt="Social Media 4" onclick="openLightbox(this.src)">
      <img src="social5.png" alt="Social Media 5" onclick="openLightbox(this.src)">
    </div>
  </div>

  <!-- Print Design -->
  <div class="card" onclick="toggleContent('print')">
    <span class="chip">Print Design</span>
    <div class="card-content" id="print">
      <p>Flyers, brochures, business cards, packaging & more.</p>
      <img src="print1.png" alt="Print 1" onclick="openLightbox(this.src)">
      <img src="print2.png" alt="Print 2" onclick="openLightbox(this.src)">
      <img src="print3.png" alt="Print 3" onclick="openLightbox(this.src)">
      <img src="print4.png" alt="Print 4" onclick="openLightbox(this.src)">
      <img src="print5.png" alt="Print 5" onclick="openLightbox(this.src)">
    </div>
  </div>

  <!-- Presentation -->
  <div class="card" onclick="toggleContent('presentation')">
    <span class="chip">Presentation</span>
    <div class="card-content" id="presentation">
      <p>Professional slides for business and academics.</p>
      <img src="presentation1.png" alt="Presentation 1" onclick="openLightbox(this.src)">
      <img src="presentation2.png" alt="Presentation 2" onclick="openLightbox(this.src)">
      <img src="presentation3.png" alt="Presentation 3" onclick="openLightbox(this.src)">
      <img src="presentation4.png" alt="Presentation 4" onclick="openLightbox(this.src)">
      <img src="presentation5.png" alt="Presentation 5" onclick="openLightbox(this.src)">
    </div>
  </div>

</div>
</section>

<!-- Skills -->
<section id="skills">
<h3>Skills</h3>
<ul class="skills-list">
  <li>Adobe Photoshop</li>
  <li>Adobe Illustrator</li>
  <li>Adobe InDesign</li>
  <li>CorelDRAW</li>
  <li>Canva</li>
  <li>Logo Design</li>
  <li>Branding & Identity</li>
  <li>Business Card & Stationery</li>
  <li>Banner / Poster / Flyer</li>
  <li>Social Media Post Design</li>
  <li>Thumbnail Design</li>
  <li>Brochure & Catalogue</li>
  <li>Photo Editing & Retouching</li>
  <li>Background Removal</li>
  <li>Color Correction</li>
  <li>Vector Illustration</li>
  <li>Typography</li>
  <li>Presentation Design</li>
  <li>Infographic Design</li>
  <li>Print Layout</li>
  <li>Mockup & Product Showcase</li>
  <li>Creative Layout & Ads</li>
  <li>File Prep for Print</li>
</ul>
</section>

<!-- Contact -->
<section id="contact" class="contact">
<h3>Contact</h3>
<p>Email: <a href="mailto:biniqbalfaihars@gmail.com">biniqbalfaihars@gmail.com</a></p>
<p>Phone: <a href="tel:01889840342">01889840342</a></p>
<p>Location: Chittagong, Bangladesh</p>
</section>

<footer>
© 2025 Faihars bin Iqbal — All Rights Reserved
</footer>

<!-- Lightbox -->
<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Zoomed Image">
</div>

<script>
function toggleContent(id){
  const contents = document.querySelectorAll('.card-content');
  contents.forEach(c=>{if(c.id !== id) c.style.display='none';});
  const el = document.getElementById(id);
  el.style.display = (el.style.display === 'block') ? 'none' : 'block';
}

function openLightbox(src){
  const lightbox = document.getElementById('lightbox');
  const img = document.getElementById('lightbox-img');
  img.src = src;
  lightbox.style.display = 'flex';
}

function closeLightbox(){
  document.getElementById('lightbox').style.display = 'none';
}
</script>

</body>
</html>
