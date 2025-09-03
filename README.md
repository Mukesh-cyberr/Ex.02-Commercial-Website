# Ex02 Commercial Website
## Date:03-09-2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML
```
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>FlexCommerce — Modern Storefront</title>
  <link rel="stylesheet" href="4.css" />
</head>
<body>
  <a class="skip-link" href="#main">Skip to content</a>

  
  <header class="topbar">
    <div class="container topbar__row">
      <div class="brand">
        <span class="brand__logo" aria-hidden="true">◆</span>
        <span class="brand__name">FlexCommerce</span>
      </div>

      <nav class="nav" aria-label="Primary">
        <button class="nav__toggle" aria-expanded="false" aria-controls="navMenu">☰</button>
        <ul id="navMenu" class="nav__list">
          <li><a href="#products">Products</a></li>
          <li><a href="#features">Features</a></li>
          <li><a href="#pricing">Pricing</a></li>
          <li><a href="#testimonials">Reviews</a></li>
          <li><a href="#contact" class="btn btn--sm">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero">
    <div class="container hero__row">
      <div class="hero__copy">
        <h1>Grow your business with a storefront that sells.</h1>
        <p class="muted">
          Flexible layouts, blazing-fast pages, and conversion-first design.
        </p>
        <div class="hero__actions">
          <a href="#products" class="btn">Shop Now</a>
          <a href="#features" class="btn btn--ghost">See Features</a>
        </div>
        <ul class="hero__badges">
          <li>✔ 30-day returns</li>
          <li>✔ Free shipping over ₹999</li>
          <li>✔ Secure checkout</li>
        </ul>
      </div>

      
      <div class="hero__visual" role="img" aria-label="Product collage illustration"></div>
    </div>
  </section>

  
  <main id="main">
    <section id="products" class="section">
      <div class="container">
        <div class="section__head">
          <h2>Best Sellers</h2>
          <a href="#" class="link">View all →</a>
        </div>

        <div class="cards">
          <!-- Card -->
          <article class="card">
            <div class="card__media" aria-hidden="true"></div>
            <div class="card__body">
              <h3 class="card__title">Pro Wireless Headset</h3>
              <p class="muted">Crystal-clear calls. 40-hr battery.</p>
              <div class="card__meta">
                <span class="price">₹4,499</span>
                <span class="pill">In stock</span>
              </div>
              <div class="card__actions">
                <button class="btn btn--sm">Add to Cart</button>
                <button class="btn btn--sm btn--ghost">Details</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card__media" aria-hidden="true"></div>
            <div class="card__body">
              <h3 class="card__title">Smart Fitness Band</h3>
              <p class="muted">Sleep + heart rate tracking.</p>
              <div class="card__meta">
                <span class="price">₹2,199</span>
                <span class="pill">New</span>
              </div>
              <div class="card__actions">
                <button class="btn btn--sm">Add to Cart</button>
                <button class="btn btn--sm btn--ghost">Details</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card__media" aria-hidden="true"></div>
            <div class="card__body">
              <h3 class="card__title">Compact Bluetooth Speaker</h3>
              <p class="muted">Rich sound. Pocket size.</p>
              <div class="card__meta">
                <span class="price">₹1,799</span>
                <span class="pill">-20%</span>
              </div>
              <div class="card__actions">
                <button class="btn btn--sm">Add to Cart</button>
                <button class="btn btn--sm btn--ghost">Details</button>
              </div>
            </div>
          </article>

          <article class="card">
            <div class="card__media" aria-hidden="true"></div>
            <div class="card__body">
              <h3 class="card__title">USB-C GaN Charger 65W</h3>
              <p class="muted">Fast charge laptop & phone.</p>
              <div class="card__meta">
                <span class="price">₹2,499</span>
                <span class="pill pill--gray">Limited</span>
              </div>
              <div class="card__actions">
                <button class="btn btn--sm">Add to Cart</button>
                <button class="btn btn--sm btn--ghost">Details</button>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    
    <section id="features" class="section section--alt">
      <div class="container features">
        <div class="feature">
          <div class="feature__icon" aria-hidden="true">🔐</div>
          <h3>Secure Payments</h3>
          <p class="muted">PCI-DSS compliant checkout with multiple options.</p>
        </div>
        <div class="feature">
          <div class="feature__icon" aria-hidden="true">⚡</div>
          <h3>Fast Delivery</h3>
          <p class="muted">Same-day dispatch on orders before 2pm.</p>
        </div>
        <div class="feature">
          <div class="feature__icon" aria-hidden="true">💬</div>
          <h3>24×7 Support</h3>
          <p class="muted">Real humans on chat, email, and phone.</p>
        </div>
      </div>
    </section>

    
    <section id="pricing" class="section">
      <div class="container">
        <h2>Simple Pricing</h2>
        <div class="pricing">
          <div class="pricecard">
            <h3>Starter</h3>
            <p class="price">₹1,299</p>
            <ul class="list">
              <li>Basic warranty</li>
              <li>Email support</li>
              <li>Standard delivery</li>
            </ul>
            <button class="btn btn--block">Choose Starter</button>
          </div>
          <div class="pricecard pricecard--primary" aria-label="Most popular">
            <div class="pill pill--accent">Popular</div>
            <h3>Pro</h3>
            <p class="price">₹2,999</p>
            <ul class="list">
              <li>2-year warranty</li>
              <li>Priority support</li>
              <li>Express delivery</li>
            </ul>
            <button class="btn btn--block">Choose Pro</button>
          </div>
          <div class="pricecard">
            <h3>Business</h3>
            <p class="price">₹5,499</p>
            <ul class="list">
              <li>Extended warranty</li>
              <li>Dedicated manager</li>
              <li>Bulk discounts</li>
            </ul>
            <button class="btn btn--block">Choose Business</button>
          </div>
        </div>
      </div>
    </section>

    
    <section id="testimonials" class="section section--alt">
      <div class="container">
        <h2>Loved by customers</h2>
        <div class="testimonials">
          <blockquote class="quote">
            <p>“Super smooth checkout and super fast shipping.”</p>
            <footer>— Aditi</footer>
          </blockquote>
          <blockquote class="quote">
            <p>“Clean design, great prices. Will buy again.”</p>
            <footer>— Karthik</footer>
          </blockquote>
          <blockquote class="quote">
            <p>“Support team solved my issue in minutes.”</p>
            <footer>— Neha</footer>
          </blockquote>
        </div>
      </div>
    </section>

    
    <section id="contact" class="cta">
      <div class="container cta__row">
        <h2>Ready to get started?</h2>
        <form class="cta__form" action="#" method="post">
          <label class="sr-only" for="email">Email</label>
          <input id="email" name="email" type="email" placeholder="Enter your email" required />
          <button class="btn">Join Newsletter</button>
        </form>
      </div>
    </section>
  </main>

  
  <footer class="footer">
    <div class="container footer__row">
      <div class="brand brand--muted">
        <span class="brand__logo" aria-hidden="true">◆</span>
        <span class="brand__name">FlexCommerce</span>
      </div>
      <ul class="footer__links">
        <li><a href="#">Privacy</a></li>
        <li><a href="#">Terms</a></li>
        <li><a href="#">Returns</a></li>
        <li><a href="#">Support</a></li>
      </ul>
      <p class="muted">© <span id="year"></span> FlexCommerce. All rights reserved.</p>
    </div>
  </footer>

  <script>
    
    const toggle = document.querySelector(".nav__toggle");
    const list = document.querySelector("#navMenu");
    toggle.addEventListener("click", () => {
      const open = toggle.getAttribute("aria-expanded") === "true";
      toggle.setAttribute("aria-expanded", String(!open));
      list.classList.toggle("is-open");
    });

    
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>

```
CSS
```
:root{
  --bg: #0b0d12;
  --panel: #11151d;
  --muted: #98a2b3;
  --text: #e6e9ef;
  --brand: #6ee7ff;
  --brand-2: #a78bfa;
  --accent: #22c55e;
  --border: #1f2532;
  --shadow: 0 10px 30px rgba(0,0,0,.25);
  --radius: 16px;
}

*{ box-sizing: border-box; }
html,body{ height:100%; }
body{
  margin:0;
  font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial;
  color: var(--text);
  background: radial-gradient(1200px 800px at 20% -10%, #131826, #0b0d12 60%);
  line-height: 1.6;
}

.container{
  width: min(1100px, 92vw);
  margin-inline: auto;
}

.muted{ color: var(--muted); }
.link{ color: var(--brand); text-decoration: none; }
.link:hover{ text-decoration: underline; }


.btn{
  display:inline-flex; align-items:center; justify-content:center;
  padding: .8rem 1.2rem; border-radius: 999px;
  background: linear-gradient(90deg, var(--brand), var(--brand-2));
  color:#0b0d12; border:0; font-weight:600; cursor:pointer; box-shadow: var(--shadow);
  transition: transform .15s ease;
}
.btn:hover{ transform: translateY(-1px); }
.btn--ghost{
  background: transparent; color: var(--text); border:1px solid var(--border); box-shadow:none;
}
.btn--sm{ padding:.55rem .9rem; font-size:.9rem; }
.btn--block{ width:100%; }


.pill{
  display:inline-flex; align-items:center; padding:.25rem .55rem; border-radius:999px;
  font-size:.8rem; background:rgba(255,255,255,.08); border:1px solid var(--border);
}
.pill--accent{ background: rgba(34,197,94,.18); border-color: rgba(34,197,94,.35); }
.pill--gray{ background: rgba(255,255,255,.06); }

.price{ font-weight: 700; }


.skip-link{
  position:absolute; left:-999px; top:auto; width:1px; height:1px; overflow:hidden;
}
.skip-link:focus{
  position:static; width:auto; height:auto; padding:.5rem 1rem;
  background:#fff; color:#000; border-radius:.5rem; margin:.5rem;
}


.topbar{
  position: sticky; top: 0; z-index: 5;
  background: rgba(11,13,18,.7); backdrop-filter: blur(8px); border-bottom: 1px solid var(--border);
}
.topbar__row{
  display:flex; align-items:center; justify-content:space-between; padding: .9rem 0;
}
.brand{ display:flex; align-items:center; gap:.6rem; font-weight:700; }
.brand__logo{ width:1.25rem; height:1.25rem; display:inline-grid; place-items:center;
  background: linear-gradient(135deg, var(--brand), var(--brand-2)); color:#0b0d12; border-radius:4px; font-size:.9rem; }
.brand__name{ letter-spacing:.3px; }
.brand--muted .brand__name{ color: var(--muted); }

.nav{ display:flex; align-items:center; gap:1rem; }
.nav__toggle{ display:none; background:none; border:1px solid var(--border); color:var(--text);
  padding:.4rem .6rem; border-radius:10px; cursor:pointer; }
.nav__list{
  display:flex; gap:1.2rem; list-style:none; margin:0; padding:0;
}
.nav__list a{ color: var(--text); text-decoration:none; padding:.45rem .7rem; border-radius: .6rem; }
.nav__list a:hover{ background: rgba(255,255,255,.06); }


.hero{
  padding: clamp(2rem, 4vw + 2rem, 5rem) 0;
}
.hero__row{
  display:flex; gap:2rem; align-items:center; justify-content:space-between;
}
.hero__copy{ max-width: 560px; }
.hero h1{ line-height:1.15; font-size: clamp(1.8rem, 2.8vw + 1rem, 3rem); margin:.2rem 0 .5rem; }
.hero__actions{ display:flex; gap:.8rem; margin:1rem 0; }
.hero__badges{ display:flex; gap:1rem; list-style:none; padding:0; margin:1rem 0 0; color:var(--muted); }

.hero__visual{
  width:min(480px, 40vw); aspect-ratio: 4/3; border-radius: var(--radius);
  background:
    radial-gradient(140px 100px at 70% 30%, rgba(167,139,250,.35), transparent 60%),
    radial-gradient(180px 120px at 30% 70%, rgba(110,231,255,.35), transparent 60%),
    linear-gradient(180deg, #0f1422, #0b0d12);
  border:1px solid var(--border);
  box-shadow: var(--shadow);
  position: relative; overflow: hidden;
}
.hero__visual::after{
  content:""; position:absolute; inset:10%; border-radius: 24px;
  border:1px dashed rgba(255,255,255,.1);
}


.section{ padding: 3rem 0; }
.section--alt{ background: linear-gradient(180deg, rgba(255,255,255,.03), transparent); }
.section__head{ display:flex; align-items:center; justify-content:space-between; margin-bottom:1rem; }


.cards{
  display:flex; gap:1rem; flex-wrap: wrap;
}
.card{
  display:flex; flex-direction: column; background: var(--panel); border:1px solid var(--border);
  border-radius: var(--radius); overflow:hidden; flex:1 1 240px; max-width: calc(25% - .75rem);
  min-width: 240px; box-shadow: var(--shadow);
}
.card__media{
  background:
    linear-gradient(120deg, rgba(110,231,255,.35), rgba(167,139,250,.35)),
    linear-gradient(180deg, #121826, #0e1320);
  height: 150px;
}
.card__body{ padding:1rem; display:flex; gap:.75rem; flex-direction:column; }
.card__title{ margin:0; font-size:1.05rem; }
.card__meta{ display:flex; align-items:center; gap:.5rem; }


.features{
  display:flex; gap:1rem; flex-wrap:wrap; align-items:stretch; justify-content:space-between;
}
.feature{
  flex:1 1 240px; min-width:240px; background: var(--panel); border:1px solid var(--border);
  border-radius: var(--radius); padding:1.2rem; box-shadow: var(--shadow);
  display:flex; flex-direction:column; gap:.4rem;
}
.feature__icon{ font-size:1.4rem; }


.pricing{
  display:flex; gap:1rem; flex-wrap:wrap;
}
.pricecard{
  flex:1 1 240px; min-width:240px; background: var(--panel); border:1px solid var(--border);
  border-radius: var(--radius); padding:1.2rem; box-shadow: var(--shadow); position:relative;
  display:flex; flex-direction:column; gap:.8rem;
}
.pricecard--primary{
  outline: 2px solid rgba(110,231,255,.45);
  background: linear-gradient(180deg, rgba(110,231,255,.06), transparent);
}
.list{ margin:0; padding-left:1.1rem; color: var(--muted); }


.testimonials{
  display:flex; gap:1rem; flex-wrap: wrap;
}
.quote{
  flex:1 1 280px; min-width:280px; background: var(--panel); border:1px solid var(--border);
  border-radius: var(--radius); padding:1.2rem; box-shadow: var(--shadow);
}


.cta{
  padding: 2.5rem 0; background: linear-gradient(90deg, rgba(110,231,255,.15), rgba(167,139,250,.15));
  border-top:1px solid var(--border); border-bottom:1px solid var(--border);
}
.cta__row{ display:flex; align-items:center; justify-content:space-between; gap:1rem; flex-wrap:wrap; }
.cta__form{ display:flex; gap:.6rem; flex-wrap:wrap; }
.cta__form input{
  flex:1 1 240px; min-width: 240px; background: var(--panel); border:1px solid var(--border);
  border-radius: 999px; padding:.8rem 1rem; color: var(--text);
}


.footer{ padding: 2rem 0; }
.footer__row{ display:flex; gap:1rem; align-items:center; justify-content:space-between; flex-wrap:wrap; }
.footer__links{ list-style:none; display:flex; gap:1rem; margin:0; padding:0; }
.footer__links a{ color: var(--muted); text-decoration:none; }
.footer__links a:hover{ color: var(--text); }


.card__actions{ display:flex; gap:.6rem; }


@media (max-width: 860px){
  .nav__toggle{ display:inline-block; }
  .nav__list{ position:absolute; right:1rem; top:60px; flex-direction:column; background: var(--panel);
    border:1px solid var(--border); border-radius: var(--radius); padding:.6rem; display:none; }
  .nav__list.is-open{ display:flex; }
}

@media (max-width: 900px){
  .card{ max-width: calc(50% - .5rem); }
}

@media (max-width: 560px){
  .hero__row{ flex-direction: column; }
  .card{ max-width: 100%; }
}


@media (prefers-reduced-motion: reduce){
  *{ animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration:0.001ms !important; }
}


.sr-only{
  position:absolute; width:1px; height:1px; padding:0; margin:-1px; overflow:hidden; clip:rect(0,0,0,0); border:0;
}


```


## OUTPUT
<img width="1900" height="915" alt="Screenshot 2025-09-03 152644" src="https://github.com/user-attachments/assets/48d0afae-80e8-4620-b0dc-87ee18ad2c51" />
<img width="1897" height="897" alt="Screenshot 2025-09-03 152805" src="https://github.com/user-attachments/assets/024c90dc-5b2c-4817-94a5-3bc73981752c" />
<img width="1896" height="902" alt="Screenshot 2025-09-03 152843" src="https://github.com/user-attachments/assets/0797728e-d8d1-4b63-8a38-7a1457e388c2" />
<img width="1901" height="904" alt="Screenshot 2025-09-03 152911" src="https://github.com/user-attachments/assets/9e36905a-6cee-4de7-b655-5a3191ca3f16" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
