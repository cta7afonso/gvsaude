<!DOCTYPE html>
<html lang="pt-PT">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Grupo Varandas da Saúde</title>

<meta name="description" content="Clínica multidisciplinar em Viana do Castelo. Medicina do Trabalho, especialidades médicas e controlo de pragas.">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>

/* RESET */

*{
margin:0;
padding:0;
box-sizing:border-box;
}

/* VARIÁVEIS */

:root{

--primary:#5bbad6;
--primary-dark:#3f9bb6;

--accent-pink:#e9b8d9;
--accent-yellow:#f4d48c;
--accent-green:#bfe3a6;

--bg:#f6f9fc;
--white:#ffffff;
--text:#2a3b4c;
--gray:#6b7c93;
--border:#e6edf5;

}

/* BODY */

body{

font-family:'Segoe UI',system-ui,sans-serif;
line-height:1.7;
color:var(--text);
background:var(--bg);

}

/* HEADER */

header{

position:fixed;
top:0;
width:100%;

background:rgba(255,255,255,0.95);
backdrop-filter:blur(8px);

box-shadow:0 2px 12px rgba(0,0,0,0.06);

padding:1rem 6%;

display:flex;
justify-content:space-between;
align-items:center;

z-index:1000;

}

/* LOGOS */

.logo-container{

display:flex;
align-items:center;
gap:1.4rem;

}

.logo-container img{

height:50px;
width:auto;
max-width:140px;

object-fit:contain;
display:block;

}

/* NAV */

nav a{

margin-left:1.6rem;
text-decoration:none;

color:var(--text);
font-weight:600;

transition:0.25s;

}

nav a:hover{
color:var(--primary);
}

/* HERO */

.hero{

background:
linear-gradient(rgba(70,140,170,0.45),rgba(70,140,170,0.45)),
url("https://images.unsplash.com/photo-1576092768241-dec2310aa3f5?auto=format&fit=crop&w=1920&q=80");

background-size:cover;
background-position:center;

color:white;

text-align:center;

padding:220px 6% 140px;

}

.hero h1{

font-size:3.4rem;
margin-bottom:1rem;

}

.hero p{

font-size:1.35rem;
max-width:900px;
margin:auto;

}

/* SEÇÕES */

section{

padding:100px 6%;

}

h2{

text-align:center;
margin-bottom:3rem;

color:var(--primary-dark);
font-size:2.6rem;

}

/* UNIDADES */

.units{

display:grid;

grid-template-columns:repeat(auto-fit,minmax(340px,1fr));

gap:2rem;

max-width:1300px;
margin:auto;

}

.unit-card{

background:var(--white);

border-radius:18px;
overflow:hidden;

border:1px solid var(--border);

box-shadow:0 8px 24px rgba(0,0,0,0.08);

transition:0.3s;

}

.unit-card:hover{

transform:translateY(-6px);

box-shadow:0 12px 28px rgba(0,0,0,0.12);

}

.unit-header{

color:white;

padding:1.6rem;

text-align:center;

font-size:1.8rem;

}

.unit-card:nth-child(1) .unit-header{
background:var(--accent-pink);
}

.unit-card:nth-child(2) .unit-header{
background:var(--accent-yellow);
}

.unit-card:nth-child(3) .unit-header{
background:var(--accent-green);
}

.unit-content{

padding:2.3rem;

}

.services-grid{

display:grid;

grid-template-columns:repeat(auto-fit,minmax(150px,1fr));

gap:1rem;

margin-top:1.5rem;

}

.service-item{

background:#f6f9fc;

padding:0.9rem;

border-radius:10px;

text-align:center;

font-weight:600;

border:1px solid var(--border);

transition:0.25s;

}

.service-item:hover{

background:var(--primary);
color:white;

}

/* MAPA */

#map-section{

background:#f0f5fa;

}

#map{

height:520px;

border:none;

width:100%;

max-width:1300px;

