# signalteckweb
<!doctype html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Signalteck — Cambio de pantalla a domicilio en Bogotá</title>
<meta name="description" content="Cambio de pantalla para celulares en Bogotá. Domicilio GRATIS hasta 25 km. Gama baja y media con instalación y mantenimiento gratis por lanzamiento. Gama alta OEM con laboratorio técnico y anticipo 50% no reembolsable. Nequi, Daviplata y efectivo.">
<meta property="og:title" content="Signalteck — Cambio de pantalla a domicilio en Bogotá">
<meta property="og:description" content="Domicilio GRATIS ≤25 km. Envío nacional a cargo del cliente (Servientrega/Inter Rapidísimo).">
<meta property="og:type" content="website">
<meta property="og:locale" content="es_CO">
<meta name="theme-color" content="#2563EB">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
:root{
--primary: #2563EB;
--primary-dark: #1d4ed8;
--secondary: #06B6D4;
--accent: #10B981;
--accent-dark: #059669;
--text: #111827;
--text-light: #6B7280;
--muted: #374151;
--bg: #F9FAFB;
--white: #ffffff;
--border: #E5E7EB;
--success-bg: #ECFDF5;
--success-text: #065F46;
--warning-bg: #FEF3C7;
--warning-text: #92400E;
--shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
}

* {
box-sizing: border-box;
margin: 0;
padding: 0;
}

body {
font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
color: var(--text);
background: var(--bg);
line-height: 1.6;
}

/* Navegación */
header {
position: sticky;
top: 0;
background: var(--white);
box-shadow: var(--shadow);
z-index: 50;
backdrop-filter: blur(8px);
}

.container {
max-width: 1200px;
margin: 0 auto;
padding: 0 20px;
}

.nav {
display: flex;
align-items: center;
justify-content: space-between;
height: 70px;
}

.logo {
display: flex;
align-items: center;
gap: 12px;
font-weight: 800;
font-size: 24px;
color: var(--primary);
}

.logo::before {
content: "📱";
font-size: 28px;
}

.nav-links {
display: flex;
gap: 32px;
}

.nav-links a {
color: var(--muted);
text-decoration: none;
font-weight: 500;
transition: color 0.3s ease;
}

.nav-links a:hover {
color: var(--primary);
}

/* Menú móvil */
.mobile-menu-btn {
display: none;
background: none;
border: none;
font-size: 24px;
cursor: pointer;
color: var(--text);
}

.mobile-nav {
display: none;
position: absolute;
top: 70px;
left: 0;
right: 0;
background: var(--white);
box-shadow: var(--shadow-lg);
padding: 20px;
}

.mobile-nav.active {
display: block;
}

.mobile-nav a {
display: block;
padding: 12px 0;
color: var(--muted);
text-decoration: none;
border-bottom: 1px solid var(--border);
}

/* Hero Section */
.hero {
background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
color: var(--white);
padding: 80px 0;
position: relative;
overflow: hidden;
}

.hero::before {
content: '';
position: absolute;
top: 0;
left: 0;
right: 0;
bottom: 0;
background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.05'%3E%3Ccircle cx='30' cy='30' r='4'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E") repeat;
}

.hero-content {
position: relative;
z-index: 2;
max-width: 800px;
}

.hero h1 {
font-size: 48px;
font-weight: 800;
margin-bottom: 20px;
line-height: 1.2;
}

.hero p {
font-size: 20px;
margin-bottom: 32px;
opacity: 0.95;
}

.cta {
display: flex;
gap: 16px;
flex-wrap: wrap;
}

.btn {
display: inline-flex;
align-items: center;
gap: 8px;
background: var(--accent);
color: var(--success-text);
padding: 16px 28px;
border-radius: 12px;
font-weight: 700;
text-decoration: none;
transition: all 0.3s ease;
box-shadow: var(--shadow);
}

.btn:hover {
background: var(--accent-dark);
transform: translateY(-2px);
box-shadow: var(--shadow-lg);
}

.btn-secondary {
background: var(--white);
color: var(--primary);
}

.btn-secondary:hover {
background: #f8fafc;
color: var(--primary-dark);
}

/* Secciones */
.section {
padding: 80px 0;
}

.section h2 {
font-size: 36px;
font-weight: 800;
margin-bottom: 48px;
text-align: center;
color: var(--text);
}

/* Grid de cards */
.grid {
display: grid;
gap: 32px;
}

.cards {
grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
}

.card {
background: var(--white);
border-radius: 20px;
box-shadow: var(--shadow);
padding: 32px;
transition: all 0.3s ease;
border: 1px solid var(--border);
}

