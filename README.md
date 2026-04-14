<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kim Tuyen ✦ Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=Nunito:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
<style>
:root{--y:#FFE135;--pk:#FF6B9D;--bl:#4ECDC4;--or:#FF8C42;--pu:#A855F7;--dark:#0F0F0F;--w:#FAFAFA;--gray:#666}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-snap-type:y mandatory}
body{background:var(--dark);color:var(--w);font-family:'Nunito',sans-serif;overflow-x:hidden}

nav{position:fixed;top:0;left:0;right:0;z-index:200;display:flex;align-items:center;justify-content:space-between;padding:16px 40px;background:rgba(15,15,15,0.85);backdrop-filter:blur(20px);border-bottom:1px solid rgba(255,255,255,0.07)}
.logo{font-family:'Syne',sans-serif;font-size:22px;font-weight:800;color:var(--y);text-decoration:none}
.ndots{display:flex;gap:8px;align-items:center}
.ndot{width:8px;height:8px;border-radius:50%;background:rgba(255,255,255,0.2);cursor:pointer;border:none;transition:all .3s}
.ndot.on{background:var(--y);transform:scale(1.5)}
.ncnt{font-family:'Syne',sans-serif;font-size:12px;color:var(--gray);margin-left:8px}

.slide{min-height:100vh;scroll-snap-align:start;position:relative;display:flex;align-items:center;padding:80px 0 48px;overflow:hidden}
.blob{position:absolute;border-radius:50%;filter:blur(90px);pointer-events:none}

/* HERO */
#s0{background:var(--dark)}
.hi{width:100%;max-width:1100px;margin:0 auto;padding:0 48px;display:grid;grid-template-columns:1fr 1fr;gap:64px;align-items:center}
.htag{display:inline-flex;align-items:center;gap:8px;background:rgba(255,225,53,0.1);border:1px solid rgba(255,225,53,0.25);border-radius:100px;padding:6px 16px;font-size:11px;color:var(--y);letter-spacing:0.12em;text-transform:uppercase;font-weight:700;margin-bottom:24px;width:fit-content;animation:up .7s ease both}
.hname{font-family:'Syne',sans-serif;font-size:clamp(54px,6.5vw,92px);font-weight:800;line-height:.93;letter-spacing:-.03em;animation:up .7s .1s ease both;margin-bottom:20px}
.hname .stroke{-webkit-text-stroke:2px var(--y);color:transparent}
.hdesc{font-size:15px;line-height:1.85;color:rgba(255,255,255,0.55);max-width:420px;margin-bottom:36px;animation:up .7s .2s ease both}
.hbtns{display:flex;gap:12px;flex-wrap:wrap;animation:up .7s .3s ease both}
.btn{padding:13px 28px;border-radius:100px;font-size:13px;font-weight:700;letter-spacing:.05em;text-decoration:none;cursor:pointer;border:none;transition:transform .2s,box-shadow .2s;font-family:'Nunito',sans-serif;display:inline-flex;align-items:center;gap:8px}
.btn:hover{transform:translateY(-3px)}
.by{background:var(--y);color:var(--dark)}.by:hover{box-shadow:0 14px 36px rgba(255,225,53,.35)}
.bg{background:transparent;border:1.5px solid rgba(255,255,255,.18);color:var(--w)}.bg:hover{border-color:rgba(255,255,255,.5)}
.stats{display:flex;gap:32px;margin-top:40px;padding-top:32px;border-top:1px solid rgba(255,255,255,.08)}
.sn{font-family:'Syne',sans-serif;font-size:32px;font-weight:800;color:var(--y)}
.sl{font-size:11px;text-transform:uppercase;letter-spacing:.12em;color:var(--gray);margin-top:2px}

.hphoto{position:relative;animation:up .7s .15s ease both}
.hframe{width:100%;aspect-ratio:4/5;border-radius:28px;background:linear-gradient(135deg,rgba(255,225,53,.1),rgba(78,205,196,.1));border:1.5px solid rgba(255,255,255,.1);overflow:hidden;cursor:pointer;position:relative;transition:transform .3s}
.hframe:hover{transform:scale(1.02)}
.hframe img{width:100%;height:100%;object-fit:cover;display:none}
.hframe img.on{display:block}
.upzone{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:12px;color:rgba(255,255,255,.35);text-align:center;padding:24px;pointer-events:none}
.upzone .ico{font-size:44px;opacity:.5}
.upzone p{font-size:13px;line-height:1.6;font-weight:600}
.upzone span{font-size:11px;opacity:.4;letter-spacing:.1em;text-transform:uppercase}
.chip{position:absolute;background:rgba(15,15,15,.9);border:1.5px solid rgba(255,255,255,.12);border-radius:100px;padding:8px 16px;font-size:12px;font-weight:700;white-space:nowrap;animation:fl var(--d,3s) ease-in-out infinite}
.c1{top:12%;right:-28px;color:var(--y);border-color:rgba(255,225,53,.3);--d:3.2s}
.c2{bottom:22%;left:-28px;color:var(--bl);border-color:rgba(78,205,196,.3);--d:4s}
.c3{top:52%;right:-24px;color:var(--pk);border-color:rgba(255,107,157,.3);--d:3.6s}
@keyframes up{from{opacity:0;transform:translateY(28px)}to{opacity:1;transform:translateY(0)}}
@keyframes fl{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}

/* SECTION HEADER */
.sh{width:100%;max-width:1100px;margin:0 auto 44px;padding:0 48px}
.slabel{display:inline-flex;align-items:center;gap:8px;font-size:11px;letter-spacing:.2em;text-transform:uppercase;font-weight:700;margin-bottom:12px}
.stitle{font-family:'Syne',sans-serif;font-size:clamp(38px,4.5vw,58px);font-weight:800;line-height:1;letter-spacing:-.025em}

/* SKILLS */
#s1{background:#111}
.sc{width:100%;max-width:1100px;margin:0 auto;padding:0 48px}
.bento{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.tile{background:rgba(255,255,255,.04);border:1.5px solid rgba(255,255,255,.08);border-radius:20px;padding:24px;transition:transform .25s,border-color .25s}
.tile:hover{transform:translateY(-5px);border-color:rgba(255,255,255,.18)}
.tile.big{grid-column:span 2}
.temi{font-size:28px;margin-bottom:12px}
.tname{font-family:'Syne',sans-serif;font-size:16px;font-weight:700;margin-bottom:6px}
.tdesc{font-size:13px;color:rgba(255,255,255,.5);line-height:1.6}
.ttags{display:flex;flex-wrap:wrap;gap:6px;margin-top:12px}
.ttag{font-size:11px;padding:4px 10px;border-radius:100px;font-weight:700}
.t1 .tname{color:var(--y)}.t1 .ttag{background:rgba(255,225,53,.12);color:var(--y)}
.t2 .tname{color:var(--pk)}.t2 .ttag{background:rgba(255,107,157,.12);color:var(--pk)}
.t3 .tname{color:var(--bl)}.t3 .ttag{background:rgba(78,205,196,.12);color:var(--bl)}
.t4 .tname{color:var(--or)}.t4 .ttag{background:rgba(255,140,66,.12);color:var(--or)}
.t5 .tname{color:var(--pu)}.t5 .ttag{background:rgba(168,85,247,.12);color:var(--pu)}
.t6 .tname{color:var(--y)}.t6 .ttag{background:rgba(255,225,53,.12);color:var(--y)}

/* EXP SLIDES */
.eslide{background:var(--dark)}
.ein{width:100%;max-width:1100px;margin:0 auto;padding:0 48px;display:grid;grid-template-columns:1fr 1fr;gap:56px;align-items:start}
.ebadge{display:inline-flex;align-items:center;gap:6px;border-radius:100px;padding:6px 14px;font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:18px}
.edate{font-size:13px;color:var(--gray);margin-bottom:10px;font-weight:600}
.etitle{font-family:'Syne',sans-serif;font-size:clamp(26px,3.2vw,42px);font-weight:800;line-height:1.1;letter-spacing:-.02em;margin-bottom:8px}
.eco{font-size:14px;color:var(--gray);margin-bottom:22px;font-weight:600}
.ebl{list-style:none}
.ebl li{font-size:14px;line-height:1.8;color:rgba(255,255,255,.7);padding-left:22px;position:relative;margin-bottom:10px}
.ebl li::before{content:'→';position:absolute;left:0;font-weight:700}
.eachieve{display:inline-flex;align-items:center;gap:8px;border-radius:12px;padding:12px 18px;font-size:13px;font-weight:700;margin-top:16px;border:1.5px solid}

/* media panel */
.eright{display:flex;flex-direction:column;gap:14px}
.mup{border-radius:20px;overflow:hidden;background:rgba(255,255,255,.04);border:1.5px dashed rgba(255,255,255,.15);aspect-ratio:16/10;position:relative;cursor:pointer;transition:border-color .2s,background .2s}
.mup:hover{border-color:rgba(255,255,255,.35);background:rgba(255,255,255,.07)}
.mup img,.mup video{width:100%;height:100%;object-fit:cover;display:none}
.mup img.on,.mup video.on{display:block}
.mhint{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:10px;color:rgba(255,255,255,.3);text-align:center;padding:20px;pointer-events:none}
.mhint .mi{font-size:32px}
.mhint p{font-size:13px;line-height:1.5;font-weight:600}
.mhint span{font-size:11px;opacity:.5;letter-spacing:.1em;text-transform:uppercase}
.mcap{font-size:13px;color:rgba(255,255,255,.45);text-align:center;padding:10px 14px;background:rgba(255,255,255,.04);border-radius:10px;border:1.5px solid rgba(255,255,255,.08);cursor:text;outline:none;transition:border-color .2s}
.mcap:focus{border-color:rgba(255,255,255,.25);color:var(--w)}

/* themes */
.tpk .ebadge{background:rgba(255,107,157,.15);color:var(--pk)}.tpk .ebl li::before{color:var(--pk)}.tpk .eachieve{background:rgba(255,107,157,.1);border-color:rgba(255,107,157,.3);color:var(--pk)}.tpk .blob{background:var(--pk)}
.tbl .ebadge{background:rgba(78,205,196,.15);color:var(--bl)}.tbl .ebl li::before{color:var(--bl)}.tbl .eachieve{background:rgba(78,205,196,.1);border-color:rgba(78,205,196,.3);color:var(--bl)}.tbl .blob{background:var(--bl)}
.ty .ebadge{background:rgba(255,225,53,.15);color:var(--y)}.ty .ebl li::before{color:var(--y)}.ty .eachieve{background:rgba(255,225,53,.1);border-color:rgba(255,225,53,.3);color:var(--y)}.ty .blob{background:var(--y)}
.tor .ebadge{background:rgba(255,140,66,.15);color:var(--or)}.tor .ebl li::before{color:var(--or)}.tor .eachieve{background:rgba(255,140,66,.1);border-color:rgba(255,140,66,.3);color:var(--or)}.tor .blob{background:var(--or)}
.tpu .ebadge{background:rgba(168,85,247,.15);color:var(--pu)}.tpu .ebl li::before{color:var(--pu)}.tpu .eachieve{background:rgba(168,85,247,.1);border-color:rgba(168,85,247,.3);color:var(--pu)}.tpu .blob{background:var(--pu)}

/* GOALS */
#sg{background:#0a0a0a}
.gin{width:100%;max-width:1100px;margin:0 auto;padding:0 48px}
.gg{display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-bottom:48px}
.gc{background:rgba(255,255,255,.04);border:1.5px solid rgba(255,255,255,.08);border-radius:20px;padding:28px;transition:transform .25s}
.gc:hover{transform:translateY(-4px)}
.gtype{font-size:11px;text-transform:uppercase;letter-spacing:.15em;font-weight:700;margin-bottom:10px}
.gtext{font-family:'Syne',sans-serif;font-size:18px;font-weight:700;line-height:1.55;color:var(--w)}
.gc:nth-child(1) .gtype{color:var(--y)}.gc:nth-child(2) .gtype{color:var(--bl)}
.lrow{display:flex;gap:12px;flex-wrap:wrap}
.lpill{display:flex;flex-direction:column;background:rgba(255,255,255,.05);border:1.5px solid rgba(255,255,255,.1);border-radius:14px;padding:14px 20px}
.ln{font-weight:700;font-size:14px;color:var(--w)}.ll{font-size:12px;color:var(--gray);margin-top:2px}

/* CONTACT */
#sc{scroll-snap-align:start;min-height:100vh;display:flex;align-items:center;justify-content:center;text-align:center;padding:80px 40px;background:var(--y)}
.ci{max-width:700px}
.cey{font-size:11px;letter-spacing:.2em;text-transform:uppercase;color:rgba(0,0,0,.45);font-weight:700;margin-bottom:20px}
.ch{font-family:'Syne',sans-serif;font-size:clamp(52px,8vw,104px);font-weight:800;line-height:.93;letter-spacing:-.03em;color:var(--dark);margin-bottom:44px}
.clinks{display:flex;flex-direction:column;gap:14px;align-items:center}
.clink{display:inline-flex;align-items:center;gap:12px;background:var(--dark);color:var(--y);border-radius:100px;padding:16px 32px;font-size:15px;font-weight:700;text-decoration:none;transition:transform .2s,box-shadow .2s;font-family:'Syne',sans-serif}
.clink:hover{transform:translateY(-3px);box-shadow:0 16px 40px rgba(0,0,0,.3)}
.clink svg{width:18px;height:18px;flex-shrink:0}

/* SCROLL HINT */
.shi{position:absolute;bottom:28px;left:50%;transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;gap:6px;color:rgba(255,255,255,.25);font-size:11px;letter-spacing:.15em;text-transform:uppercase;animation:bob 2s ease-in-out infinite}
@keyframes bob{0%,100%{transform:translateX(-50%) translateY(0)}50%{transform:translateX(-50%) translateY(-7px)}}
.shi svg{width:20px;height:20px}

/* TOOLBAR */
.tb{position:fixed;bottom:24px;left:50%;transform:translateX(-50%);z-index:300;background:rgba(18,18,18,.96);backdrop-filter:blur(20px);border:1px solid rgba(255,255,255,.1);border-radius:100px;padding:10px 22px;display:flex;align-items:center;gap:14px;font-size:12px;color:rgba(255,255,255,.45);box-shadow:0 20px 60px rgba(0,0,0,.5)}
.tbd{width:7px;height:7px;background:var(--y);border-radius:50%;animation:pp 2s ease-in-out infinite}
@keyframes pp{0%,100%{opacity:1}50%{opacity:.35}}

/* EDITABLE */
[contenteditable="true"]{outline:none;transition:background .2s;border-radius:4px}
[contenteditable="true"]:hover{background:rgba(255,255,255,.05)}
[contenteditable="true"]:focus{background:rgba(255,255,255,.09);box-shadow:0 0 0 2px rgba(255,225,53,.4)}

@media(max-width:768px){
  nav{padding:14px 20px}
  .hi,.ein{grid-template-columns:1fr;gap:32px}
  .hphoto{display:none}
  .slide{padding:80px 0 32px}
  .sh,.sc,.ein,.gin{padding:0 20px}
  .bento{grid-template-columns:1fr 1fr}
  .tile.big{grid-column:span 2}
  .gg{grid-template-columns:1fr}
  #sc{padding:80px 24px}
}
</style>
</head>
<body>

<nav>
  <a href="#s0" class="logo">KT ✦</a>
  <div style="display:flex;align-items:center;gap:12px">
    <div class="ndots" id="nd"></div>
    <span class="ncnt" id="nc">01 / 09</span>
  </div>
</nav>

<!-- ── HERO ── -->
<section class="slide" id="s0">
  <div class="blob" style="width:520px;height:520px;background:var(--y);top:-120px;right:-100px;opacity:.12"></div>
  <div class="blob" style="width:320px;height:320px;background:var(--pk);bottom:-60px;left:-80px;opacity:.1"></div>
  <div class="hi">
    <div>
      <div class="htag">✦ Digital Marketer · HCM City</div>
      <h1 class="hname">Hello,<br>I'm <span class="stroke">Kim</span><br>Tuyen</h1>
      <p class="hdesc" contenteditable="true">Soon-to-be Marketing graduate từ Van Lang University. Đam mê consumer behavior, SEO và xây dựng brand story qua data-driven strategies.</p>
      <div class="hbtns">
        <a href="#sc" class="btn by">Let's talk 👋</a>
        <a href="#s2" class="btn bg">Xem kinh nghiệm ↓</a>
      </div>
      <div class="stats">
        <div><div class="sn" contenteditable="true">3.2</div><div class="sl">GPA / 4.0</div></div>
        <div><div class="sn" contenteditable="true">2+</div><div class="sl">Internships</div></div>
        <div><div class="sn" contenteditable="true">2</div><div class="sl">Projects led</div></div>
        <div><div class="sn">5K+</div><div class="sl">Organic reach</div></div>
      </div>
    </div>
    <div class="hphoto">
      <div class="hframe" id="hframe">
        <img id="himg" alt="Kim Tuyen">
        <div class="upzone" id="uhint">
          <div class="ico">🙋‍♀️</div>
          <p>Upload ảnh của bạn</p>
          <span>Click để chọn</span>
        </div>
      </div>
      <div class="chip c1">✦ SEO</div>
      <div class="chip c2">📊 Analytics</div>
      <div class="chip c3">🎨 Content</div>
    </div>
  </div>
  <div class="shi">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12l7 7 7-7"/></svg>scroll
  </div>
  <input type="file" id="hfile" accept="image/*" style="display:none">
</section>

<!-- ── SKILLS ── -->
<section class="slide" id="s1">
  <div class="blob" style="width:420px;height:420px;background:var(--bl);top:50%;left:50%;transform:translate(-50%,-50%);opacity:.08"></div>
  <div style="width:100%">
    <div class="sh"><div class="slabel" style="color:var(--bl)">✦ Skills & Tools</div><h2 class="stitle">What I <span style="color:var(--bl)">bring</span></h2></div>
    <div class="sc">
      <div class="bento">
        <div class="tile big t1"><div class="temi">🔍</div><div class="tname">SEO & Digital Strategy</div><div class="tdesc">On-page, backlinks, internal linking — thực chiến tại Ecxo Agency trên dự án NAT Center</div><div class="ttags"><span class="ttag">SEMrush</span><span class="ttag">On-page</span><span class="ttag">Backlinks</span><span class="ttag">Google Analytics</span></div></div>
        <div class="tile t2"><div class="temi">📱</div><div class="tname">Social Media</div><div class="tdesc">Content calendar, organic growth, Instagram & TikTok algorithm</div><div class="ttags"><span class="ttag">Instagram</span><span class="ttag">TikTok</span><span class="ttag">KOL</span></div></div>
        <div class="tile t3"><div class="temi">📊</div><div class="tname">Data Analytics</div><div class="tdesc">Biến data thành insight — phân tích thị trường, giá, hành vi NTD</div><div class="ttags"><span class="ttag">Tableau</span><span class="ttag">RapidMiner</span><span class="ttag">GA4</span></div></div>
        <div class="tile t4"><div class="temi">🧠</div><div class="tname">Market Research</div><div class="tdesc">Consumer behavior, competitive intelligence, international markets</div><div class="ttags"><span class="ttag">SWOT</span><span class="ttag">Ansoff</span><span class="ttag">IMC</span><span class="ttag">SMART</span></div></div>
        <div class="tile t5"><div class="temi">✍️</div><div class="tname">Content Creation</div><div class="tdesc">Visual assets, video editing tối ưu thuật toán social</div><div class="ttags"><span class="ttag">Canva</span><span class="ttag">CapCut</span><span class="ttag">Video</span></div></div>
        <div class="tile t6"><div class="temi">💼</div><div class="tname">Sales Planning</div><div class="tdesc">Kế hoạch bán hàng, phân tích kênh GT/MT/Online, chiết khấu</div><div class="ttags"><span class="ttag">Zoho CRM</span><span class="ttag">Kênh phân phối</span></div></div>
      </div>
    </div>
  </div>
</section>

<!-- ── EXP 1: Skill Direct ── -->
<section class="slide eslide tpk" id="s2">
  <div class="blob" style="width:500px;height:500px;top:-120px;right:-100px;opacity:.1"></div>
  <div class="ein">
    <div>
      <div class="ebadge">📍 Internship · 01</div>
      <div class="edate" contenteditable="true">10/2025 — 01/2026</div>
      <h2 class="etitle" contenteditable="true">Digital Marketing Intern</h2>
      <div class="eco" contenteditable="true">Skill Direct · Ho Chi Minh City</div>
      <ul class="ebl">
        <li contenteditable="true">Nghiên cứu sâu nền tảng Instagram, xây dựng content calendar hàng tháng và định hướng sáng tạo</li>
        <li contenteditable="true">Sản xuất visual assets chất lượng cao bằng Canva & CapCut, tối ưu cho thuật toán Instagram</li>
        <li contenteditable="true">Quản lý community engagement và theo dõi performance metrics để tối ưu nội dung</li>
      </ul>
      <div class="eachieve">🚀 <span contenteditable="true">5,000+ organic reach tháng đầu cho tài khoản du học Úc mới</span></div>
    </div>
    <div class="eright">
      <div class="mup" id="mu-s2">
        <img id="mi-s2" alt=""><video id="mv-s2" controls></video>
        <div class="mhint"><div class="mi">🖼️</div><p>Upload ảnh hoặc video<br>kinh nghiệm này</p><span>JPG · PNG · MP4 · MOV</span></div>
      </div>
      <div class="mcap" contenteditable="true">Thêm caption cho ảnh/video...</div>
    </div>
  </div>
</section>

<!-- ── EXP 2: Ecxo Agency ── -->
<section class="slide eslide tbl" id="s3">
  <div class="blob" style="width:480px;height:480px;bottom:-100px;left:-100px;opacity:.1"></div>
  <div class="ein">
    <div>
      <div class="ebadge">🔍 Internship · 02</div>
      <div class="edate" contenteditable="true">03/2025 — 07/2025</div>
      <h2 class="etitle" contenteditable="true">SEO Intern</h2>
      <div class="eco" contenteditable="true">Ecxo Agency · Ho Chi Minh City</div>
      <ul class="ebl">
        <li contenteditable="true">Tham gia dự án SEO của NAT Center — thực hiện on-page SEO, internal links, backlinks</li>
        <li contenteditable="true">Phân tích hiệu suất từ khóa và hỗ trợ tối ưu hóa nội dung liên tục</li>
        <li contenteditable="true">Làm việc trực tiếp với team để cải thiện thứ hạng tìm kiếm organic</li>
      </ul>
      <div class="eachieve">🎯 <span contenteditable="true">Cải thiện on-page SEO & cấu trúc internal link cho NAT Center</span></div>
    </div>
    <div class="eright">
      <div class="mup" id="mu-s3">
        <img id="mi-s3" alt=""><video id="mv-s3" controls></video>
        <div class="mhint"><div class="mi">📸</div><p>Upload ảnh hoặc video<br>kinh nghiệm này</p><span>JPG · PNG · MP4 · MOV</span></div>
      </div>
      <div class="mcap" contenteditable="true">Thêm caption cho ảnh/video...</div>
    </div>
  </div>
</section>

<!-- ── PROJECT 1: ORION ── -->
<section class="slide eslide tor" id="s4">
  <div class="blob" style="width:520px;height:520px;top:-150px;right:-80px;opacity:.09"></div>
  <div class="ein">
    <div>
      <div class="ebadge">👑 Leader · Quản trị Bán hàng</div>
      <div class="edate" contenteditable="true">2025 · Nhóm 10/10 · 9 thành viên</div>
      <h2 class="etitle" contenteditable="true">Kế hoạch Bán hàng 2026<br>ORION Việt Nam</h2>
      <div class="eco" contenteditable="true">Van Lang University · Group Leader</div>
      <ul class="ebl">
        <li contenteditable="true">Lead nhóm xây dựng kế hoạch bán hàng 2026 cho ORION — thương hiệu số 1 VN, 66% thị phần ChocoPie</li>
        <li contenteditable="true">Mục tiêu SMART: tăng doanh thu ròng 15%, lợi nhuận gộp ≥35%, tăng 1,5% thị phần Q4/2026</li>
        <li contenteditable="true">Chiến lược phân kênh: GT 60% / MT 25% / TMĐT 15% — đề xuất TikTok Shop là kênh tăng trưởng chiến lược</li>
        <li contenteditable="true">Phân tích SWOT, đối thủ (Mondelez, Lotte, Kinh Đô), hành vi tiêu dùng Gen Z</li>
      </ul>
      <div class="eachieve">🏆 <span contenteditable="true">Leader — 100% thành viên đóng góp đầy đủ</span></div>
    </div>
    <div class="eright">
      <div class="mup" id="mu-s4">
        <img id="mi-s4" alt=""><video id="mv-s4" controls></video>
        <div class="mhint"><div class="mi">📊</div><p>Upload slide hoặc video<br>thuyết trình dự án</p><span>JPG · PNG · MP4 · MOV</span></div>
      </div>
      <div class="mcap" contenteditable="true">Dự án Quản trị Bán hàng — ORION Việt Nam 2026</div>
    </div>
  </div>
</section>

<!-- ── PROJECT 2: VINAMIT ── -->
<section class="slide eslide tpu" id="s5">
  <div class="blob" style="width:500px;height:500px;bottom:-100px;left:-80px;opacity:.09"></div>
  <div class="ein">
    <div>
      <div class="ebadge">👑 Leader · Marketing Quốc Tế</div>
      <div class="edate" contenteditable="true">2025 · Nhóm 8 · 8 thành viên</div>
      <h2 class="etitle" contenteditable="true">Chiến lược thâm nhập<br>Hàn Quốc — Vinamit</h2>
      <div class="eco" contenteditable="true">Van Lang University · Group Leader</div>
      <ul class="ebl">
        <li contenteditable="true">Lead nhóm chiến lược Marketing quốc tế cho Vinamit sấy dẻo thâm nhập thị trường Hàn Quốc</li>
        <li contenteditable="true">Phụ trách Chiến lược Giá: phân tích đối thủ TROO, THEHARU, Irosam; nghiên cứu hành vi NTD Hàn (healthy/organic)</li>
        <li contenteditable="true">Xây dựng cấu trúc giá xuất khẩu: COGS → FOB → CIF → SRP tại Hàn (₩4,205–₩4,995/100g), tối ưu VKFTA 10%</li>
        <li contenteditable="true">Phân tích price elasticity theo kênh Coupang/Naver vs GS25; thị trường snack Hàn USD 5,67 tỷ</li>
      </ul>
      <div class="eachieve">🌏 <span contenteditable="true">Chiến lược giá thâm nhập thị trường Hàn Quốc</span></div>
    </div>
    <div class="eright">
      <div class="mup" id="mu-s5">
        <img id="mi-s5" alt=""><video id="mv-s5" controls></video>
        <div class="mhint"><div class="mi">🇰🇷</div><p>Upload slide hoặc video<br>thuyết trình dự án</p><span>JPG · PNG · MP4 · MOV</span></div>
      </div>
      <div class="mcap" contenteditable="true">Marketing Quốc Tế — Vinamit × Hàn Quốc</div>
    </div>
  </div>
</section>

<!-- ── PROJECT 3: Legendary Chocolatier ── -->
<section class="slide eslide ty" id="s6">
  <div class="blob" style="width:450px;height:450px;top:50%;right:-80px;transform:translateY(-50%);opacity:.09"></div>
  <div class="ein">
    <div>
      <div class="ebadge">🍫 Academic Project</div>
      <div class="edate" contenteditable="true">2024 · 3 tháng</div>
      <h2 class="etitle" contenteditable="true">Social Media Plan<br>Legendary Chocolatier</h2>
      <div class="eco" contenteditable="true">Van Lang University · Marketing Project</div>
      <ul class="ebl">
        <li contenteditable="true">Xây dựng kế hoạch social media marketing toàn diện trong 3 tháng</li>
        <li contenteditable="true">Phân tích thị trường và xác định target audience, brand positioning</li>
        <li contenteditable="true">Lập chiến lược nội dung, lịch đăng bài và kế hoạch quảng cáo</li>
      </ul>
      <div class="eachieve">🎨 <span contenteditable="true">Comprehensive social media marketing plan</span></div>
    </div>
    <div class="eright">
      <div class="mup" id="mu-s6">
        <img id="mi-s6" alt=""><video id="mv-s6" controls></video>
        <div class="mhint"><div class="mi">🍫</div><p>Upload ảnh hoặc video<br>dự án này</p><span>JPG · PNG · MP4 · MOV</span></div>
      </div>
      <div class="mcap" contenteditable="true">Legendary Chocolatier — Social Media Strategy</div>
    </div>
  </div>
</section>

<!-- ── GOALS ── -->
<section class="slide" id="sg">
  <div class="blob" style="width:360px;height:360px;background:var(--pu);bottom:0;right:0;opacity:.09"></div>
  <div style="width:100%">
    <div class="sh"><div class="slabel" style="color:var(--y)">✦ Goals & Vision</div><h2 class="stitle">Where I'm <span style="color:var(--y)">headed →</span></h2></div>
    <div class="gin">
      <div class="gg">
        <div class="gc"><div class="gtype">⚡ Short-term</div><div class="gtext" contenteditable="true">Xây dựng nền tảng vững chắc về SEO và social media để chuẩn bị cho chuyên môn hóa trong tương lai.</div></div>
        <div class="gc"><div class="gtype">🚀 Long-term</div><div class="gtext" contenteditable="true">Trở thành SEO Specialist hoặc Social Media Marketing Manager, dẫn dắt và mentoring một team.</div></div>
      </div>
      <div class="slabel" style="color:var(--bl);margin-bottom:16px">✦ Languages</div>
      <div class="lrow">
        <div class="lpill"><div class="ln">Tiếng Việt</div><div class="ll">Native</div></div>
        <div class="lpill"><div class="ln">English</div><div class="ll">Aptis ESOL B2</div></div>
      </div>
    </div>
  </div>
</section>

<!-- ── CONTACT ── -->
<section id="sc">
  <div class="ci">
    <div class="cey">✦ Let's work together</div>
    <h2 class="ch">Ready<br>to talk?</h2>
    <div class="clinks">
      <a href="mailto:Hskimtuyen123@gmail.com" class="clink"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>Hskimtuyen123@gmail.com</a>
      <a href="https://www.linkedin.com/in/phamhoaikimtuyen/" target="_blank" class="clink"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>LinkedIn Profile</a>
      <a href="tel:+84337258994" class="clink"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07A19.5 19.5 0 013.07 9.81a19.79 19.79 0 01-3.07-8.67A2 2 0 012.18 1h3a2 2 0 012 1.72c.127.96.361 1.903.7 2.81a2 2 0 01-.45 2.11L6.91 8.15a16 16 0 006.29 6.29l1.51-1.51a2 2 0 012.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0122 16.92z"/></svg>+84 337 258 994</a>
    </div>
  </div>
</section>

<!-- TOOLBAR -->
<div class="tb"><div class="tbd"></div><span>Click text để sửa &nbsp;·&nbsp; Click vùng media để upload ảnh / video</span></div>

<!-- Hidden inputs -->
<input type="file" id="hfile" accept="image/*" style="display:none">
<input type="file" id="mfile" accept="image/*,video/*" style="display:none">

<script>
const SLIDES=['s0','s1','s2','s3','s4','s5','s6','sg','sc'];
const LABELS=['Home','Skills','Skill Direct','Ecxo Agency','ORION','Vinamit','Chocolatier','Goals','Contact'];

// NAV DOTS
const nd=document.getElementById('nd'),nc=document.getElementById('nc');
SLIDES.forEach((id,i)=>{
  const d=document.createElement('button');
  d.className='ndot'+(i===0?' on':'');d.title=LABELS[i];
  d.onclick=()=>document.getElementById(id).scrollIntoView({behavior:'smooth'});
  nd.appendChild(d);
});
const io=new IntersectionObserver(e=>{e.forEach(x=>{if(x.isIntersecting){const i=SLIDES.indexOf(x.target.id);if(i<0)return;document.querySelectorAll('.ndot').forEach((d,j)=>d.classList.toggle('on',j===i));nc.textContent=String(i+1).padStart(2,'0')+' / '+String(SLIDES.length).padStart(2,'0');}});},{threshold:.5});
SLIDES.forEach(id=>{const el=document.getElementById(id);if(el)io.observe(el);});

// HERO PHOTO
document.getElementById('hframe').onclick=()=>document.getElementById('hfile').click();
document.getElementById('hfile').addEventListener('change',function(e){
  const f=e.target.files[0];if(!f)return;
  const r=new FileReader();r.onload=ev=>{
    const img=document.getElementById('himg');img.src=ev.target.result;img.classList.add('on');
    document.getElementById('uhint').style.display='none';
  };r.readAsDataURL(f);
});

// MEDIA UPLOADS
let curSlot=null;
['s2','s3','s4','s5','s6'].forEach(id=>{
  document.getElementById('mu-'+id).addEventListener('click',function(){
    curSlot=id;document.getElementById('mfile').value='';document.getElementById('mfile').click();
  });
});
document.getElementById('mfile').addEventListener('change',function(e){
  const f=e.target.files[0];if(!f||!curSlot)return;
  const isVid=f.type.startsWith('video/');
  const r=new FileReader();r.onload=ev=>{
    const wrap=document.getElementById('mu-'+curSlot);
    wrap.querySelector('.mhint').style.display='none';
    if(isVid){
      const v=document.getElementById('mv-'+curSlot);v.src=ev.target.result;v.classList.add('on');
      document.getElementById('mi-'+curSlot).classList.remove('on');
    } else {
      const i=document.getElementById('mi-'+curSlot);i.src=ev.target.result;i.classList.add('on');
      document.getElementById('mv-'+curSlot).classList.remove('on');
    }
  };r.readAsDataURL(f);
});

// FADE IN
const fels=document.querySelectorAll('.tile,.ein>div,.gc');
const fobs=new IntersectionObserver(e=>{e.forEach(x=>{if(x.isIntersecting){x.target.style.opacity='1';x.target.style.transform='translateY(0)';}});},{threshold:.1});
fels.forEach(el=>{el.style.opacity='0';el.style.transform='translateY(24px)';el.style.transition='opacity .55s ease,transform .55s ease';fobs.observe(el);});
</script>
</body>
</html>
