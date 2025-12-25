*{box-sizing:border-box}
body{
  margin:0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
  background: var(--bg);
  color: var(--text);
}
a{color:inherit}

.wrap{
  max-width: 560px;
  margin: 0 auto;
  padding: 14px 16px 40px;
}

/* Top */
header{
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:12px;
  padding: 6px 2px 10px;
}
.brand{
  font-weight:800;
  letter-spacing:.2px;
  font-size: 18px;
  color: var(--brand);
  white-space:nowrap;
}
.tag{
  font-size:12px;
  color:var(--muted);
  text-align:right;
  line-height:1.2;
}

/* Hero */
.hero{
  border: 1px solid var(--line);
  border-radius: var(--radius);
  overflow:hidden;
  box-shadow: var(--shadow);
  background: linear-gradient(180deg, rgba(25,118,210,.10), rgba(67,167,255,.06));
}

.hero-img{
  height: 180px;
  background:
    radial-gradient(900px 240px at 10% 10%, rgba(67,167,255,.55), transparent 60%),
    radial-gradient(700px 240px at 90% 0%, rgba(25,118,210,.45), transparent 55%),
    linear-gradient(135deg, rgba(255,255,255,.85), rgba(255,255,255,.10)),
    url("https://images.unsplash.com/photo-1569428034239-f9565e32e224?auto=format&fit=crop&w=1400&q=60");
  background-size: cover;
  background-position: center;
  position:relative;
}

.hero-img::after{
  content:"";
  position:absolute; inset:0;
  background: linear-gradient(180deg, rgba(255,255,255,.10), rgba(255,255,255,.92));
}

.hero-body{
  padding: 14px 16px 16px;
}
h1{
  margin: 2px 0 6px;
  font-size: 22px;
  line-height:1.2;
}
.sub{
  margin:0;
  color: var(--muted);
  line-height:1.5;
  font-size: 14px;
}

/* Main buttons */
.nav{
  display:grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
  padding: 14px 16px 16px;
}
.btn{
  display:flex;
  align-items:center;
  justify-content:center;
  padding: 14px 12px;
  min-height: 48px;
  border-radius: 14px;
  border: 1px solid var(--line);
  background: #fff;
  font-weight: 800;
  text-decoration:none;
  box-shadow: 0 8px 18px rgba(25,118,210,.08);
  user-select:none;
  -webkit-tap-highlight-color: transparent;
}
.btn:active{ transform: translateY(1px); }

/* Sections */
section{
  margin-top: 14px;
  border: 1px solid var(--line);
  border-radius: var(--radius);
  background: #fff;
  box-shadow: var(--shadow);
  overflow:hidden;
}
.sec-h{
  padding: 14px 16px 10px;
  border-bottom: 1px solid var(--line);
  background: var(--card);
  font-weight: 900;
  letter-spacing:.2px;
}
.sec-b{ padding: 14px 16px 16px; }
.grid{
  display:grid;
  gap:10px;
}
.card{
  border:1px solid var(--line);
  border-radius: 14px;
  padding: 12px 12px;
  background: #fff;
}
.card b{ display:block; margin-bottom:6px; }
.small{ color: var(--muted); font-size: 13px; line-height:1.45; margin:0; }

/* Order */
form{
  display:grid; gap:10px;
}
input, textarea{
  width:100%;
  border:1px solid var(--line);
  border-radius: 12px;
  padding: 12px 12px;
  font-size: 14px;
  outline:none;
}
textarea{ min-height: 110px; resize: vertical; }
.submit{
  border:none;
  border-radius: 14px;
  padding: 14px 12px;
  font-weight: 900;
  background: linear-gradient(90deg, var(--brand), var(--brand2));
  color:#fff;
  cursor:pointer;
  box-shadow: 0 10px 22px rgba(25,118,210,.22);
}

/* Contact quick links */
.quick{
  display:grid;
  grid-template-columns: 1fr 1fr;
  gap:10px;
  margin-top: 10px;
}
.pill{
  display:flex; align-items:center; justify-content:center;
  padding:12px 10px;
  border-radius: 999px;
  border:1px solid var(--line);
  text-decoration:none;
  font-weight:800;
  background:#fff;
}

footer{
  text-align:center;
  color: var(--muted);
  font-size: 12px;
  margin-top: 14px;
  padding: 10px 0 0;
}