margin:auto;
display:block;

border-radius:16px;

box-shadow:0 10px 30px rgba(0,0,0,0.1);

}

/* FOOTER */

footer{

background:white;

padding:4rem 6% 2rem;

border-top:1px solid var(--border);

}

.footer-grid{

display:grid;

grid-template-columns:repeat(auto-fit,minmax(260px,1fr));

gap:3rem;

max-width:1300px;
margin:auto;

}

.footer-col h4{

font-size:1.3rem;

margin-bottom:1rem;

color:var(--primary-dark);

}

.footer-col p,
.footer-col a{

font-size:1rem;

color:#4a5c6a;

margin:0.4rem 0;

text-decoration:none;

}

.footer-col a:hover{
color:var(--primary);
}

/* REDES SOCIAIS */

.social-section{

text-align:center;

margin-top:2rem;

padding-top:2rem;

border-top:1px solid var(--border);

}

.social-group{

display:flex;

justify-content:center;

gap:4rem;

flex-wrap:wrap;

}

.social-unit{

text-align:center;

}

.social-unit h5{

margin-bottom:0.7rem;

color:var(--primary-dark);

}

.social-icons{

display:flex;

justify-content:center;

gap:1.6rem;

}

.social-icons a{

font-size:2rem;

color:var(--gray);

transition:0.3s;

}

.social-icons a:hover{

color:var(--primary);

transform:translateY(-4px);

}

/* COPYRIGHT */

.copyright{

text-align:center;

margin-top:3rem;

padding-top:1.5rem;

border-top:1px solid var(--border);

font-size:0.9rem;

}

/* RESPONSIVO */

@media(max-width:768px){

header{

flex-wrap:wrap;
justify-content:center;

}

.logo-container{

margin-bottom:0.8rem;

flex-wrap:wrap;
justify-content:center;

}

nav{

width:100%;
display:flex;
justify-content:center;

}

nav a{

margin:0 1rem;

}

.hero{

padding:160px 6% 100px;

}

.hero h1{

font-size:2.4rem;

}

#map{

height:420px;

}

}

</style>

</head>

<body>


<header>

<div class="logo-container">

<img src="images/logo-grupo-varandas.png" alt="Grupo Varandas da Saúde" loading="lazy">

<img src="images/logo-clinica-bandeira.png" alt="Clínica da Bandeira" loading="lazy">

<img src="images/logo-varandas-saude.png" alt="Varandas da Saúde" loading="lazy">

<img src="images/logo-prevent-control.png" alt="Prevent Control" loading="lazy">

</div>

<nav>

<a href="#unidades">Unidades</a>

<a href="#map-section">Localização</a>

<a href="#contatos">Contactos</a>

</nav>

</header>


<section class="hero">

<h1>Excelência em Cuidados de Saúde e Segurança</h1>

<p>
Clínica multidisciplinar, Medicina do Trabalho, Higiene e Segurança no Trabalho e Controlo de Pragas.
Atendimento profissional em Viana do Castelo desde 1997.
</p>

</section>


<section id="unidades">

<h2>As Nossas Unidades</h2>

<div class="units">


<div class="unit-card">

<div class="unit-header">
Clínica da Bandeira
</div>

<div class="unit-content">

<p>Cuidados de saúde gerais e especializados focados no bem-estar do paciente.</p>

<div class="services-grid">

<div class="service-item">Medicina Geral</div>
<div class="service-item">Endocrinologia</div>
<div class="service-item">Psiquiatria</div>
<div class="service-item">Reumatologia</div>
<div class="service-item">Nutrição</div>
<div class="service-item">Osteopatia</div>
<div class="service-item">Enfermagem</div>
<div class="service-item">Análises Clínicas</div>
<div class="service-item">Medicina Dentária</div>
<div class="service-item">Implantologia</div>
<div class="service-item">Ortodontia</div>

</div>

</div>

</div>


<div class="unit-card">

