<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cineplay TV</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;max-width:100%}
html,body{overflow-x:hidden;font-family:Arial;background:#0b0b0b;color:#fff;text-align:center}

.header{background:#7b2cff;padding:12px;font-weight:bold}

.banner{
background:url('https://images.unsplash.com/photo-1524985069026-dd778a71c7b4?q=80&w=1200&auto=format&fit=crop') center/cover no-repeat;
padding:70px 20px;
}

.overlay{background:rgba(0,0,0,0.7);padding:30px;border-radius:10px}

.container{padding:20px}

.btn{
display:block;margin:12px auto;padding:15px;background:#ff2d2d;color:#fff;
text-decoration:none;border-radius:12px;width:90%;max-width:320px;
font-weight:bold;animation:pulsar 1.5s infinite;
}

/* ===== PLANOS ===== */
.planos-container{
display:flex;
overflow-x:auto;
gap:15px;
padding:10px 20px;
scroll-snap-type:x mandatory;
}
.planos-container::-webkit-scrollbar{display:none}

.planos-bg{
background:
linear-gradient(to bottom, rgba(11,11,11,0.9), rgba(11,11,11,1)),
url('https://images.unsplash.com/photo-1606813907291-d86efa9b94db?q=80&w=1200&auto=format&fit=crop') center/cover no-repeat;
padding:30px 10px;
border-radius:20px;
margin:20px 0;
}

/* ===== CARDS ===== */
.card{
min-width:260px;
flex:0 0 auto;
scroll-snap-align:center;
background:rgba(20,20,20,0.85);
backdrop-filter:blur(10px);
border:1px solid rgba(255,255,255,0.05);
box-shadow:0 0 20px rgba(0,0,0,0.6);
margin:15px auto;
padding:20px;
border-radius:15px;
max-width:350px;
}

.highlight{border:2px solid #7b2cff}

.price{font-size:22px;color:#7b2cff;margin:10px 0}

/* ===== SETAS ===== */
.setas{
display:flex;
justify-content:center;
gap:15px;
margin-bottom:10px;
}

.setas button{
background:#7b2cff;
border:none;
color:#fff;
padding:10px 15px;
border-radius:10px;
font-size:18px;
cursor:pointer;
}

/* ===== AVALIAÇÕES ===== */
.reviews-box{
background:#0f0f0f;
padding:20px;
border-radius:15px;
margin-top:20px;
}

.review{
background:#121212;
padding:12px;
margin:10px auto;
border-radius:12px;
max-width:320px;
display:flex;
align-items:center;
gap:10px;
border:1px solid rgba(255,255,255,0.05);
}

.review img{
width:32px;
height:32px;
border-radius:50%;
object-fit:cover;
}

.review p{
font-size:13px;
text-align:left;
}

.footer{margin-top:30px;padding:20px;font-size:14px;color:#aaa}

@keyframes pulsar{
0%{transform:scale(1)}
50%{transform:scale(1.08)}
100%{transform:scale(1)}
}
</style>
</head>

<body>

<div class="header">
🔥 OFERTA LIMITADA TERMINA EM <span id="timer"></span>
<p style="color:red;">⚠️ Restam poucas vagas hoje</p>
</div>

<div class="banner">
<div class="overlay">

<img src="https://i.postimg.cc/8cS7DbFT/1000392886-removebg-preview.png" style="width:180px;">

<h2 style="color:#ff4444;">
🔥 Tenha acesso a milhares de conteúdos pagando muito menos
</h2>

<p>
🎬 +100 MIL conteúdos liberados<br>
📺 Canais ao vivo + Premiere + Telecine<br>
⚡ Sem travar | HD/FULL HD
</p>

<a class="btn" href="https://wa.me/5582996062108?text=Quero%20teste%20gratis%20agora">
🔥 TESTE GRÁTIS AGORA
</a>

<a class="btn" href="https://aftv.news/1072646">
📲 BAIXAR APLICATIVO
</a>

</div>
</div>

<div class="container">

<!-- PIX -->
<h2>💰 Pagamento via Pix</h2>

<div style="background:#111;padding:15px;border-radius:10px;margin:15px;">
<p><b>3c3a8735-4475-4340-8090-649f95432cfa</b></p>

<button class="btn" onclick="copiarPix()">📋 Copiar chave Pix</button>

<a class="btn" href="https://wa.me/5582996062108?text=Já%20fiz%20o%20pagamento%20via%20Pix">
📲 Enviar comprovante
</a>
</div>

<!-- PLANOS MENSAIS -->
<div class="planos-bg">
<h2>💰 Planos Mensais</h2>

<p style="font-size:13px;color:#aaa;">👉 Arraste para o lado para ver mais planos</p>

<div class="setas">
<button onclick="scrollPlanos(this,-1)">⬅️</button>
<button onclick="scrollPlanos(this,1)">➡️</button>
</div>

<div class="planos-container">

<div class="card">
<h3>1 Tela</h3>
<div class="price">R$ 24,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%201%20tela">Assinar</a>
</div>

<div class="card highlight">
<h3>2 Telas ⭐ Mais Vendido</h3>
<div class="price">R$ 34,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%202%20telas">Assinar</a>
</div>

<div class="card">
<h3>3 Telas</h3>
<div class="price">R$ 39,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%203%20telas">Assinar</a>
</div>

</div>
</div>

<!-- PLANOS ANUAIS -->
<div class="planos-bg">
<h2>🔥 Planos Anuais</h2>

<p style="font-size:13px;color:#aaa;">👉 Arraste para o lado para ver mais planos</p>

<div class="setas">
<button onclick="scrollPlanos(this,-1)">⬅️</button>
<button onclick="scrollPlanos(this,1)">➡️</button>
</div>

<div class="planos-container">

<div class="card">
<h3>1 Tela</h3>
<div class="price">R$ 179,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%201%20tela">Assinar</a>
</div>

<div class="card highlight">
<h3>2 Telas ⭐ Melhor Custo</h3>
<div class="price">R$ 229,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%202%20telas">Assinar</a>
</div>

<div class="card">
<h3>3 Telas</h3>
<div class="price">R$ 264,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%203%20telas">Assinar</a>
</div>

</div>
</div>

<!-- AVALIAÇÕES -->
<div class="reviews-box">

<h2>⭐ Avaliações</h2>
<p style="color:#aaa;font-size:13px;margin-top:5px;">+187 pessoas já avaliaram</p>

<div class="review">
<img src="https://randomuser.me/api/portraits/men/32.jpg">
<p>Até agora tá rodando bem aqui 👍</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/women/45.jpg">
<p>Uso mais à noite e não travou ainda</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/men/12.jpg">
<p>Instalei rápido, foi tranquilo</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/women/22.jpg">
<p>Pelo preço vale a pena sim</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/men/55.jpg">
<p>Tem bastante coisa, tô testando ainda</p>
</div>

</div>

</div>

<script>
function copiarPix(){
navigator.clipboard.writeText("3c3a8735-4475-4340-8090-649f95432cfa");
alert("Chave Pix copiada!");
}

function scrollPlanos(btn, dir){
const container = btn.parentElement.nextElementSibling;
container.scrollBy({
left: dir * 280,
behavior: 'smooth'
});
}

let time=600;
setInterval(()=>{
let m=Math.floor(time/60);
let s=time%60;
document.getElementById('timer').innerHTML=m+":"+(s<10?'0':'')+s;
time--;
if(time<0) time=600;
},1000);
</script>

</body>
</html>