.card:hover {
transform: translateY(-4px);
box-shadow: var(--shadow-lg);
}

.badge {
display: inline-block;
background: var(--success-bg);
color: var(--success-text);
padding: 8px 16px;
border-radius: 50px;
font-size: 12px;
font-weight: 700;
margin-bottom: 16px;
text-transform: uppercase;
letter-spacing: 0.5px;
}

.badge.premium {
background: var(--warning-bg);
color: var(--warning-text);
}

.card h3 {
font-size: 24px;
font-weight: 700;
margin-bottom: 16px;
color: var(--text);
}

.price {
font-size: 32px;
font-weight: 800;
color: var(--primary);
margin-bottom: 24px;
}

.list {
list-style: none;
margin-bottom: 32px;
}

.list li {
padding: 8px 0;
position: relative;
padding-left: 28px;
color: var(--muted);
}

.list li::before {
content: "✓";
position: absolute;
left: 0;
color: var(--accent);
font-weight: bold;
}

/* Utilidades */
.two-cols {
grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
}

.success {
background: var(--success-bg);
color: var(--success-text);
padding: 24px;
border-radius: 12px;
border-left: 4px solid var(--accent);
}

.warning {
background: var(--warning-bg);
color: var(--warning-text);
padding: 24px;
border-radius: 12px;
border-left: 4px solid #F59E0B;
}

.small {
font-size: 14px;
color: var(--text-light);
line-height: 1.5;
}

.kicker {
color: var(--primary);
font-weight: 700;
}

/* FAQ Accordion */
.faq-item {
background: var(--white);
border-radius: 12px;
margin-bottom: 16px;
overflow: hidden;
box-shadow: var(--shadow);
}

.faq-question {
padding: 24px;
background: none;
border: none;
width: 100%;
text-align: left;
font-weight: 600;
font-size: 16px;
cursor: pointer;
display: flex;
justify-content: space-between;
align-items: center;
color: var(--text);
}

.faq-question:hover {
background: var(--bg);
}

.faq-answer {
padding: 0 24px 24px;
color: var(--muted);
display: none;
}

.faq-item.active .faq-answer {
display: block;
}

/* Footer */
footer {
background: var(--text);
color: var(--white);
padding: 48px 0 24px;
margin-top: 80px;
}

.footer-content {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
gap: 48px;
margin-bottom: 32px;
}

.footer-section h3 {
font-weight: 700;
margin-bottom: 16px;
}

.footer-section a {
color: rgba(255, 255, 255, 0.8);
text-decoration: none;
display: block;
margin-bottom: 8px;
transition: color 0.3s ease;
}

.footer-section a:hover {
color: var(--white);
}

.footer-bottom {
border-top: 1px solid rgba(255, 255, 255, 0.1);
padding-top: 24px;
text-align: center;
color: rgba(255, 255, 255, 0.6);
}

/* Responsive */
@media (max-width: 768px) {
.nav-links {
display: none;
}

.mobile-menu-btn {
display: block;
}

.hero {
padding: 60px 0;
}

.hero h1 {
font-size: 36px;
}

.hero p {
font-size: 18px;
}

.section {
padding: 60px 0;
}

.section h2 {
font-size: 28px;
}

.cards {
grid-template-columns: 1fr;
}

.two-cols {
grid-template-columns: 1fr;
}

.container {
padding: 0 16px;
}

.cta {
justify-content: center;
}
}

@media (max-width: 480px) {
.hero h1 {
font-size: 28px;
}

.card {
padding: 24px;
}

.price {
font-size: 28px;
}
}

/* Animaciones */
@keyframes fadeInUp {
from {
opacity: 0;
transform: translateY(30px);
}
to {
opacity: 1;
transform: translateY(0);
}
}

.card {
animation: fadeInUp 0.6s ease forwards;
}

.card:nth-child(2) {
animation-delay: 0.1s;
}

.card:nth-child(3) {
animation-delay: 0.2s;
}

/* Botón WhatsApp flotante */
.whatsapp-float {
position: fixed;
bottom: 24px;
right: 24px;
background: #25D366;
color: white;
border-radius: 50px;
padding: 16px 24px;
text-decoration: none;
font-weight: 700;
box-shadow: var(--shadow-lg);
z-index: 100;
transition: all 0.3s ease;
display: flex;
align-items: center;
gap: 8px;
}

