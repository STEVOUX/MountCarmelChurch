<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mount Carmel Church – Kara, Kodungallur, Thrissur</title>
  <meta name="description" content="Official website of Mount Carmel Church, Kara, Kodungallur, Thrissur. Mass timings, events, announcements, gallery, saints, and contact details." />
  <meta property="og:title" content="Mount Carmel Church – Kara, Kodungallur, Thrissur" />
  <meta property="og:description" content="Mass timings, events, announcements, contact, and ministries." />
  <meta property="og:type" content="website" />
  <meta name="theme-color" content="#0f172a" />

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0b1020;          /* deep indigo slate */
      --bg-soft:#121a33;     /* card background */
      --txt:#e8ecf4;         /* primary text */
      --muted:#b6c0d9;       /* secondary text */
      --brand:#ffd166;       /* warm gold */
      --brand-2:#6ee7b7;     /* mint accent */
      --accent:#8ab4ff;      /* link accent */
      --danger:#ef4444;
      --ok:#22c55e;
      --shadow: 0 10px 30px rgba(0,0,0,.35);
      --radius: 18px;
      --ring: 0 0 0 2px rgba(255,255,255,.07), 0 10px 30px rgba(0,0,0,.35);
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,"Helvetica Neue",Arial; color:var(--txt); background:radial-gradient(1200px 800px at 80% -10%, #1b2450 0%, transparent 50%) , var(--bg);}
    a{color:var(--accent);text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1200px,92%);margin-inline:auto}

    /* Header / Nav */
    header{position:sticky;top:0;z-index:50;background:rgba(11,16,32,.7);backdrop-filter:saturate(140%) blur(12px);border-bottom:1px solid rgba(255,255,255,.06)}
    .nav{display:flex;align-items:center;justify-content:space-between;gap:16px;padding:12px 0}
    .brand{display:flex;align-items:center;gap:12px}
    .brand .logo{width:42px;height:42px;border-radius:12px;background:linear-gradient(135deg,var(--brand),#ff9f1c); display:grid;place-items:center;color:#1a1a1a;font-weight:800;box-shadow:var(--shadow)}
    .brand h1{font-family:"Playfair Display",serif; font-size:22px;letter-spacing:.25px;margin:0}
    .brand small{display:block;color:var(--muted);font-weight:500;line-height:1.1}
    .links{display:flex;gap:18px;align-items:center;white-space:nowrap}
    .links a{color:var(--txt);opacity:.9;font-weight:700;padding:10px 8px;border-radius:10px}
    .links a:hover{color:var(--brand);background:rgba(255,255,255,.05)}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:10px 16px;border-radius:999px;border:1px solid rgba(255,255,255,.12);color:var(--txt);font-weight:700;background:linear-gradient(180deg,rgba(255,255,255,.06),rgba(255,255,255,.03));box-shadow:var(--shadow)}
    .btn:hover{border-color:rgba(255,255,255,.25)}
    .hamburger{display:none;border:1px solid rgba(255,255,255,.12);background:transparent;border-radius:12px;padding:10px;color:var(--txt)}

    /* Hero */
    .hero{position:relative;overflow:hidden}
    .hero::before{content:"";position:absolute;inset:0;background:url('https://images.unsplash.com/photo-1519681393784-d120267933ba?q=80&w=2000&auto=format&fit=crop') center/cover no-repeat;opacity:.2;filter:grayscale(30%) contrast(115%)}
    .hero .wrap{position:relative;padding:86px 0 52px; display:grid;grid-template-columns:1.2fr .9fr;gap:36px;align-items:center}
    .pill{display:inline-flex;gap:8px;align-items:center;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.15);border-radius:999px;padding:8px 12px;color:var(--muted);font-weight:700}
    .hero h2{font-family:"Playfair Display",serif;font-size:54px;line-height:1.05;margin:14px 0}
    .hero p{color:var(--muted);font-size:18px}
    .hero .cta{display:flex;gap:14px;flex-wrap:wrap;margin-top:16px}
    .card{background:linear-gradient(180deg,rgba(255,255,255,.06),rgba(255,255,255,.03));border:1px solid rgba(255,255,255,.1);border-radius:var(--radius);box-shadow:var(--shadow)}
    .schedule{padding:18px}
    .schedule h3{margin:0 0 10px;font-size:20px}
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}

    /* Generic Sections */
    section{padding:64px 0}
    .section-head{display:flex;align-items:end;justify-content:space-between;margin-bottom:24px}
    .section-head h3{font-family:"Playfair Display",serif;font-size:34px;margin:0}
    .section-head p{color:var(--muted)}
    .muted{color:var(--muted)}
    .stat{display:flex;align-items:center;gap:12px}

    /* Gallery */
    .gallery{display:grid;grid-template-columns:repeat(6,1fr);gap:10px}
    .gallery img{border-radius:14px;cursor:pointer;border:1px solid rgba(255,255,255,.14)}

    /* Info / Contact */
    .info{display:grid;grid-template-columns:1.2fr 1fr;gap:26px}
    .map{border:0;width:100%;height:360px;border-radius:var(--radius);filter:saturate(110%) contrast(110%);}

    /* News */
    .composer{display:grid;gap:10px}
    .composer input, .composer textarea{padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)}
    .post{background:linear-gradient(180deg,rgba(255,255,255,.05),rgba(255,255,255,.03));border:1px solid rgba(255,255,255,.09);border-radius:16px;padding:14px}
    .post h4{margin:0 0 6px}
    .post time{color:var(--muted);font-size:12px}

    /* Footer */
    footer{background:linear-gradient(180deg,rgba(255,255,255,.04),rgba(255,255,255,.02));border-top:1px solid rgba(255,255,255,.08);padding:28px 0;color:var(--muted)}

    /* Responsive */
    @media (max-width:980px){
      .hero .wrap{grid-template-columns:1fr}
      .grid.cols-3{grid-template-columns:1fr 1fr}
      .info{grid-template-columns:1fr}
    }
    @media (max-width:760px){
      .links{display:none}
      .hamburger{display:inline-flex}
      .grid.cols-3, .grid.cols-2{grid-template-columns:1fr}
      .hero h2{font-size:40px}
      .gallery{grid-template-columns:repeat(2,1fr)}
    }
  </style>
