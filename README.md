<!DOCTYPE html>
<html lang="ru"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover"><title>Your Studio – брендинг, дизайн и контент для спорта</title><link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;700;800&display=swap" rel="stylesheet"><style id="css">
:root{
  --dark:#0A0A0A;--dark2:#171717;--line-d:#2A2A2A;--on-dark:#fff;--mute-d:#B5B5B5;
  --green:#2BE360;--green-ink:#06210F;
  --paper:#fff;--paper-ink:#0A0A0A;--paper-card:#F1F1F1;--paper-mute:#555;
  --f:"Manrope",system-ui,-apple-system,"Segoe UI",Arial,sans-serif;
  box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);color-scheme:light;
}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--paper:#101010;--paper-ink:#F4F4F4;--paper-card:#1B1B1B;--paper-mute:#A8A8A8;color-scheme:dark}}
:root[data-theme="dark"]{--paper:#101010;--paper-ink:#F4F4F4;--paper-card:#1B1B1B;--paper-mute:#A8A8A8;color-scheme:dark}
html{height:100%;scroll-padding-top:calc(env(safe-area-inset-top,0px) + 70px)}
*,*::before,*::after{box-sizing:border-box}
body{margin:0;min-height:100%;background:var(--paper);color:var(--paper-ink);font:400 16px/1.6 var(--f)}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--dark);z-index:20}
a{color:inherit}:focus-visible{outline:3px solid var(--green);outline-offset:3px}
.w{max-width:1200px;margin:0 auto;padding:0 clamp(16px,4vw,40px)}
h1,h2,h3{margin:0;line-height:1.1;font-weight:800}
h2{font-size:clamp(28px,4.4vw,48px);text-align:center;margin-bottom:28px}
.btn{display:inline-flex;align-items:center;gap:8px;background:var(--green);color:var(--green-ink);font:700 15px var(--f);padding:12px 22px;border-radius:8px;border:0;text-decoration:none;cursor:pointer}
.btn:hover{background:#fff}
.btn.o{background:transparent;color:#fff;border:1.5px solid #555}.btn.o:hover{border-color:var(--green);color:var(--green)}

/* header + hero */
header{position:sticky;top:env(safe-area-inset-top,0px);z-index:19;background:var(--dark);color:#fff}
.bar{display:flex;align-items:center;justify-content:space-between;height:60px;gap:12px}
.logo{font-weight:800;font-size:20px;letter-spacing:-.02em;text-decoration:none}
nav{display:flex;gap:22px;align-items:center}nav a{text-decoration:none;font-size:14px;font-weight:500;color:var(--mute-d)}nav a:hover{color:#fff}
nav .btn{color:var(--green-ink)}
@media(max-width:760px){nav a:not(.btn){display:none}}
.hero{background:var(--dark);color:#fff;overflow:hidden}
.hero .w{display:grid;grid-template-columns:1fr 1fr;gap:24px;align-items:center;min-height:560px}
.hero h1{font-size:clamp(34px,5.6vw,68px);margin-bottom:18px}
.hero p{color:var(--mute-d);max-width:42ch;margin:0 0 26px}
.cta-row{display:flex;gap:12px;flex-wrap:wrap}
.reel{display:flex;gap:12px;height:560px;-webkit-mask-image:linear-gradient(transparent,#000 12%,#000 88%,transparent);mask-image:linear-gradient(transparent,#000 12%,#000 88%,transparent)}
.col{flex:1;display:flex;flex-direction:column;gap:12px;animation:up 40s linear infinite}
.col.r{animation-direction:reverse;animation-duration:48s}
@keyframes up{to{transform:translateY(-50%)}}
.tile{aspect-ratio:3/4;border-radius:8px;overflow:hidden;position:relative;flex:none;background:linear-gradient(160deg,var(--a),var(--b));display:grid;place-items:end start;padding:12px;font-weight:800;font-size:20px;line-height:1.05}
.tile img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
@media(max-width:760px){.hero .w{grid-template-columns:1fr;padding-top:36px}.reel{height:340px}}

/* clients */
.sec{padding:clamp(44px,7vw,84px) 0}
.eyebrow{text-align:center;font-size:13px;font-weight:700;color:var(--paper-mute);margin-bottom:24px}
.logos{display:grid;grid-template-columns:repeat(auto-fill,minmax(110px,1fr));gap:14px}
.logo-s{height:64px;border:1.5px dashed color-mix(in srgb,var(--paper-ink) 25%,transparent);border-radius:8px;display:grid;place-items:center;font-size:13px;color:var(--paper-mute)}
.logo-s img{max-width:80%;max-height:70%}

/* problems + services */
.cards3{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,260px),1fr));gap:16px}
.q{background:var(--paper-card);border-radius:10px;padding:24px;font-weight:700;font-size:18px;line-height:1.35}
.lead{max-width:760px;margin:26px 0 22px;color:var(--paper-mute)}
.svc .cards3{grid-template-columns:repeat(auto-fit,minmax(min(100%,300px),1fr));gap:40px 16px}
.svc .media{aspect-ratio:4/3;border-radius:10px;overflow:hidden;position:relative;background:linear-gradient(135deg,var(--a),var(--b))}
.svc h3{font-size:22px;margin:16px 0 8px}.svc p{color:var(--paper-mute);margin:0 0 14px;font-size:15px}
.svc ul{list-style:none;margin:0;padding:0;display:grid;gap:8px;font-size:14.5px;font-weight:500}
.svc li{display:flex;gap:10px}.svc li::before{content:"";flex:none;width:16px;height:16px;margin-top:3px;border-radius:50%;background:var(--green) center/10px no-repeat url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 10 10'%3E%3Cpath d='M2 5.2l2 2L8 3' fill='none' stroke='%2306210F' stroke-width='1.6'/%3E%3C/svg%3E")}

/* dark showcase */
.show{background:var(--dark);color:#fff;border-radius:20px;margin:0 clamp(8px,2vw,24px);padding:clamp(36px,6vw,72px) 0}
.show h2{max-width:14ch;margin-left:auto;margin-right:auto}
.cases{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,420px),1fr));gap:24px}
.case .media{aspect-ratio:16/10;border-radius:10px;overflow:hidden;background:linear-gradient(135deg,var(--a),var(--b));position:relative;display:grid;place-items:center;font-weight:800;font-size:clamp(26px,4vw,44px);text-align:center;padding:16px}
.case h3{font-size:19px;margin:14px 0 6px}.case p{color:var(--mute-d);font-size:14.5px;margin:0 0 10px}
.tags{display:flex;flex-wrap:wrap;gap:6px;list-style:none;padding:0;margin:0}.tags li{font-size:12px;border:1px solid #444;border-radius:999px;padding:2px 10px;color:var(--mute-d)}
.more{text-align:center;margin:30px 0 40px}
.slider{max-width:760px;margin:0 auto;text-align:center;position:relative;padding:0 48px}
.slide{display:none}.slide.on{display:block}
.slide blockquote{margin:0 0 16px;font-weight:500;font-size:clamp(17px,2.2vw,21px);line-height:1.45}
.slide cite{font-style:normal;font-size:14px;color:var(--mute-d)}
.sb{position:absolute;top:30%;width:38px;height:38px;border-radius:50%;border:0;background:var(--green);color:var(--green-ink);font-size:18px;cursor:pointer}
.sb.p{left:0}.sb.n{right:0}
.dots{display:flex;gap:8px;justify-content:center;margin-top:20px}.dots button{width:9px;height:9px;border-radius:50%;border:0;background:#555;padding:0;cursor:pointer}.dots button[aria-current="true"]{background:var(--green)}
.news{margin:64px auto 0;max-width:1080px;display:grid;grid-template-columns:1fr 1fr;gap:28px;align-items:center;background:var(--dark2);border-radius:14px;padding:clamp(24px,4vw,44px);text-align:left}
.news h3{font-size:clamp(24px,3vw,34px);margin:8px 0 10px}.news p{margin:0;color:var(--mute-d);font-size:15px}.news .k{color:var(--green);font-weight:700;font-size:13px}
.news form{display:grid;gap:12px}.news input[type=email]{font:inherit;padding:13px 14px;border-radius:8px;border:1px solid #444;background:#fff;color:#111;width:100%}
.news small{color:var(--mute-d)}#msg{min-height:1.3em;font-weight:600;color:var(--green)}
@media(max-width:760px){.news{grid-template-columns:1fr}}

/* social + banner + footer */
.soc .q{display:flex;flex-direction:column;gap:8px;font-size:16px}.soc .q b{font-size:20px}.soc .q span{font-weight:400;color:var(--paper-mute);font-size:14.5px}.soc .q a{margin-top:6px;font-weight:700;text-decoration:none;color:var(--paper-ink)}
.banner{background:var(--dark);color:#fff;border-radius:16px;margin:0 clamp(8px,2vw,24px);overflow:hidden;display:grid;grid-template-columns:1fr 1fr}
.banner>div:first-child{padding:clamp(28px,5vw,56px)}.banner h2{text-align:left;font-size:clamp(28px,4vw,44px);margin-bottom:12px}.banner p{color:var(--mute-d);margin:0 0 22px}
.collage{min-height:280px;background:linear-gradient(135deg,#C6252B,#0B3D91 60%,#111);position:relative;display:grid;place-items:center;color:rgba(255,255,255,.7);font-weight:700}
@media(max-width:760px){.banner{grid-template-columns:1fr}}
footer{background:var(--dark);color:#fff;margin-top:24px;padding:32px 0 36px}
footer .w{display:flex;flex-wrap:wrap;gap:16px 28px;justify-content:space-between;align-items:center}
footer nav a{font-size:14px}footer small{width:100%;color:var(--mute-d);font-size:13px}
@media(prefers-reduced-motion:reduce){.col{animation:none}}

[data-img]{position:relative}
img.u{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
.logo-s img.u{object-fit:contain;padding:8px;max-width:none;max-height:none}
[data-img].has{color:transparent}
.ed [contenteditable]{outline:1px dashed var(--green);outline-offset:2px;cursor:text}
.ed [contenteditable]:focus{outline:2px solid var(--green);background:rgba(43,227,96,.14)}
.ed .col{animation:none}
.up{position:absolute;z-index:5;top:8px;right:8px;background:var(--green);color:var(--green-ink);border:0;border-radius:6px;font:700 12px var(--f);padding:6px 10px;cursor:pointer}
#bar{position:fixed;z-index:30;right:12px;bottom:calc(12px + env(safe-area-inset-bottom,0px));display:flex;flex-wrap:wrap;gap:8px;align-items:center;max-width:calc(100% - 24px);background:#111;color:#fff;padding:8px 10px;border-radius:12px;box-shadow:0 6px 24px rgba(0,0,0,.45);font:600 14px var(--f)}
#bar button{font:700 14px var(--f);border:0;border-radius:8px;padding:8px 14px;cursor:pointer;background:var(--green);color:var(--green-ink)}
#bar button.g{background:#333;color:#fff}
</style></head><body><div id="app"></div><template id="tpl"><header><div class="w bar">
  <a class="logo" href="#top">YOUR STUDIO</a>
  <nav aria-label="Основное"><a href="#top">Главная</a><a href="#services">Услуги</a><a href="#work">Наши работы</a><a href="#contact">О нас</a><a href="#news">Блог</a><a class="btn" href="#contact">Работайте с нами</a></nav>
</div></header>

<main id="top">
<div class="hero"><div class="w">
  <div>
    <h1>Брендинг, дизайн и контент для спорта</h1>
    <p>Спортивные организации доверяют нам разработку креативных решений, которые укрепляют бренд, привлекают болельщиков и увеличивают доход.</p>
    <div class="cta-row"><a class="btn" href="#work">Наша работа ↗</a><a class="btn o" href="#contact">О нас</a></div>
  </div>
  <div class="reel" id="reel" aria-hidden="true"></div>
</div></div>

<section class="sec"><div class="w">
  <div class="eyebrow">Объединяемся с чемпионами</div>
  <div class="logos" id="logos"></div>
</div></section>

<section class="sec" style="padding-top:0"><div class="w">
  <h2>Ваш бизнес сталкивается с этими проблемами?</h2>
  <div class="cards3">
    <div class="q">«Наш брендинг и креативная концепция отстают от конкурентов и лидеров отрасли».</div>
    <div class="q">«Нашу внутреннюю команду дизайнеров перегружают или ей не хватает специализированных навыков».</div>
    <div class="q">«Нам сложно использовать наш дизайнерский контент для получения дохода».</div>
  </div>
  <p class="lead">Мы сотрудничаем со спортивными организациями, которые хотят вывести свой бренд на новый уровень и улучшить креативную составляющую. Если ваша команда сталкивается с внутренними проблемами в дизайне, несоответствием бренда или трудностями в превращении контента в коммерческий успех, мы поможем.</p>
  <a class="btn" href="#contact">Решайте свои задачи ↗</a>
</div></section>

<section class="sec svc" id="services"><div class="w">
  <h2>Как мы можем вам помочь</h2>
  <div class="cards3">
    <article><div class="media" data-img="s0" style="--a:#1a7f37;--b:#ffd21f"></div><h3>Фирменный стиль и визуальная идентичность</h3><p>Независимо от того, начинаете ли вы с нуля или обновляете уже существующий дизайн, мы поможем создать яркий и гибкий визуальный язык.</p><ul><li>Позиционирование и направление бренда</li><li>Разработка логотипа и фирменного знака</li><li>Системы визуальной идентичности</li></ul></article>
    <article><div class="media" data-img="s1" style="--a:#2438ff;--b:#e4372b"></div><h3>Графика и анимация</h3><p>Выделитесь и повысьте вовлечённость аудитории на различных платформах с помощью захватывающих визуальных эффектов и контента для массовой аудитории.</p><ul><li>Статическая и анимированная графика на заказ</li><li>Шаблоны для соцсетей и наборы ресурсов</li><li>Визуальные материалы и ключевые изображения для кампаний</li></ul></article>
    <article><div class="media" data-img="s2" style="--a:#222;--b:#777"></div><h3>Видеосъёмка и монтаж</h3><p>Поднимите свой контент на новый уровень с помощью увлекательных видеороликов, основанных на сюжете. Мы поможем вам во всём: от стратегической поддержки до создания библиотеки коротких роликов.</p><ul><li>Короткометражный и брендовый видеоконтент</li><li>Кинематографическое повествование и режиссура</li><li>Компьютерная графика, визуальные эффекты и монтаж</li></ul></article>
    <article><div class="media" data-img="s3" style="--a:#0a1aa8;--b:#2be360"></div><h3>Дизайн по подписке</h3><p>Фиксированная ежемесячная плата вместо оплаты каждой задачи отдельно. У вас появляется своя дизайн-команда, которая всегда на связи и знает ваш бренд.</p><ul><li>Единая очередь задач и быстрые сроки</li><li>Постоянные дизайнеры, которые знают ваш стиль</li><li>Прозрачная стоимость на весь месяц</li></ul></article>
    <article><div class="media" data-img="s4" style="--a:#e4372b;--b:#ffd21f"></div><h3>Дизайн-сопровождение турнира</h3><p>Берём на себя весь визуал турнира от анонса до финального свистка, чтобы всё выглядело единым целым на экране, в соцсетях и на арене.</p><ul><li>Фирменный стиль и шаблоны под турнир</li><li>Афиши, экранная графика и контент на каждый матч</li><li>Наградные и итоговые материалы</li></ul></article>
    <article><div class="media" data-img="s5" style="--a:#111;--b:#7a2bff"></div><h3>Штучные услуги</h3><p>Нужна одна конкретная вещь, а не долгий проект? Сделаем разовую работу быстро и в нужном вам стиле, без обязательств на будущее.</p><ul><li>Презентации для партнёров и спонсоров</li><li>Постеры, афиши и баннеры</li><li>Другие разовые дизайн-задачи</li></ul></article>
  </div>
</div></section>

<section class="show" id="work"><div class="w">
  <h2>Ознакомьтесь с нашей работой в поддержку этих чемпионов.</h2>
  <div class="cases" id="cases"></div>
  <div class="more"><a class="btn" href="#work">Посмотреть больше</a></div>
  <div class="slider" id="slider">
    <button class="sb p" aria-label="Назад">‹</button><button class="sb n" aria-label="Вперёд">›</button>
    <div class="slide on"><blockquote>«Компания отреагировала невероятно оперативно и превзошла все ожидания. Я бы рекомендовал всем спортивным организациям обратиться к ним».</blockquote><cite>Имя Фамилия, должность, клиент</cite></div>
    <div class="slide"><blockquote>«Мы доверили им работу как специализированному агентству с сетью лучших креативных специалистов, которые помогают воплотить наши идеи».</blockquote><cite>Имя Фамилия, должность, клиент</cite></div>
    <div class="dots"></div>
  </div>
  <div class="news" id="news">
    <div><div class="k">Ваш еженедельный дайджест спортивного контента</div><h3>Станьте тем, кто изменит правила игры.</h3><p>Подпишитесь на рассылку и получайте идеи, инсайты индустрии и ресурсы, которые держат вас на шаг впереди.</p></div>
    <form id="form" novalidate><input type="email" id="email" placeholder="Введите ваш адрес электронной почты" aria-label="Электронная почта"><button class="btn" type="submit">Да, пожалуйста</button><small>Я согласен получать другие сообщения от Your Studio.</small><div id="msg" role="status"></div></form>
  </div>
</div></section>

<section class="sec soc"><div class="w">
  <h2>Будьте в курсе событий</h2>
  <div class="cards3">
    <div class="q"><b>Инстаграм</b><span>Оцените наши самые новые работы прямо сейчас.</span><a href="#">Подписывайтесь на нас ↗</a></div>
    <div class="q"><b>LinkedIn</b><span>Будьте в курсе трендов и проектов в области спортивного дизайна.</span><a href="#">Давайте общаться ↗</a></div>
    <div class="q"><b>Рассылка</b><span>Получайте доступ к нашей еженедельной подборке контента и креативных идей.</span><a href="#news">Присоединяйтесь сейчас ↗</a></div>
  </div>
</div></section>

<div class="banner" id="contact">
  <div><h2>Давайте работать вместе</h2><p>Сотрудничая с нами, вы получите помощь, которая выведет ваш бренд на новый уровень и принесёт результат.</p><a class="btn" href="mailto:hello@example.com">Начать ↗</a></div>
  <div class="collage" id="collage" data-img="b0">Ваш коллаж работ</div>
</div>
</main>

<footer><div class="w">
  <a class="logo" href="#top">YOUR STUDIO</a>
  <nav aria-label="Футер"><a href="#services">Услуги</a><a href="#work">Наши работы</a><a href="#contact">О нас</a><a href="#contact">Связаться с нами</a><a href="#news">Блог</a></nav>
  <small>© 2026 Your Studio. Все права защищены.</small>
</div></footer>
</template><script id="state" type="application/json">{"t":{},"img":{}}</script><script id="code">document.getElementById("app").innerHTML=document.getElementById("tpl").innerHTML;
// Свои картинки: вставьте путь в поле img. Пустое поле показывает цветную заглушку.
var POSTERS=[["#1a7f37","#ffd21f","Матч"],["#0b3d91","#e4372b","Финал"],["#111","#2be360","Кампания"],["#7a2bff","#0b3d91","Игрок"],["#e4372b","#111","Дерби"],["#ff7a1a","#0b1230","Сезон"]].map(function(p,k){return{a:p[0],b:p[1],t:p[2],k:k,img:""}});
var CLIENTS=[],i;for(i=1;i<=18;i++)CLIENTS.push({n:"Логотип "+i,img:""});
var CASES=[
 {t:"Брендинг тура",d:"Гибкая концепция тура, объединяющая команду и город.",tags:["Арт-дирекция","Брендинг","Графика"],a:"#ffd21f",b:"#1a7f37",img:""},
 {t:"Визуальная идентичность мероприятия",d:"Новый бренд для ежегодного саммита по спортивному маркетингу.",tags:["Брендинг","Соцсети"],a:"#0a1aa8",b:"#111",img:""},
 {t:"Графический пакет наград",d:"Две гибкие системы для регулярного контента о игроках.",tags:["Арт-дирекция","Графика"],a:"#0b3d91",b:"#14b8d4",img:""},
 {t:"Дизайн формы к дебютному матчу",d:"Специальная форма, ставшая самой продаваемой в истории клуба.",tags:["Брендинг","Графика"],a:"#e4372b",b:"#7a0f14",img:""}
];
function img(o,alt){return o.img?'<img src="'+o.img+'" alt="'+(alt||"")+'">':""}
function tile(p){return '<div class="tile" data-img="p'+p.k+'" style="--a:'+p.a+';--b:'+p.b+'">'+img(p)+(p.img?"":p.t)+'</div>'}
var reel=document.getElementById("reel");
[0,1].forEach(function(c){
  var set=POSTERS.filter(function(_,k){return k%2===c}).map(tile).join("");
  reel.insertAdjacentHTML("beforeend",'<div class="col'+(c?" r":"")+'">'+set+set+'</div>');
});
document.getElementById("logos").innerHTML=CLIENTS.map(function(c,k){return '<div class="logo-s" data-img="l'+k+'">'+(c.img?img(c,c.n):c.n)+'</div>'}).join("");
document.getElementById("cases").innerHTML=CASES.map(function(c,k){
  return '<article class="case"><div class="media" data-img="c'+k+'" style="--a:'+c.a+';--b:'+c.b+'">'+img(c)+(c.img?"":c.t)+'</div><h3>'+c.t+'</h3><p>'+c.d+'</p><ul class="tags">'+c.tags.map(function(t){return'<li>'+t+'</li>'}).join("")+'</ul></article>'}).join("");
// slider
var sl=document.querySelectorAll(".slide"),dots=document.querySelector(".dots"),cur=0;
function go(n){cur=(n+sl.length)%sl.length;sl.forEach(function(s,k){s.classList.toggle("on",k===cur)});Array.prototype.forEach.call(dots.children,function(d,k){d.setAttribute("aria-current",k===cur)})}
sl.forEach(function(_,k){var d=document.createElement("button");d.setAttribute("aria-label","Отзыв "+(k+1));d.onclick=function(){go(k)};dots.appendChild(d)});
document.querySelector(".sb.p").onclick=function(){go(cur-1)};document.querySelector(".sb.n").onclick=function(){go(cur+1)};go(0);
document.getElementById("form").addEventListener("submit",function(e){
  e.preventDefault();var m=document.getElementById("msg");
  if(!/^\S+@\S+\.\S+$/.test(document.getElementById("email").value.trim())){m.style.color="#ff8a80";m.textContent="Введите корректный адрес почты.";return}
  m.style.color="";m.textContent="Спасибо! Вы подписаны.";this.reset();
});
var S=JSON.parse(document.getElementById("state").textContent);S.t=S.t||{};S.img=S.img||{};
var SEL='h1,h2,h3,p,li,cite,blockquote,.eyebrow,.k,small,a.btn,.q,b,.soc span,.soc a,.logo,nav a';
function leaves(){return Array.prototype.filter.call(document.getElementById("app").querySelectorAll(SEL),function(e){return !e.querySelector(SEL)})}
var L=leaves(),O=L.map(function(e){return e.textContent}),OH=L.map(function(e){return e.innerHTML});
L.forEach(function(e,i){var t=S.t[i];if(t&&t[0]===O[i])e.innerHTML=t[1]});
function applyImgs(){document.querySelectorAll("[data-img]").forEach(function(el){var u=S.img[el.dataset.img],ex=el.querySelector(":scope>img.u");if(ex)ex.remove();el.classList.toggle("has",!!u);if(u){var im=document.createElement("img");im.className="u";im.src=u;im.alt="";el.insertBefore(im,el.firstChild)}})}
applyImgs();
(async function(){
  var u,A,P;
  try{if(!window.claude)return;u=await claude.use("user");if(!u||!(await u.canEdit()))return;A=await claude.use("assets");P=await claude.use("artifact");if(!A||!P)return}catch(e){return}
  var ed=false,bar=document.createElement("div");bar.id="bar";document.body.appendChild(bar);
  var fi=document.createElement("input");fi.type="file";fi.accept="image/*";fi.hidden=true;document.body.appendChild(fi);
  var key=null,msg=document.createElement("span");
  function ui(){bar.innerHTML="";if(!ed){bar.appendChild(btn("Редактировать сайт",start,""))}else{bar.appendChild(btn("Сохранить",save,""));bar.appendChild(btn("Отмена",function(){location.reload()},"g"))}bar.appendChild(msg)}
  function btn(t,f,c){var b=document.createElement("button");b.type="button";b.textContent=t;b.className=c;b.onclick=f;return b}
  function ups(){document.querySelectorAll(".up").forEach(function(b){b.remove()});if(!ed)return;document.querySelectorAll("[data-img]").forEach(function(el){var b=document.createElement("button");b.type="button";b.className="up";b.textContent="Фото";b.onclick=function(ev){ev.stopPropagation();key=el.dataset.img;fi.value="";fi.click()};el.appendChild(b)})}
  function start(){ed=true;document.body.classList.add("ed");leaves().forEach(function(e){e.contentEditable="true"});ups();msg.textContent="Нажмите на текст, чтобы изменить. «Фото» меняет картинку.";ui()}
  fi.onchange=async function(){var f=fi.files[0];if(!f)return;msg.textContent="Загрузка фото…";try{var r=await A.upload(f);S.img[key]=r.url;applyImgs();ups();msg.textContent="Фото загружено. Нажмите «Сохранить»."}catch(er){msg.textContent="Не удалось загрузить: "+(er.message||er.code||"ошибка")}};
  document.addEventListener("keydown",function(e){if(ed&&e.key==="Enter"&&e.target.isContentEditable)e.preventDefault()});
  document.addEventListener("paste",function(e){if(ed&&e.target.isContentEditable){e.preventDefault();document.execCommand("insertText",false,(e.clipboardData||window.clipboardData).getData("text/plain"))}});
  document.addEventListener("click",function(e){if(ed&&e.target.closest("a"))e.preventDefault()},true);
  async function save(){
    msg.textContent="Сохраняю…";S.t={};
    leaves().forEach(function(e,i){if(e.innerHTML!==OH[i])S.t[i]=[O[i],e.innerHTML]});
    var json=JSON.stringify(S).replace(/</g,"\\u003c");
    var html='<!DOCTYPE html>\n<html lang="ru"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover"><title>'+document.title+'</title><link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;700;800&display=swap" rel="stylesheet"><style id="css">'+document.getElementById("css").textContent+'</style></head><body><div id="app"></div><template id="tpl">'+document.getElementById("tpl").innerHTML+'</template><script id="state" type="application/json">'+json+'<\/script><script id="code">'+document.getElementById("code").textContent+'<\/script></body></html>';
    try{await P.publish(html);msg.textContent="Сохранено."}catch(er){msg.textContent="Не удалось сохранить: "+(er.message||er.code||"ошибка")}
  }
  ui();
})();
</script></body></html>