.whatsapp-float:hover {
transform: scale(1.05);
background: #128C7E;
}
</style>
</head>
<body>
<header>
<div class="container">
<nav class="nav">
<div class="logo">Signalteck</div>
<div class="nav-links">
<a href="#precios">Precios</a>
<a href="#cobertura">Cobertura</a>
<a href="#como-funciona">Proceso</a>
<a href="#contacto">Contacto</a>
<a href="#faq">FAQ</a>
</div>
<button class="mobile-menu-btn" onclick="toggleMobileMenu()">☰</button>
</nav>
<div class="mobile-nav" id="mobileNav">
<a href="#precios" onclick="closeMobileMenu()">Precios</a>
<a href="#cobertura" onclick="closeMobileMenu()">Cobertura</a>
<a href="#como-funciona" onclick="closeMobileMenu()">Proceso</a>
<a href="#contacto" onclick="closeMobileMenu()">Contacto</a>
<a href="#faq" onclick="closeMobileMenu()">FAQ</a>
</div>
</div>
</header>

<section class="hero">
<div class="container">
<div class="hero-content">
<h1>Cambio de pantalla a domicilio en Bogotá</h1>
<p>Domicilio GRATIS hasta 25 km. Gama baja y media con instalación y mantenimiento GRATIS por lanzamiento. Pagos: Nequi, Daviplata y efectivo.</p>
<div class="cta">
<a class="btn" href="https://wa.me/573243115342?text=Hola%20Signalteck,%20quiero%20agendar%20cambio%20de%20pantalla.%20Mi%20marca/modelo:%20____.%20Dirección:%20____.%20Franja%20preferida:%20____." target="_blank" rel="noopener">
📱 Agendar WhatsApp
</a>
<a class="btn btn-secondary" href="tel:+573243115342">
📞 Llamar ahora
</a>
</div>
</div>
</div>
</section>

<section id="precios" class="section">
<div class="container">
<h2>Precios y Servicios</h2>
<div class="grid cards">
<div class="card">
<div class="badge">PROMO LANZAMIENTO</div>
<h3>Gama Baja</h3>
<div class="price">$120.000</div>
<ul class="list">
<li>Instalación incluida</li>
<li>Mantenimiento preventivo incluido</li>
<li>Domicilio GRATIS ≤ 25 km</li>
<li>Tiempo estimado: 60 min</li>
<li>Garantía completa</li>
</ul>
<div class="small">Cobertura: Bogotá y alrededores. Envío nacional: a cargo del cliente.</div>
<br>
<a class="btn" href="https://wa.me/573243115342?text=Hola%20Signalteck,%20gama%20baja%20$120.000.%20Marca/modelo:%20____.%20Dirección:%20____.%20Franja:%20____." target="_blank" rel="noopener">Agendar Gama Baja</a>
</div>

<div class="card">
<div class="badge">PROMO LANZAMIENTO</div>
<h3>Gama Media</h3>
<div class="price">$280.000</div>
<ul class="list">
<li>Con huella en pantalla</li>
<li>Instalación incluida</li>
<li>Mantenimiento preventivo incluido</li>
<li>Domicilio GRATIS ≤ 25 km</li>
<li>Tiempo estimado: 60-90 min</li>
<li>Garantía completa</li>
</ul>
<div class="small">Cobertura: Bogotá y alrededores. Envío nacional: a cargo del cliente.</div>
<br>
<a class="btn" href="https://wa.me/573243115342?text=Hola%20Signalteck,%20gama%20media%20$280.000.%20Marca/modelo:%20____.%20Dirección:%20____.%20Franja:%20____." target="_blank" rel="noopener">Agendar Gama Media</a>
</div>

<div class="card">
<div class="badge premium">LABORATORIO TÉCNICO ESPECIALIZADO</div>
<h3>Gama Alta OEM</h3>
<div class="price">$1.100.000</div>
<ul class="list">
<li>Display original certificado (OEM)</li>
<li>Instalación profesional</li>
<li>Trabajo en laboratorio técnico: 2-4 días</li>
<li>Recogida y entrega GRATIS ≤ 25 km</li>
<li>Garantía del fabricante</li>
</ul>
<div class="warning">
<strong>Importante:</strong> Anticipo del 50% NO reembolsable para pedido del repuesto original. Consulta instalación con el ingeniero.
</div>
<br>
<a class="btn" href="https://wa.me/573243115342?text=Hola%20ingeniero,%20quiero%20cotizar%20gama%20alta%20OEM.%20Marca/modelo:%20____.%20Solicito%20recogida%20en:%20____." target="_blank" rel="noopener">Cotizar con Ingeniero</a>
</div>
</div>
</div>
</section>