</head>
<body>
  <!-- Header / Nav -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo" aria-hidden>⛪</div>
        <div>
          <h1>Mount Carmel Church</h1>
          <small>Kara, Kodungallur, Thrissur</small>
        </div>
      </div>
      <nav class="links" aria-label="Primary">
        <a href="#about">About</a>
        <a href="#schedule">Mass Timings</a>
        <a href="#saints">Saints</a>
        <a href="#news">News</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact" class="btn">Contact</a>
      </nav>
      <button class="hamburger" id="menuBtn" aria-label="Open menu">☰</button>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero">
    <div class="container wrap">
      <div>
        <span class="pill">Welcome to our parish</span>
        <h2>Faith • Community • Service</h2>
        <p>We are a Christ‑centered community in Kara, Kodungallur (Thrissur), serving families through the sacraments, catechesis, and charitable works under the Diocese of Kottapuram (Latin rite).</p>
        <div class="cta">
          <a href="#schedule" class="btn">See Mass Timings</a>
          <a href="#contact" class="btn" style="border-color:rgba(255,209,102,.6)">Plan a Visit</a>
        </div>
        <!-- Latest news peek (auto from News storage) -->
        <div id="latestNewsPeek" class="muted" style="margin-top:14px"></div>
      </div>
      <div class="card schedule" id="schedule">
        <h3>Weekly Mass Schedule</h3>
        <div class="grid cols-2">
          <div>
            <div><span class="chip">Monday – Friday</span><br> 6:30 AM <span class="muted">(Daily Mass)</span></div>
            <div style="margin-top:10px"><span class="chip">First Friday</span><br> 6:30 AM & 7:00 AM; <span class="muted">House visits with Holy Communion for the elderly/bed‑ridden (short 2–3 min service) by prior name submission</span></div>
          </div>
          <div>
            <div><span class="chip">Saturday</span><br> 6:30 AM & 7:00 AM; <span class="muted">Novena immediately after morning Mass</span></div>
            <div style="margin-top:10px"><span class="chip">Sunday</span><br> 6:30 AM & 8:30 AM; <span class="muted">Sunday Catechism 9:30–11:00 AM</span></div>
          </div>
        </div>
        <p class="muted" style="margin:12px 0 0">Timings may vary on feast days—see <a href="#news">announcements</a>.</p>
      </div>
    </div>
  </section>

  <!-- About / Details -->
  <section id="about">
    <div class="container">
      <div class="section-head">
        <h3>About Our Church</h3>
        <p>Rooted in prayer, growing in service.</p>
      </div>

      <div class="grid cols-2">
        <div class="card" style="padding:20px">
          <p>Mount Carmel Church, Kara (Kodungallur, Thrissur) is a welcoming parish community. Founded in <strong>1861</strong>, we celebrate the sacraments, form families in faith, and reach out through youth, prayer, and social ministries.</p>
          <ul style="line-height:1.9" class="muted">
            <li><strong>Location:</strong> Kara P.O., Kara – 680671</li>
            <li><strong>Vicar:</strong> Very Rev. Fr. Joshy Kallarakal</li>
            <li><strong>Members:</strong> 3048 • <strong>Houses:</strong> 609 • <strong>Family Units:</strong> 18</li>
            <li><strong>Clergy/Religious:</strong> 6 Diocesan Priests • 22 Religious Sisters</li>
            <li><strong>Rite & Diocese:</strong> Latin • Diocese of Kottapuram</li>
          </ul>
          <a class="btn" href="#contact">Contact the Office</a>
        </div>

        <div class="grid cols-2">
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Established</span><h4 style="margin:6px 0 0">1861</h4></div>
            <p class="muted">Over 160 years of faith in the Kara community.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Families</span><h4 style="margin:6px 0 0">609 Houses</h4></div>
            <p class="muted">Organized into 18 family units for pastoral care.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Community</span><h4 style="margin:6px 0 0">3048 Members</h4></div>
            <p class="muted">Serving all ages: children, youth, elders.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Ministry</span><h4 style="margin:6px 0 0">Priests & Sisters</h4></div>
            <p class="muted">6 diocesan priests, 22 religious sisters supporting parish life.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Saints -->
  <section id="saints">
    <div class="container">
      <div class="section-head">
        <h3>Our Saints & Patrons</h3>
        <p>Intercessors who guide our parish</p>
      </div>

      <div class="grid cols-3">
        <article class="card" style="padding:18px">
          <span class="chip">Patron</span>
          <h4>Our Lady of Mount Carmel</h4>
          <p class="muted">Honored as our parish patroness, reminding us to wear the Scapular and seek Mary's help to follow Jesus more closely.</p>
        </article>
        <article class="card" style="padding:18px">
          <span class="chip">Protector</span>
          <h4>St. Joseph</h4>
          <p class="muted">Model of fatherly care and faithfulness; protector of families and workers.</p>
        </article>
        <article class="card" style="padding:18px">
          <span class="chip">Martyr</span>
          <h4>St. Sebastian</h4>
          <p class="muted">Widely venerated in Kerala; intercedes for the sick and those in danger.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- News / Announcements -->
  <section id="news">
    <div class="container">
      <div class="section-head">
        <h3>News & Announcements</h3>
        <p>Share updates like a community post</p>
      </div>

      <!-- Composer -->
      <div class="card" style="padding:18px;margin-bottom:18px">
        <form id="newsForm" class="composer">
          <input type="text" name="title" placeholder="Post title (e.g., First Friday Adoration)" required>
          <textarea name="body" rows="3" placeholder="Write your announcement…" required></textarea>
          <div style="display:flex;gap:10px;align-items:center;flex-wrap:wrap">
            <input type="text" name="author" placeholder="Posted by (optional)" style="flex:1 1 240px">
            <button class="btn" type="submit">Post Update</button>
            <button class="btn" type="button" id="clearNews" title="Clear all saved posts" style="background:linear-gradient(180deg,rgba(255,0,0,.2),rgba(255,0,0,.08));border-color:rgba(255,0,0,.35)">Clear All</button>
          </div>
          <small class="muted">Posts are saved in your browser (localStorage). They will persist after refresh on this device.</small>
        </form>
      </div>

      <!-- Feed -->
      <div id="newsFeed" class="grid cols-2"></div>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <div class="container">
      <div class="section-head">
        <h3>Parish Gallery</h3>
        <p>Moments from our community (click to enlarge)</p>
      </div>

      <!-- Upload box -->
      <div class="card" style="padding:16px;margin-bottom:16px">
        <form id="galleryForm" style="display:flex;gap:12px;align-items:center;flex-wrap:wrap">
          <input type="file" id="galleryInput" accept="image/*" multiple>
          <button type="button" class="btn" id="addToGallery">Add Selected Photos</button>
          <small class="muted">Uploaded photos are stored locally in your browser (no server).</small>
        </form>
      </div>

      <div class="gallery" id="galleryGrid" aria-live="polite">
        <!-- Starter images (your Discord links) -->
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114803380813926/images_3.jpg?ex=68ac33ed&is=68aae26d&hm=58d7b3f50d17639be37cbbf26945c29dfb5775da3ce83736c8a91e378d8ff9a7&" alt="Church view 1" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114803615825940/images_4.jpg?ex=68ac33ed&is=68aae26d&hm=0bbd6b87fd33bf22adeee3feb57f524d8b95e7d9fdf5acb6234516de3cf4a5a9&" alt="Church view 2" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114803863158835/images.jpg?ex=68ac33ed&is=68aae26d&hm=00d6fe30f475237e6cd4610dd0e686f61ffe8aab0746a6db248107e34682b03e&" alt="Church view 3" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114804106301540/mount-carmel-church-kara-thrissur-churches-939gz5r6o6.avif?ex=68ac33ed&is=68aae26d&hm=1533d06386fad3a107daf23348e8b2b2c9141f533e5308b0a7916f7fa036231f&" alt="Church view 4" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114804463079464/mount-carmel-church-kara-thrissur-churches-LL2AjNnQqK-250.avif?ex=68ac33ed&is=68aae26d&hm=636f977d3205775efc31daa2dcb9b06e79dbf91ad4687649720c141828404732&" alt="Church view 5" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114805297741855/mount-carmel-church-kara-thrissur-churches-Sv7EGnlf7s_1.jpg?ex=68ac33ed&is=68aae26d&hm=43ecebfb1646e677f527d932430f751e6c78ecb4df196ab702c08a05642afa36&" alt="Church view 6" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114805633290270/mount-carmel-church-kara-thrissur-churches-szhblfi508.avif?ex=68ac33ed&is=68aae26d&hm=928afb8f922c8e3434f3d9507b11bc72437b96d4c702a45644a5b38e8f1e2a0e&" alt="Church view 7" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114806069366815/mount-carmel-church-kara-thrissur-churches-Y7px5sztaU-250.avif?ex=68ac33ed&is=68aae26d&hm=a39c77bc78f629d69c7784f820cc35abc2645e35e5b9adf7db3521ec867b65d5&" alt="Church view 8" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409114806472151081/mount-carmel-church-kara-thrissur-churches-YYcBdnIUDA-250_1.avif?ex=68ac33ed&is=68aae26d&hm=489b17aaa2642f3d99e58b8c8922848d23926b57c95ccbe532c552a5a8396a95&" alt="Church view 9" data-origin="starter">
      </div>
    </div>
  </section>

  <!-- Contact / Visit -->
  <section id="contact">
    <div class="container info">
      <div class="card" style="padding:20px">
        <div class="section-head" style="margin-bottom:10px">
          <h3>Contact & Visit</h3>
          <p>We’d love to see you</p>
        </div>
        <p class="muted">
          <strong>Mount Carmel Church (Latin)</strong><br>
          Kara P.O., Kara – 680671, Kodungallur, Thrissur, Kerala<br>
          Parish Office Phone: <a href="tel:+919495131287">+91 9495131287</a><br>
          Email: <a href="mailto:parishoffice@example.com">parishoffice@example.com</a>
        </p>
        <form id="msgForm" class="grid cols-2" style="gap:12px;margin-top:8px">
          <input class="card" name="name" placeholder="Your name" required style="padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)">
          <input class="card" name="email" placeholder="Email" type="email" required style="padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)">
          <input class="card" name="phone" placeholder="Phone (optional)" style="padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)">
          <input class="card" name="subject" placeholder="Subject" required style="padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)">
          <textarea class="card" name="message" placeholder="Your message" rows="4" required style="grid-column:1/-1;padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);color:var(--txt)"></textarea>
          <button class="btn" type="submit">Send Message</button>
          <small id="formNote" style="align-self:center" class="muted">This opens your email app (no server needed).</small>
        </form>
      </div>
      <div class="card" style="padding:10px">
        <iframe class="map" loading="lazy" allowfullscreen
          referrerpolicy="no-referrer-when-downgrade"
          src="https://www.google.com/maps?q=Kara%20Kodungallur%20Thrissur&output=embed"
          title="Map to Mount Carmel Church"></iframe>
      </div>
    </div>
  </section>

  <!-- Donate CTA -->
  <section>
    <div class="container card" style="padding:20px;display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;gap:16px">
      <div>
        <h3 style="margin:0 0 6px;font-family:'Playfair Display',serif">Support Our Mission</h3>
        <p class="muted" style="margin:0">Your generosity helps our parish services and outreach.</p>
      </div>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn" href="#">Give Online</a>
        <a class="btn" href="#">Bank / UPI Details</a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container" style="display:flex;gap:14px;flex-wrap:wrap;align-items:center;justify-content:space-between">
      <div>© <span id="year"></span> Mount Carmel Church, Kara • All rights reserved</div>
      <div class="muted" style="display:flex;gap:12px;align-items:center;flex-wrap:wrap">
        <span>Website made by <strong>Steve Shine</strong></span>
        <span aria-hidden>•</span>
        <a href="mailto:steveshine999@gmail.com">steveshine999@gmail.com</a>
        <span aria-hidden>•</span>
        <a href="tel:+918921370655">+91 8921370655</a>
      </div>
    </div>
  </footer>

  <!-- Lightbox Modal -->
  <dialog id="lightbox" style="border:none;border-radius:14px;padding:0;background:#0a0f20;max-width:min(92vw,1000px)">
    <img id="lightImg" alt="Expanded gallery image" style="width:100%;height:auto;border-radius:14px"/>
    <form method="dialog" style="position:absolute;top:8px;right:8px">
      <button class="btn" aria-label="Close">Close ✕</button>
    </form>
  </dialog>

  <script>
    // ---------- Mobile menu toggle ----------
    const menuBtn = document.getElementById('menuBtn');
    menuBtn?.addEventListener('click', () => {
      const nav = document.querySelector('.links');
      nav.style.display = nav.style.display === 'flex' ? 'none' : 'flex';
    });

    // ---------- Lightbox for gallery ----------
    const dlg = document.getElementById('lightbox');
    const lightImg = document.getElementById('lightImg');
    function openLightbox(src, alt){ lightImg.src = src; lightImg.alt = alt || 'Gallery image'; dlg.showModal(); }
    document.getElementById('galleryGrid').addEventListener('click', (e)=>{
      const t = e.target;
      if(t.tagName === 'IMG') openLightbox(t.src, t.alt);
    });

    // ---------- Gallery uploads (persist to localStorage) ----------
    const galleryInput = document.getElementById('galleryInput');
    const addToGalleryBtn = document.getElementById('addToGallery');
    const galleryGrid = document.getElementById('galleryGrid');
    const GALLERY_KEY = 'mcc_kara_gallery_v1';

    function loadGallery(){
      try{
        const saved = JSON.parse(localStorage.getItem(GALLERY_KEY)||'[]');
        for(const url of saved){
          const img = document.createElement('img');
          img.src = url; img.alt = 'Uploaded photo';
          img.dataset.origin = 'local';
          galleryGrid.appendChild(img);
        }
      }catch(err){ console.warn('Gallery load error', err); }
    }

    function saveGallery(){
      const urls = [...galleryGrid.querySelectorAll('img')]
        .filter(img => img.dataset.origin === 'local')
        .map(img => img.src);
      localStorage.setItem(GALLERY_KEY, JSON.stringify(urls));
    }

    addToGalleryBtn.addEventListener('click', async ()=>{
      const files = [...(galleryInput.files||[])];
      if(!files.length) return alert('Please choose one or more images.');
      for(const f of files){
        if(!f.type.startsWith('image/')) continue;
        const url = await fileToDataURL(f);
        const img = document.createElement('img');
        img.src = url; img.alt = f.name; img.dataset.origin = 'local';
        galleryGrid.appendChild(img);
      }
      saveGallery();
      galleryInput.value = '';
      window.scrollTo({top: galleryGrid.offsetTop - 80, behavior:'smooth'});
    });

    function fileToDataURL(file){
      return new Promise((res, rej)=>{
        const r = new FileReader();
        r.onload = ()=>res(r.result); r.onerror = rej; r.readAsDataURL(file);
      });
    }

    // ---------- News posts (persist to localStorage) ----------
    const NEWS_KEY = 'mcc_kara_news_v1';
    const newsForm = document.getElementById('newsForm');
    const newsFeed = document.getElementById('newsFeed');
    const clearNewsBtn = document.getElementById('clearNews');
    const latestNewsPeek = document.getElementById('latestNewsPeek');

    function loadNews(){
      let items = [];
      try{ items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]'); }catch(err){ items = []; }

      // Seed with the requested first post if empty
      if(items.length === 0){
        items.push({
          id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()),
          title: "Sunday Catechism – First Semester Exam",
          body: "This year's first semester exam of Sunday Catechism will be conducted on October 5th.",
          author: "Parish Office",
          ts: Date.now()
        });
        localStorage.setItem(NEWS_KEY, JSON.stringify(items));
      }

      renderNews(items);
    }

    function renderNews(items){
      // newest first
      items.sort((a,b)=>b.ts - a.ts);
      newsFeed.innerHTML = '';
      for(const post of items){
        const card = document.createElement('article');
        card.className = 'post';
        card.innerHTML = `
          <h4>${escapeHTML(post.title)}</h4>
          <time>${new Date(post.ts).toLocaleString()}</time>
          <p class="muted" style="margin:8px 0 0">${escapeHTML(post.body)}</p>
          <div class="muted" style="margin-top:8px;display:flex;gap:10px;align-items:center">
            <span>— ${escapeHTML(post.author||'Anonymous')}</span>
            <button class="btn" data-del="${post.id}" title="Delete this post" style="padding:6px 10px;font-weight:600">Delete</button>
          </div>
        `;
        newsFeed.appendChild(card);
      }

      // Latest news peek in hero
      if(items[0]){
        latestNewsPeek.innerHTML = `Latest: <strong>${escapeHTML(items[0].title)}</strong> — ${escapeHTML(items[0].body)}`;
      }
    }

    newsFeed.addEventListener('click',(e)=>{
      const btn = e.target.closest('button[data-del]');
      if(!btn) return;
      const id = btn.getAttribute('data-del');
      let items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]');
      items = items.filter(x=>x.id !== id);
      localStorage.setItem(NEWS_KEY, JSON.stringify(items));
      renderNews(items);
    });

    newsForm.addEventListener('submit',(e)=>{
      e.preventDefault();
      const fd = new FormData(newsForm);
      const title = (fd.get('title')||'').toString().trim();
      const body = (fd.get('body')||'').toString().trim();
      const author = (fd.get('author')||'').toString().trim();
      if(!title || !body) return alert('Please fill in title and body.');
      const post = { id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()), title, body, author, ts: Date.now() };
      const items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]');
      items.push(post);
      localStorage.setItem(NEWS_KEY, JSON.stringify(items));
      newsForm.reset();
      renderNews(items);
      window.location.hash = '#news';
    });

    clearNewsBtn.addEventListener('click',()=>{
      if(confirm('Delete all saved news posts from this browser?')){
        localStorage.removeItem(NEWS_KEY); loadNews();
      }
    });

    function escapeHTML(str){
      return str.replace(/[&<>"]/g, s => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[s]));
    }

    // ---------- Contact form (mailto) ----------
    const form = document.getElementById('msgForm');
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const data = Object.fromEntries(new FormData(form));
      const body = encodeURIComponent(
        `Name: ${data.name}\nEmail: ${data.email}\nPhone: ${data.phone||''}\n\n${data.message}`
      );
      const subject = encodeURIComponent(data.subject || 'Enquiry from church website');
      // Change the email below to your parish email if needed
      window.location.href = `mailto:parishoffice@example.com?subject=${subject}&body=${body}`;
    });

    // ---------- Footer year ----------
    document.getElementById('year').textContent = new Date().getFullYear();

    // ---------- Init ----------
    loadGallery();
    loadNews();
  </script>
</body>
</html>
