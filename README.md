<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>محمد اسماعيل محمد | Premium Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0a0f1c;
  --text:#ffffff;
  --accent:#00c6ff;
  --accent2:#0072ff;
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Inter',sans-serif;
}

body{
  background:var(--bg);
  color:var(--text);
  overflow-x:hidden;
}

/* Animated Background */
.background{
  position:fixed;
  width:100%;
  height:100%;
  background:linear-gradient(135deg,#00c6ff22,#0072ff22);
  z-index:-2;
}

.hero{
  height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  flex-direction:column;
  padding:20px;
}

.profile-img{
  width:170px;
  height:170px;
  border-radius:50%;
  object-fit:cover;
  border:4px solid var(--accent);
  box-shadow:0 0 40px rgba(0,198,255,0.5);
  opacity:0;
  transform:translateY(-30px) scale(0.8);
  animation:fadeIn 1.2s ease forwards;
}

@keyframes fadeIn{
  to{
    opacity:1;
    transform:translateY(0) scale(1);
  }
}

.hero h1{
  margin-top:20px;
  font-size:48px;
  background:linear-gradient(90deg,var(--accent),var(--accent2));
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.hero p{
  margin-top:15px;
  max-width:600px;
  opacity:0.85;
}

.btn{
  margin-top:25px;
  padding:12px 28px;
  border-radius:30px;
  text-decoration:none;
  font-weight:600;
  background:linear-gradient(90deg,var(--accent),var(--accent2));
  color:#fff;
  transition:0.3s;
}

.btn:hover{
  transform:translateY(-4px);
  box-shadow:0 10px 25px rgba(0,198,255,0.4);
}

/* Sections */
.section{
  padding:100px 20px;
  text-align:center;
}

.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:20px;
  margin-top:40px;
}

.card{
  background:rgba(255,255,255,0.05);
  padding:25px;
  border-radius:15px;
  backdrop-filter:blur(12px);
  transition:0.3s;
}

.card:hover{
  transform:translateY(-8px);
}

.contact-buttons{
  margin-top:40px;
  display:grid;
  gap:15px;
  max-width:400px;
  margin-left:auto;
  margin-right:auto;
}

.contact-btn{
  padding:14px;
  border-radius:10px;
  text-decoration:none;
  font-weight:600;
  transition:0.3s;
}

.phone{background:#22c55e;color:#fff;}
.whatsapp{background:#25D366;color:#fff;}
.email{background:var(--accent);color:#000;}

.contact-btn:hover{
  transform:scale(1.05);
}

footer{
  text-align:center;
  padding:20px;
  opacity:0.7;
}

/* Floating particles */
.particle{
  position:fixed;
  width:6px;
  height:6px;
  background:white;
  border-radius:50%;
  opacity:0.3;
  animation:float 6s infinite ease-in-out;
}

@keyframes float{
  0%{transform:translateY(0);}
  50%{transform:translateY(-20px);}
  100%{transform:translateY(0);}
}
</style>
</head>

<body>

<div class="background"></div>

<!-- Floating particles -->
<script>
for(let i=0;i<25;i++){
  let p=document.createElement("div");
  p.className="particle";
  p.style.left=Math.random()*100+"vw";
  p.style.top=Math.random()*100+"vh";
  p.style.animationDuration=(3+Math.random()*5)+"s";
  document.body.appendChild(p);
}
</script>

<section class="hero">
<img src="profile.jpg" class="profile-img" alt="Profile">

<h1>محمد اسماعيل محمد</h1>
<p>
HVAC Engineer & Software Developer building modern digital systems
with professional quality and clean design.
</p>

<a href="#contact" class="btn">Contact Me</a>
</section>

<section class="section">
<h2>Skills</h2>
<div class="grid">
<div class="card">HTML / CSS / JavaScript</div>
<div class="card">Python Development</div>
<div class="card">Telegram Bots</div>
<div class="card">HVAC Systems</div>
</div>
</section>

<section id="contact" class="section">
<h2>Contact</h2>

<div class="contact-buttons">
<a class="contact-btn phone" href="tel:01211291411">📞 Call 01211291411</a>
<a class="contact-btn whatsapp" href="https://wa.me/201211291411" target="_blank">💬 WhatsApp</a>
<a class="contact-btn email" href="mailto:mohmedalawamy2732010@gmail.com">📧 Email Me</a>
</div>

</section>

<footer>
© 2026 محمد اسماعيل محمد
</footer>

</body>
</html>