<section id="cobertura" class="section">
<div class="container">
<h2>Cobertura y Logística</h2>
<div class="grid two-cols">
<div>
<h3>🚛 Servicio Local</h3>
<p><span class="kicker">Bogotá y hasta 25 km:</span> Domicilio, recogida y entrega completamente GRATIS. Incluye hasta 2 intentos de visita sin costo adicional.</p>
<br>
<p><span class="kicker">Intentos adicionales:</span> Desde el tercer intento, coordina el costo con nuestro equipo de logística al <a href="tel:+573243115342">324 311 5342</a>.</p>
</div>
<div class="success">
<h3>💳 Métodos de Pago</h3>
<p><strong>Aceptamos:</strong> Nequi, Daviplata y efectivo.</p>
<div class="small">Para confirmar transferencias digitales, envía el comprobante por WhatsApp para procesar tu servicio más rápido.</div>
</div>
</div>
<br>
<div class="success">
<h3>📦 Envíos Nacionales</h3>
<p>Cubrimos todo Colombia mediante <strong>Servientrega</strong> e <strong>Inter Rapidísimo</strong>. El cliente gestiona y paga el envío, después comparte el número de guía por WhatsApp para hacer seguimiento.</p>
</div>
</div>
</section>

<section id="como-funciona" class="section">
<div class="container">
<h2>¿Cómo Funciona?</h2>
<div class="grid two-cols">
<div class="card">
<h3>🏠 Gama Baja y Media (Domicilio)</h3>
<ol style="padding-left: 20px; color: var(--muted);">
<li style="margin-bottom: 12px;"><strong>Contacto:</strong> Escríbenos por WhatsApp con marca y modelo de tu celular</li>
<li style="margin-bottom: 12px;"><strong>Agendamiento:</strong> Coordinamos domicilio dentro de la cobertura (≤ 25 km)</li>
<li style="margin-bottom: 12px;"><strong>Reparación:</strong> Llegamos a tu ubicación y reparamos en sitio (60-90 min)</li>
<li style="margin-bottom: 12px;"><strong>Pago:</strong> Cancelas con Nequi, Daviplata o efectivo y recibes tu garantía</li>
</ol>
</div>
<div class="card">
<h3>🔧 Gama Alta OEM (Laboratorio Técnico)</h3>
<ol style="padding-left: 20px; color: var(--muted);">
<li style="margin-bottom: 12px;"><strong>Recepción:</strong> Recogemos tu equipo GRATIS o lo recibes por envío</li>
<li style="margin-bottom: 12px;"><strong>Diagnóstico:</strong> Evaluamos y cotizamos instalación con el ingeniero</li>
<li style="margin-bottom: 12px;"><strong>Anticipo:</strong> 50% NO reembolsable para pedir repuesto original</li>
<li style="margin-bottom: 12px;"><strong>Entrega:</strong> Reparación completa en 2-4 días con pruebas y garantía</li>
</ol>
</div>
</div>
</div>
</section>

<section id="contacto" class="section">
<div class="container">
<h2>Contacto</h2>
<div class="grid two-cols">
<div class="card">
<h3>📍 Signalteck</h3>
<p><strong>Ubicación:</strong> Bogotá, Colombia</p>
<p><strong>Teléfono:</strong> <a href="tel:+573243115342">+57 324 311 5342</a></p>
<p><strong>WhatsApp:</strong> <a href="https://wa.me/573243115342" target="_blank">Escríbenos directamente</a></p>
<p><strong>Horarios:</strong> Lunes a Domingo</p>
</div>
<div class="success">
<h3>🚀 ¿Listo para reparar tu celular?</h3>
<p>Obtén tu cotización inmediata y agenda tu servicio en menos de 2 minutos.</p>
<br>
<a class="btn" href="https://wa.me/573243115342?text=Hola%20Signalteck,%20necesito%20cotización%20para%20cambio%20de%20pantalla.%20Mi%20equipo%20es:%20____" target="_blank">💬 Cotizar por WhatsApp</a>
</div>
</div>
</div>
</section>

<section id="faq" class="section">
<div class="container">
<h2>Preguntas Frecuentes</h2>
<div class="faq-item">
<button class="faq-question" onclick="toggleFaq(this)">
¿Qué incluye la promoción de lanzamiento? <span>+</span>
</button>
<div class="faq-answer">
En gamas baja y media incluye: instalación profesional, mantenimiento preventivo completo, domicilio GRATIS dentro de 25 km de Bogotá, y garantía sobre la pantalla y mano de obra.
</div>
</div>

<div class="faq-item">
<button class="faq-question" onclick="toggleFaq(this)">
¿Cuántos intentos de visita domiciliaria incluye? <span>+</span>
</button>
<div class="faq-answer">
Incluimos hasta 2 intentos de visita completamente gratis. Desde el tercer intento en adelante, se coordina una tarifa especial con nuestro equipo de logística al 324 311 5342.
</div>
</div>

