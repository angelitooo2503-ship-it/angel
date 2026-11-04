[index.html](https://github.com/user-attachments/files/34396122/index.html)
# angel<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BMW MOTORRAD NEWS</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@800;900&family=Open+Sans:wght@400;700&display=swap" rel="stylesheet">
<style>
:root{ --azul:#0066B1; --rojo:#E30613; --titulo:'Playfair Display', serif; --texto:'Open Sans', sans-serif; }
*{margin:0; padding:0; box-sizing:border-box;}
body{font-family:var(--texto); background:#0a1931;}

/* CABECERA BMW AZUL CON ROJO */
.cabecera{
  background: linear-gradient(90deg, var(--azul) 0%, #004a8a 70%, var(--rojo) 100%);
  color:white; text-align:center; padding:18px; border-bottom:4px solid var(--rojo);
}
.fecha{font-size:11px; text-align:left; max-width:1100px; margin:0 auto 5px; opacity:.9;}
.logo{font-family:var(--titulo); font-size:48px; font-weight:900; letter-spacing:2px;}
.logo span{color:white; background:var(--rojo); padding:0 10px; border-radius:4px; margin-left:5px;}
.sublogo{letter-spacing:8px; font-size:10px; margin-top:5px;}
nav{display:flex; justify-content:center; gap:25px; margin-top:12px; border-top:1px solid rgba(255,255,255,.3); padding-top:10px;}
nav a{color:white; text-decoration:none; font-weight:700; font-size:12px; letter-spacing:1px;}

.periodico{max-width:1100px; margin:20px auto; background:white; padding:20px; border-left:6px solid var(--azul); border-right:6px solid var(--rojo);}

/* PRINCIPAL */
.principal{display:grid; grid-template-columns:1.3fr .7fr; gap:20px; border-bottom:3px solid black; padding-bottom:20px;}
.etiqueta{background:var(--rojo); color:white; padding:5px 12px; font-size:11px; font-weight:bold; animation:pulso 2s infinite;}
.texto h2{font-family:var(--titulo); font-size:34px; line-height:1.05; margin:10px 0; color:#0a1931;}
.texto p{color:#333; line-height:1.5;}
.img-principal{height:330px; overflow:hidden; border-radius:6px; border:3px solid var(--azul);}
.img-principal img{width:100%; height:100%; object-fit:cover; filter:blur(8px); animation:enfocar 1.2s ease forwards;}

.secundarias{display:grid; grid-template-columns:repeat(3,1fr); gap:18px; margin-top:20px; border-bottom:3px solid var(--azul); padding-bottom:20px;}
.img-box{height:190px; overflow:hidden; position:relative; border:2px solid var(--azul);}
.img-box img{width:100%; height:100%; object-fit:cover; transition:.5s;}
.img-box::before{content:""; position:absolute; inset:0; background:var(--azul); transform:scaleX(0); transform-origin:left; transition:.6s; mix-blend-mode:multiply; z-index:1;}
.img-box:hover::before{transform:scaleX(1);}
.nota h3{font-family:var(--titulo); font-size:16px; margin:10px 0; color:#0a1931;}
.nota p{font-size:12px; color:#555;}

/* FLIP SECCIONES - SOLO BMW */
.titulo-seccion{font-family:var(--titulo); font-size:22px; margin:25px 0 15px; color:var(--azul); border-left:5px solid var(--rojo); padding-left:10px;}
.secciones-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:15px;}
.flip-card{height:220px; perspective:1000px; cursor:pointer;}
.flip-inner{position:relative; width:100%; height:100%; transition:transform .8s; transform-style:preserve-3d;}
.flip-card:hover .flip-inner{transform:rotateY(180deg);}
.flip-front, .flip-back{position:absolute; width:100%; height:100%; backface-visibility:hidden; border-radius:10px; overflow:hidden; display:flex; align-items:center; justify-content:center; font-weight:bold; border:2px solid var(--azul);}
.flip-front img, .flip-back img{width:100%; height:100%; object-fit:cover;}
.flip-back{transform:rotateY(180deg); background:var(--azul); color:white; flex-direction:column; text-align:center; padding:10px;}
.verde{background:var(--azul); color:white; font-size:24px;}
.rojo-card{background:var(--rojo); color:white;}

@keyframes enfocar{to{filter:blur(0);}}
@keyframes pulso{0%,100%{transform:scale(1);} 50%{transform:scale(1.05);}}
footer{background:linear-gradient(90deg, var(--azul), var(--rojo)); color:white; text-align:center; padding:15px; font-size:11px; margin-top:20px;}
@media(max-width:800px){.principal{grid-template-columns:1fr;} .secundarias{grid-template-columns:1fr;} .secciones-grid{grid-template-columns:1fr 1fr;}}
</style>
</head>
<body>

<header class="cabecera">
  <div class="fecha">Miércoles 14 de Octubre 2026 | Edición Especial BMW Motorrad</div>
  <h1 class="logo">BMW MOTORRAD<span>NEWS</span></h1>
  <p class="sublogo">AZUL • MORADO • ROJO • MAKE LIFE A RIDE</p>
  <nav><a href="#">R 1300 GS</a><a href="#">S 1000 RR</a><a href="#">M 1000 R</a><a href="#">CE 04</a><a href="#">F 900</a></nav>
</header>

<main class="periodico">
  <section class="principal">
    <div class="texto">
      <span class="etiqueta">BMW EXCLUSIVA</span>
      <h2>BMW R 1300 GS Adventure 2026: 145 HP y frena sola con radar</h2>
      <p>La nueva GS con radar, suspensión inteligente y 30 litros de tanque fue presentada en México. La versión Adventure promete cruzar todo el país sin parar. Desde $489,900 MXN.</p>
    </div>
    <div class="img-principal">
      <img src="https://images.unsplash.com/photo-1558981806-ec527fa84c39?w=800" alt="BMW R1300GS">
    </div>
  </section>

  <div class="secundarias">
    <article class="nota">
      <div class="img-box"><img src="https://www.bmw-motorrad.com.mx/content/dam/bmwmotorradnsc/common/images/models/modeloverview/2024/nsc-s1000rr-P0N3H-modeloverview-600x360.jpg.asset.1739785597262.jpg" alt="BMW S1000RR"></div>
      <h3>BMW S 1000 RR 2026: 210 HP y 0-100 en 3.1s</h3>
      <p>La super deportiva con alerones M llega con control de tracción de 7 niveles.</p>
    </article>
    <article class="nota">
      <div class="img-box"><img src="https://images.unsplash.com/photo-1558981852-426c6c22a060?w=500" alt="BMW GS"></div>
      <h3>BMW F 900 GS: La mediana más vendida</h3>
      <p>Con 105 HP, es la favorita de Tecámac para ruta y ciudad.</p>
    </article>
    <article class="nota">
      <div class="img-box"><img src="https://cdn.motor1.com/images/mgl/lE78l6/1116:0:2827:2827/prueba-bmw-ce-04.webp" alt="BMW R nineT"></div>
      <h3>BMW CE 04: La eléctrica que parece del futuro</h3>
      <p>130 km de autonomía, carga rápida y diseño sci-fi. Ya en agencias BMW.</p>
    </article>
  </div>

  <h2 class="titulo-seccion">secciones - voltea para ver la moto</h2>
  <div class="secciones-grid">
    <div class="flip-card"><div class="flip-inner"><div class="flip-front verde">Front<br>R1300</div><div class="flip-back"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNu-diItn6yps2VeHJK3V6wLMxieSxyItBOxpIevtMPUukXdQJusld8-SW&s=10" alt="BMW"></div></div></div>
    <div class="flip-card"><div class="flip-inner"><div class="flip-front"><img src="https://www.bmw-motorrad.com.mx/content/dam/bmwmotorradnsc/common/images/models/modeloverview/2024/nsc-s1000rr-P0N3H-modeloverview-600x360.jpg.asset.1739785597262.jpg"></div><div class="flip-back rojo-card">S 1000 RR<br>Back - 210 HP</div></div></div>
    <div class="flip-card"><div class="flip-inner"><div class="flip-front" style="background:#e9e3d1; color:#0a1931; padding:15px; font-size:13px;">Pasa el mouse<br><b>atrás hay BMW</b></div><div class="flip-back"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuYzhfDaX-sIy8D5-f6hWFBjpR1CRDs-kIYXU1eWep8A&s=10" alt="BMW GS"></div></div></div>
    <div class="flip-card"><div class="flip-inner"><div class="flip-front"><img src="hhttps://cdn.motor1.com/images/mgl/lE78l6/1116:0:2827:2827/prueba-bmw-ce-04.webp" alt="BMW R nineT"></div><div class="flip-back verde">Front<br>CE 04</div></div></div>
    <div class="flip-card"><div class="flip-inner"><div class="flip-front" style="background:#0a1931; color:white; font-size:16px;">Sección 6 - Texto<br><b>BMW M 1000 RR</b></div><div class="flip-back rojo-card">M 1000 RR<br>Edición M - $650k</div></div></div>
    <div class="flip-card"><div class="flip-inner"><div class="flip-front"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXv_zxzs3zK1NgbQwjHA4AESz_byquYZaOBhmJFJoXQw&s" alt="BMW"></div></div></div>
  </div>
</main>

<footer>BMW MOTORRAD NEWS | Estilo Azul + Rojo M | Fotos reales BMW Motorrad | Efecto Front/Back | 2 Tipografías: Playfair Display + Open Sans</footer>
</body>
</html>
