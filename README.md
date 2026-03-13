<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Hoài Đặng</title>
  <meta name="description" content="Hoài Đặng - Chia sẻ cuộc sống người Việt tại Mỹ, công việc, kinh doanh tiệm nail và những trải nghiệm thật tại Texas." />
  <meta name="theme-color" content="#6d28d9" />

  <meta property="og:title" content="Hoài Đặng" />
  <meta property="og:description" content="Chia sẻ cuộc sống người Việt tại Mỹ, công việc, kinh doanh tiệm nail và những trải nghiệm thật tại Texas." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://hoaidang.com" />
  <meta property="og:image" content="https://hoaidang.com/profile.jpg" />

  <style>
    * {
      box-sizing: border-box;
    }

    :root {
      --bg1: #4f46e5;
      --bg2: #7c3aed;
      --bg3: #ec4899;
      --card: rgba(255, 255, 255, 0.14);
      --card-border: rgba(255, 255, 255, 0.2);
      --text: #ffffff;
      --muted: rgba(255, 255, 255, 0.9);
      --shadow: 0 20px 50px rgba(0, 0, 0, 0.24);
    }

    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
      color: var(--text);
      min-height: 100vh;
      background:
        radial-gradient(circle at 0% 0%, rgba(255,255,255,0.18), transparent 28%),
        radial-gradient(circle at 100% 0%, rgba(255,220,160,0.18), transparent 26%),
        radial-gradient(circle at 50% 100%, rgba(255,255,255,0.10), transparent 25%),
        linear-gradient(135deg, var(--bg1) 0%, var(--bg2) 48%, var(--bg3) 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
    }

    .wrap {
      width: 100%;
      max-width: 560px;
    }

    .card {
      background: var(--card);
      border: 1px solid var(--card-border);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border-radius: 30px;
      box-shadow: var(--shadow);
      padding: 28px 22px 24px;
      text-align: center;
      overflow: hidden;
      position: relative;
    }

    .card::before {
      content: "";
      position: absolute;
      top: -70px;
      left: -70px;
      width: 180px;
      height: 180px;
      background: rgba(255,255,255,0.12);
      border-radius: 50%;
      filter: blur(8px);
    }

    .card::after {
      content: "";
      position: absolute;
      right: -60px;
      bottom: -60px;
      width: 160px;
      height: 160px;
      background: rgba(255,255,255,0.10);
      border-radius: 50%;
      filter: blur(8px);
    }

    .top {
      position: relative;
      z-index: 1;
    }

    .avatar-ring {
      width: 132px;
      height: 132px;
      margin: 0 auto 14px;
      border-radius: 50%;
      padding: 5px;
      background: linear-gradient(135deg, rgba(255,255,255,0.95), rgba(255,255,255,0.45));
      box-shadow: 0 12px 30px rgba(0,0,0,0.18);
    }

    .avatar {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
      display: block;
      background: rgba(255,255,255,0.18);
    }

    h1 {
      margin: 0;
      font-size: 36px;
      line-height: 1.05;
      letter-spacing: 0.2px;
    }

    .tagline {
      margin: 10px auto 0;
      display: inline-block;
      padding: 8px 14px;
      border-radius: 999px;
      background: rgba(255,255,255,0.14);
      border: 1px solid rgba(255,255,255,0.14);
      font-size: 13px;
      font-weight: 700;
      color: #fff;
    }

    .desc {
      margin: 16px auto 22px;
      max-width: 440px;
      font-size: 15px;
      line-height: 1.65;
      color: var(--muted);
    }

    .links {
      position: relative;
      z-index: 1;
      display: grid;
      gap: 14px;
      margin-top: 4px;
    }

    .btn {
      text-decoration: none;
      color: #1c1c1c;
      background: rgba(255,255,255,0.96);
      border-radius: 20px;
      padding: 15px 16px;
      display: flex;
      align-items: center;
      gap: 14px;
      box-shadow: 0 12px 26px rgba(0,0,0,0.14);
      transition: transform 0.18s ease, box-shadow 0.18s ease, background 0.18s ease;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 16px 30px rgba(0,0,0,0.18);
      background: #ffffff;
    }

    .btn:active {
      transform: translateY(0);
    }

    .icon {
      width: 42px;
      height: 42px;
      border-radius: 14px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-weight: 800;
      font-size: 14px;
      flex-shrink: 0;
    }

    .meta {
      text-align: left;
      flex: 1;
    }

    .meta strong {
      display: block;
      font-size: 16px;
      line-height: 1.2;
    }

    .meta span {
      display: block;
      margin-top: 3px;
      font-size: 13px;
      color: #666;
      line-height: 1.4;
    }

    .arrow {
      font-size: 20px;
      color: #999;
      flex-shrink: 0;
    }

    .tiktok .icon {
      background: linear-gradient(135deg, #111111, #333333);
    }

    .facebook .icon {
      background: linear-gradient(135deg, #1877f2, #3b82f6);
    }

    .youtube .icon {
      background: linear-gradient(135deg, #ff0000, #ff4d4d);
    }

    .nails .icon {
      background: linear-gradient(135deg, #db2777, #f472b6);
    }

    .email .icon {
      background: linear-gradient(135deg, #10b981, #34d399);
    }

    .bottom {
      position: relative;
      z-index: 1;
      margin-top: 22px;
      padding-top: 18px;
      border-top: 1px solid rgba(255,255,255,0.16);
      color: rgba(255,255,255,0.92);
    }

    .location {
      font-size: 14px;
      font-weight: 700;
      letter-spacing: 0.2px;
    }

    .mini {
      margin-top: 6px;
      font-size: 13px;
      color: rgba(255,255,255,0.85);
      line-height: 1.5;
    }

    @media (max-width: 560px) {
      body {
        padding: 16px;
      }

      .card {
        padding: 24px 16px 20px;
        border-radius: 24px;
      }

      .avatar-ring {
        width: 118px;
        height: 118px;
      }

      h1 {
        font-size: 31px;
      }

      .btn {
        padding: 14px 14px;
        border-radius: 18px;
      }

      .icon {
        width: 40px;
        height: 40px;
        border-radius: 12px;
      }

      .meta strong {
        font-size: 15px;
      }

      .meta span {
        font-size: 12px;
      }
    }
  </style>

  <script type="application/ld+json">
  {
    "@context":"https://schema.org",
    "@type":"Person",
    "name":"Hoài Đặng",
    "alternateName":"Hoai Dang",
    "url":"https://hoaidang.com",
    "jobTitle":"Content Creator",
    "description":"Vietnamese entrepreneur and content creator based in Odessa, Texas, sharing real-life experiences about living and working in America.",
    "address":{
      "@type":"PostalAddress",
      "addressLocality":"Odessa",
      "addressRegion":"Texas",
      "addressCountry":"US"
    },
    "sameAs":[
      "https://www.tiktok.com/@hoaidangllc",
      "https://www.facebook.com/hoaidangllc",
      "https://www.youtube.com/@hoaidangllc",
      "https://annienail.com",
      "https://github.com/hoaidangllc"
    ]
  }
  </script>
</head>
<body>
  <div class="wrap">
    <main class="card">
      <div class="top">
        <div class="avatar-ring">
          <img class="avatar" src="profile.jpg" alt="Hoài Đặng">
        </div>

        <h1>Hoài Đặng</h1>

        <div class="tagline">Cuộc sống ở Mỹ • Kinh doanh • Chuyện thật mỗi ngày</div>

        <p class="desc">
          Chia sẻ cuộc sống người Việt tại Mỹ, công việc, kinh doanh tiệm nail
          và những góc nhìn rất thật ở Texas.
        </p>
      </div>

      <section class="links">
        <a class="btn tiktok" href="https://www.tiktok.com/@hoaidangllc" target="_blank" rel="noopener noreferrer">
          <div class="icon">TT</div>
          <div class="meta">
            <strong>TikTok</strong>
            <span>Xem video ngắn về cuộc sống và công việc tại Mỹ</span>
          </div>
          <div class="arrow">›</div>
        </a>

        <a class="btn facebook" href="https://www.facebook.com/hoaidangllc" target="_blank" rel="noopener noreferrer">
          <div class="icon">f</div>
          <div class="meta">
            <strong>Facebook</strong>
            <span>Theo dõi bài viết, video và những chia sẻ hằng ngày</span>
          </div>
          <div class="arrow">›</div>
        </a>

        <a class="btn youtube" href="https://www.youtube.com/@hoaidangllc" target="_blank" rel="noopener noreferrer">
          <div class="icon">YT</div>
          <div class="meta">
            <strong>YouTube</strong>
            <span>Xem thêm nội dung dài hơn và kênh video của Hoài</span>
          </div>
          <div class="arrow">›</div>
        </a>

        <a class="btn nails" href="https://annienail.com" target="_blank" rel="noopener noreferrer">
          <div class="icon">NS</div>
          <div class="meta">
            <strong>Annie’s Nails &amp; Spa</strong>
            <span>Website chính thức của tiệm nail tại Odessa, Texas</span>
          </div>
          <div class="arrow">›</div>
        </a>

        <a class="btn email" href="mailto:info@annienail.com">
          <div class="icon">@</div>
          <div class="meta">
            <strong>Liên hệ</strong>
            <span>info@annienail.com</span>
          </div>
          <div class="arrow">›</div>
        </a>
      </section>

      <div class="bottom">
        <div class="location">Odessa, Texas – USA</div>
        <div class="mini">Vietnamese creator & entrepreneur</div>
      </div>
    </main>
  </div>
</body>
</html>