<div class="unit-header">
Varandas da Saúde
</div>

<div class="unit-content">

<p>Serviços especializados em saúde ocupacional e exames médicos.</p>

<div class="services-grid">

<div class="service-item">Medicina do Trabalho</div>
<div class="service-item">Exames Ocupacionais</div>
<div class="service-item">Consultas Ocupacionais</div>
<div class="service-item">Exames Empresas</div>
<div class="service-item">Recibos Verdes</div>
<div class="service-item">Avaliações de Risco</div>

</div>

</div>

</div>


<div class="unit-card">

<div class="unit-header">
Prevent Control
</div>

<div class="unit-content">

<p>Soluções completas de higiene, segurança alimentar e controlo de pragas.</p>

<div class="services-grid">

<div class="service-item">Higiene e Segurança</div>
<div class="service-item">Implementação HACCP</div>
<div class="service-item">Controlo de Pragas</div>
<div class="service-item">Consultoria Alimentar</div>
<div class="service-item">Auditorias</div>
<div class="service-item">Planos de Prevenção</div>

</div>

</div>

</div>


</div>

</section>


<section id="map-section">

<h2>A Nossa Localização</h2>

<iframe
id="map"
src="https://www.google.com/maps?q=Rua+da+Bandeira+435+Viana+do+Castelo&output=embed"
loading="lazy">
</iframe>

</section>


<footer id="contatos">

<div class="footer-grid">

<div class="footer-col">

<h4>Contacto Geral</h4>

<p><i class="fas fa-phone"></i> 258 838 011</p>

<p><i class="fas fa-mobile-alt"></i> 934 579 140</p>

<p>
<i class="fas fa-envelope"></i>
<a href="mailto:geral@varandasdasaude.pt">
geral@varandasdasaude.pt
</a>
</p>

</div>


<div class="footer-col">

<h4>Morada</h4>

<p>Rua da Bandeira 435</p>

<p>4900-560 Viana do Castelo</p>

<p>Portugal</p>

</div>


<div class="footer-col">

<h4>Horário</h4>

<p>Clínica da Bandeira: 09:00 – 18:30</p>

<p>Varandas da Saúde: 09:00 – 19:00</p>

<p>Prevent Control: 09:00 – 18:30</p>

<p>Segunda a Sexta</p>

</div>

</div>


<div class="social-section">

<h4>Redes Sociais do Grupo</h4>

<div class="social-group">


<div class="social-unit">

<h5>Clínica da Bandeira</h5>

<div class="social-icons">

<a href="https://www.facebook.com/clinicadabandeira" target="_blank" aria-label="Facebook">

<i class="fab fa-facebook-f"></i>

</a>

<a href="https://www.instagram.com/clinicadabandeira" target="_blank" aria-label="Instagram">

<i class="fab fa-instagram"></i>

</a>

</div>

</div>


<div class="social-unit">

<h5>Varandas da Saúde</h5>

<div class="social-icons">

<a href="https://www.facebook.com/varandasdasaude/" target="_blank">

<i class="fab fa-facebook-f"></i>

</a>

<a href="https://www.instagram.com/varandasdasaude/" target="_blank">

<i class="fab fa-instagram"></i>

</a>

</div>

</div>


<div class="social-unit">

<h5>Prevent Control</h5>

<div class="social-icons">

<a href="https://www.facebook.com/AJpreventcontrol/" target="_blank">

<i class="fab fa-facebook-f"></i>

</a>

<a href="https://www.instagram.com/preventcontrol_" target="_blank">

<i class="fab fa-instagram"></i>

</a>

<a href="https://www.linkedin.com/in/a-j-shst-05636b53/" target="_blank">

<i class="fab fa-linkedin-in"></i>

</a>

</div>

</div>

</div>

</div>


<div class="copyright">

© 2026 Grupo Varandas da Saúde — Todos os direitos reservados

</div>

</footer>

</body>
</html>