<div class="faq-item">
<button class="faq-question" onclick="toggleFaq(this)">
¿Por qué la gama alta tarda más tiempo? <span>+</span>
</button>
<div class="faq-answer">
Los equipos de gama alta requieren repuestos originales OEM que debemos pedir especialmente. El proceso toma 2-4 días en nuestro laboratorio técnico para garantizar instalación perfecta. Requiere anticipo del 50% no reembolsable para pedido del repuesto.
</div>
</div>

<div class="faq-item">
<button class="faq-question" onclick="toggleFaq(this)">
¿Cómo funcionan los envíos nacionales? <span>+</span>
</button>
<div class="faq-answer">
El cliente gestiona y paga el envío con Servientrega o Inter Rapidísimo. Una vez enviado, compartes el número de guía por WhatsApp para hacer seguimiento del proceso de reparación.
</div>
</div>

<div class="faq-item">
<button class="faq-question" onclick="toggleFaq(this)">
¿Qué garantía ofrecen? <span>+</span>
</button>
<div class="faq-answer">
En gama baja y media: garantía completa sobre pantalla y mano de obra. En gama alta: garantía según especificaciones del repuesto OEM original y la instalación cotizada con el ingeniero.
</div>
</div>
</div>
</div>
</section>

<footer>
<div class="container">
<div class="footer-content">
<div class="footer-section">
<h3>Signalteck</h3>
<p>Especialistas en reparación de pantallas de celulares en Bogotá y toda Colombia.</p>
<br>
<p><strong>Tel/WhatsApp:</strong><br><a href="tel:+573243115342">+57 324 311 5342</a></p>
</div>
<div class="footer-section">
<h3>Servicios</h3>
<a href="#precios">Cambio de Pantalla</a>
<a href="#precios">Gama Baja - $120.000</a>
<a href="#precios">Gama Media - $280.000</a>
<a href="#precios">Gama Alta OEM</a>
</div>
<div class="footer-section">
<h3>Cobertura</h3>
<a href="#cobertura">Bogotá y 25 km</a>
<a href="#cobertura">Domicilio GRATIS</a>
<a href="#cobertura">Envíos Nacionales</a>
<a href="#contacto">Horarios</a>
</div>
<div class="footer-section">
<h3>Legal</h3>
<a href="#terminos">Términos del Servicio</a>
<a href="#privacidad">Política de Privacidad</a>
<a href="#garantias">Garantías</a>
</div>
</div>
<div class="footer-bottom">
<p>© 2024 Signalteck - Reparación de celulares en Bogotá, Colombia</p>
</div>
</div>
</footer>

<!-- WhatsApp flotante -->
<a href="https://wa.me/573243115342?text=Hola%20Signalteck,%20necesito%20información%20sobre%20cambio%20de%20pantalla" class="whatsapp-float" target="_blank" rel="noopener">
💬 WhatsApp
</a>

<script>
// Menú móvil
function toggleMobileMenu() {
const mobileNav = document.getElementById('mobileNav');
mobileNav.classList.toggle('active');
}

function closeMobileMenu() {
const mobileNav = document.getElementById('mobileNav');
mobileNav.classList.remove('active');
}

// FAQ Accordion
function toggleFaq(button) {
const faqItem = button.parentElement;
const isActive = faqItem.classList.contains('active');
const allFaqItems = document.querySelectorAll('.faq-item');

// Cerrar todos los items
allFaqItems.forEach(item => {
item.classList.remove('active');
item.querySelector('span').textContent = '+';
});

// Abrir el clickeado si no estaba activo
if (!isActive) {
faqItem.classList.add('active');
button.querySelector('span').textContent = '-';
}
}

// Smooth scroll para navegación
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
anchor.addEventListener('click', function (e) {
e.preventDefault();
const target = document.querySelector(this.getAttribute('href'));
if (target) {
target.scrollIntoView({
behavior: 'smooth',
block: 'start'
});
closeMobileMenu();
}
});
});

// Cerrar menú móvil al hacer click fuera
document.addEventListener('click', function(e) {
const mobileNav = document.getElementById('mobileNav');
const menuBtn = document.querySelector('.mobile-menu-btn');

if (!mobileNav.contains(e.target) && !menuBtn.contains(e.target)) {
mobileNav.classList.remove('active');
}
});
</script>

<script type="application/ld+json">
{
"@context":"https://schema.org",
"@type":"LocalBusiness",
"name":"Signalteck",
"description":"Reparación y cambio de pantallas de celulares en Bogotá y alrededores
