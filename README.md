# Title
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Zeyuan Song Portfolio</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#111;
    color:white;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:25px 10%;
    background:#181818;
}

.logo{
    font-size:1.5rem;
    font-weight:bold;
}

.nav-links{
    display:flex;
    gap:30px;
}

.nav-links button{
    background:none;
    border:none;
    color:white;
    cursor:pointer;
    font-size:1rem;
}

.nav-links button:hover{
    color:#4da6ff;
}

.section{
    display:none;
    padding:80px 10%;
    min-height:80vh;
}

.active{
    display:block;
}

.hero{
    text-align:center;
    margin-top:100px;
}

.hero h1{
    font-size:4rem;
}

.hero p{
    margin-top:15px;
    color:#bbb;
}

.card-container{
    display:flex;
    flex-wrap:wrap;
    gap:20px;
    margin-top:30px;
}

.card{
    background:#1f1f1f;
    padding:20px;
    width:300px;
    border-radius:10px;
}

.card h3{
    margin-bottom:10px;
}

.contact-item{
    margin:15px 0;
}

</style>
</head>

<body>

<nav>

<div class="logo">
Zeyuan Song
</div>

<div class="nav-links">
<button onclick="showSection('about')">About Me</button>
<button onclick="showSection('portfolio')">Portfolio</button>
<button onclick="showSection('contact')">Contact</button>
</div>

</nav>

<section id="about" class="section active">

<div class="hero">

<h1>Zeyuan Song</h1>

<p>
Gameplay Programmer | Unity | Unreal Engine
</p>

<p>
Master of Science in Game Science and Design
</p>

</div>

</section>

<section id="portfolio" class="section">

<h2>Projects</h2>

<div class="card-container">

<div class="card">
<h3>Tower Defense</h3>
<p>
2D Pixel Art Tower Defense built in Unity.
</p>
</div>

<div class="card">
<h3>Emergent Pursuit</h3>
<p>
Adaptive AI and Immersion Research Project.
</p>
</div>

<div class="card">
<h3>DX11 Renderer</h3>
<p>
Custom C++ Renderer with Shadow Mapping.
</p>
</div>

</div>

</section>

<section id="contact" class="section">

<h2>Contact</h2>

<div class="contact-item">
Email: your@email.com
</div>

<div class="contact-item">
GitHub: github.com/yourname
</div>

<div class="contact-item">
LinkedIn: linkedin.com/in/yourname
</div>

</section>

<script>

function showSection(id){

document.querySelectorAll('.section')
.forEach(section=>{
section.classList.remove('active');
});

document.getElementById(id)
.classList.add('active');

}

</script>

</body>
</html>
