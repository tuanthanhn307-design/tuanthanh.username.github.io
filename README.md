
<!DOCTYPE html>
<html lang="vi" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Nguyễn Tuấn Thanh | 11T2 — Nhiếp ảnh, STEM &amp; Bóng chuyền</title>
  <meta name="description" content="Trang giới thiệu bản thân của Nguyễn Tuấn Thanh - Học sinh lớp 11T2, Trường THPT Chuyên Bến Tre tại Vĩnh Long. Đam mê Nhiếp ảnh, STEM, Thiết kế 3D &amp; Lập trình sáng tạo và Bóng chuyền (Chuyền 2)." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet" />

  <style>
    :root {
      --bg-primary: #0b0f17;
      --bg-secondary: #131a26;
      --bg-card: rgba(20, 28, 43, 0.85);
      --header-bg: rgba(11, 15, 23, 0.85);
      --text-primary: #f1f5f9;
      --text-secondary: #94a3b8;
      --accent-stem: #38bdf8;
      --accent-photo: #f59e0b;
      --accent-volley: #a78bfa;
      --accent-creative: #fb7185;
      --accent-charity: #34d399;
      --border-color: rgba(148, 163, 184, 0.16);
      --grid-color: rgba(56, 189, 248, 0.05);
      --shadow: 0 12px 32px rgba(0, 0, 0, 0.35);
    }

    [data-theme="light"] {
      --bg-primary: #f8fafc;
      --bg-secondary: #ffffff;
      --bg-card: rgba(255, 255, 255, 0.95);
      --header-bg: rgba(248, 250, 252, 0.88);
      --text-primary: #0f172a;
      --text-secondary: #475569;
      --accent-stem: #0284c7;
      --accent-photo: #d97706;
      --accent-volley: #7c3aed;
      --accent-creative: #e11d48;
      --accent-charity: #059669;
      --border-color: rgba(15, 23, 42, 0.12);
      --grid-color: rgba(2, 132, 199, 0.06);
      --shadow: 0 10px 25px rgba(15, 23, 42, 0.08);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
      scroll-padding-top: 84px;
      font-family: 'Inter', system-ui, -apple-system, sans-serif;
    }

    body {
      background-color: var(--bg-primary);
      color: var(--text-primary);
      line-height: 1.65;
      background-image:
        linear-gradient(to right, var(--grid-color) 1px, transparent 1px),
        linear-gradient(to bottom, var(--grid-color) 1px, transparent 1px);
      background-size: 36px 36px;
      transition: background-color 0.25s ease, color 0.25s ease;
    }

    .mono {
      font-family: 'JetBrains Mono', monospace;
    }

    .container {
      max-width: 1080px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* Header & Mobile Menu */
    header {
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      background: var(--header-bg);
      border-bottom: 1px solid var(--border-color);
    }

    .nav-wrapper {
      display: flex;
      justify-content: space-between;
      align-items: center;
      min-height: 68px;
      gap: 12px;
    }

    .logo {
      font-weight: 800;
      font-size: 1.15rem;
      letter-spacing: -0.02em;
      text-decoration: none;
      color: var(--text-primary);
      display: inline-flex;
      align-items: center;
      gap: 8px;
      white-space: nowrap;
    }

    .logo-badge {
      font-size: 0.72rem;
      padding: 2px 8px;
      border-radius: 6px;
      background: rgba(56, 189, 248, 0.14);
      color: var(--accent-stem);
      border: 1px solid rgba(56, 189, 248, 0.3);
    }

    .nav-right {
      display: flex;
      align-items: center;
      gap: 18px;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 18px;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--text-secondary);
      font-size: 0.9rem;
      font-weight: 500;
      transition: color 0.2s ease;
      white-space: nowrap;
    }

    .nav-links a:hover {
      color: var(--accent-stem);
    }

    .btn-icon {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      color: var(--text-primary);
      padding: 7px 12px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 0.85rem;
      font-weight: 600;
      transition: transform 0.2s ease, border-color 0.2s ease;
      white-space: nowrap;
    }

    .btn-icon:hover {
      border-color: var(--accent-stem);
      transform: translateY(-1px);
    }

    .menu-toggle {
      display: none;
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      color: var(--text-primary);
      padding: 7px 11px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
      line-height: 1;
    }

    .mobile-menu {
      display: none;
      flex-direction: column;
      padding: 12px 20px 18px;
      border-top: 1px solid var(--border-color);
      background: var(--header-bg);
      gap: 10px;
    }

    .mobile-menu.open {
      display: flex;
    }

    .mobile-menu a {
      text-decoration: none;
      color: var(--text-primary);
      padding: 8px 4px;
      font-weight: 500;
      border-bottom: 1px solid var(--border-color);
    }

    .mobile-menu a:last-child {
      border-bottom: none;
    }

    /* Hero Section */
    .hero {
      padding: 68px 0 52px;
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 40px;
      align-items: center;
    }

    .status-pill {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      font-size: 0.8rem;
      padding: 6px 14px;
      border-radius: 999px;
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      color: var(--accent-stem);
      margin-bottom: 18px;
    }

    .dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--accent-photo);
      box-shadow: 0 0 8px var(--accent-photo);
      flex-shrink: 0;
    }

    h1 {
      font-size: clamp(2rem, 4.2vw, 3rem);
      font-weight: 800;
      line-height: 1.15;
      letter-spacing: -0.03em;
      margin-bottom: 16px;
    }

    .highlight-stem {
      color: var(--accent-stem);
    }

    .highlight-photo {
      color: var(--accent-photo);
    }

    .highlight-volley {
      color: var(--accent-volley);
    }

    .highlight-creative {
      color: var(--accent-creative);
    }

    .hero-desc {
      color: var(--text-secondary);
      font-size: 1.03rem;
      margin-bottom: 28px;
      max-width: 560px;
    }

    .cta-group {
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 12px 20px;
      border-radius: 10px;
      font-weight: 600;
      font-size: 0.94rem;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.2s ease;
      border: 1px solid transparent;
    }

    .btn-primary {
      background: var(--accent-stem);
      color: #08101c;
    }

    .btn-primary:hover {
      filter: brightness(1.08);
      transform: translateY(-2px);
    }

    .btn-outline {
      background: var(--bg-card);
      color: var(--text-primary);
      border-color: var(--border-color);
    }

    .btn-outline:hover {
      border-color: var(--accent-photo);
      transform: translateY(-2px);
    }

    /* Camera Viewfinder Card */
    .viewfinder {
      position: relative;
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: 18px;
      padding: 16px;
      box-shadow: var(--shadow);
    }

    .vf-header, .vf-footer {
      display: flex;
      justify-content: space-between;
      font-size: 0.75rem;
      color: var(--text-secondary);
      padding: 4px 6px;
    }

    .vf-rec {
      color: #ef4444;
      font-weight: 600;
    }

    .avatar-box {
      position: relative;
      width: 100%;
      aspect-ratio: 4 / 4.5;
      border-radius: 12px;
      overflow: hidden;
      margin: 8px 0;
      background: linear-gradient(135deg, #1e293b, #0f172a);
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .avatar-box img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center 22%;
      display: block;
    }

    .crosshair {
      position: absolute;
      inset: 14px;
      border: 1px dashed rgba(245, 158, 11, 0.5);
      border-radius: 8px;
      pointer-events: none;
    }

    /* Sections */
    section {
      padding: 52px 0;
    }

    .section-header {
      margin-bottom: 28px;
    }

    .section-tag {
      font-size: 0.8rem;
      letter-spacing: 0.08em;
      color: var(--accent-stem);
      font-weight: 600;
      display: block;
      margin-bottom: 6px;
    }

    .section-title {
      font-size: 1.7rem;
      font-weight: 800;
      letter-spacing: -0.02em;
    }

    /* Info Strip */
    .info-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 16px;
    }

    .info-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      padding: 20px;
      border-radius: 14px;
      transition: transform 0.2s ease, border-color 0.2s ease;
    }

    .info-card:hover {
      transform: translateY(-3px);
      border-color: var(--accent-stem);
    }

    .info-label {
      font-size: 0.82rem;
      color: var(--text-secondary);
      margin-bottom: 4px;
    }

    .info-value {
      font-weight: 700;
      font-size: 1.05rem;
    }

    .info-value a {
      color: inherit;
      text-decoration: none;
    }

    .info-value a:hover {
      color: var(--accent-stem);
    }

    /* Skills & Gear Grids */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 24px;
    }

    .gear-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
    }

    .skill-panel,
    .gear-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: 16px;
      padding: 26px;
      box-shadow: var(--shadow);
    }

    .skill-panel.stem {
      border-top: 3px solid var(--accent-stem);
    }

    .skill-panel.photo,
    .gear-card {
      border-top: 3px solid var(--accent-photo);
    }

    .skill-panel.volley {
      border-top: 3px solid var(--accent-volley);
    }

    .skill-panel.creative {
      border-top: 3px solid var(--accent-creative);
    }

    .gear-tag {
      display: inline-block;
      font-size: 0.75rem;
      padding: 3px 9px;
      border-radius: 6px;
      background: rgba(245, 158, 11, 0.14);
      color: var(--accent-photo);
      border: 1px solid rgba(245, 158, 11, 0.3);
      margin-bottom: 10px;
    }

    .gear-title {
      font-size: 1.2rem;
      font-weight: 700;
      margin-bottom: 6px;
    }

    .gear-lens {
      font-size: 0.92rem;
      color: var(--accent-stem);
      font-weight: 600;
      margin-bottom: 12px;
    }

    .panel-title {
      font-size: 1.2rem;
      font-weight: 700;
      margin-bottom: 10px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .panel-desc {
      color: var(--text-secondary);
      font-size: 0.94rem;
    }

    .skill-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 12px;
      margin-top: 16px;
    }

    .skill-list li {
      padding: 12px 14px;
      border-radius: 10px;
      background: rgba(148, 163, 184, 0.07);
      border: 1px solid var(--border-color);
      font-size: 0.93rem;
      color: var(--text-secondary);
    }

    .skill-list strong {
      display: block;
      color: var(--text-primary);
      margin-bottom: 2px;
    }

    /* Gallery */
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(290px, 1fr));
      gap: 20px;
    }

    .photo-card {
      position: relative;
      border-radius: 14px;
      overflow: hidden;
      background: var(--bg-secondary);
      border: 1px solid var(--border-color);
      aspect-ratio: 16 / 11;
    }

    .photo-card img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      transition: transform 0.4s ease;
    }

    .photo-card:hover img {
      transform: scale(1.05);
    }

    .photo-overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(to top, rgba(9, 13, 22, 0.92), rgba(9, 13, 22, 0.15) 60%, transparent);
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      padding: 18px;
      color: #f8fafc;
    }

    .photo-meta {
      font-size: 0.74rem;
      color: #fbbf24;
      margin-bottom: 3px;
    }

    .photo-caption {
      font-weight: 600;
      font-size: 0.98rem;
    }

    /* Charity & Contact Box */
    .charity-grid {
      display: grid;
      grid-template-columns: 0.9fr 1.1fr;
      gap: 24px;
      align-items: center;
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-top: 3px solid var(--accent-charity);
      border-radius: 18px;
      padding: 32px 28px;
      box-shadow: var(--shadow);
    }

    .qr-frame {
      background: #ffffff;
      border-radius: 14px;
      padding: 14px;
      max-width: 280px;
      width: 100%;
      margin: 0 auto;
      border: 1px solid var(--border-color);
      text-align: center;
    }

    .qr-frame img {
      width: 100%;
      height: auto;
      display: block;
      border-radius: 8px;
    }

    .bank-details {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 10px;
      margin: 18px 0 22px;
    }

    .bank-details li {
      padding: 10px 14px;
      border-radius: 10px;
      background: rgba(148, 163, 184, 0.08);
      border: 1px solid var(--border-color);
      font-size: 0.94rem;
      color: var(--text-secondary);
    }

    .bank-details strong {
      color: var(--text-primary);
    }

    .contact-box {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: 18px;
      padding: 36px 28px;
      text-align: center;
      box-shadow: var(--shadow);
    }

    .contact-box p {
      color: var(--text-secondary);
      max-width: 560px;
      margin: 10px auto 24px;
    }

    .contact-actions {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 14px;
    }

    .copy-feedback {
      font-size: 0.85rem;
      color: var(--accent-stem);
      margin-top: 14px;
      min-height: 20px;
    }

    footer {
      border-top: 1px solid var(--border-color);
      padding: 28px 0;
      text-align: center;
      color: var(--text-secondary);
      font-size: 0.88rem;
    }

    @media (max-width: 820px) {
      .hero,
      .skills-grid,
      .charity-grid {
        grid-template-columns: 1fr;
        padding-top: 32px;
      }
      .nav-links {
        display: none;
      }
      .menu-toggle {
        display: inline-flex;
        align-items: center;
        justify-content: center;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="container nav-wrapper">
      <a href="#" class="logo">
        <span>NTT</span>
        <span class="logo-badge mono">11T2 // STEM &amp; PHOTO</span>
      </a>

      <div class="nav-right">
        <nav class="nav-links" aria-label="Điều hướng chính">
          <a href="#gioi-thieu">Giới thiệu</a>
          <a href="#ky-nang">Kỹ năng</a>
          <a href="#thiet-bi">Thiết bị</a>
          <a href="#bo-suu-tap">Góc Nhiếp ảnh</a>
          <a href="#tu-thien">Từ thiện</a>
          <a href="#lien-he">Liên hệ</a>
        </nav>
        <button type="button" class="btn-icon" id="themeToggle" aria-label="Đổi giao diện Sáng hoặc Tối">☀️ Sáng</button>
        <button type="button" class="menu-toggle" id="menuToggle" aria-label="Mở menu điều hướng" aria-expanded="false">☰</button>
      </div>
    </div>

    <!-- Mobile Navigation Drawer -->
    <nav class="mobile-menu" id="mobileMenu" aria-label="Điều hướng điện thoại">
      <a href="#gioi-thieu">Giới thiệu</a>
      <a href="#ky-nang">Năng lực &amp; Đam mê</a>
      <a href="#thiet-bi">Thiết bị Nhiếp ảnh</a>
      <a href="#bo-suu-tap">Góc Nhiếp ảnh</a>
      <a href="#tu-thien">Mã chuyển khoản từ thiện</a>
      <a href="#lien-he">Liên hệ</a>
    </nav>
  </header>

  <main class="container">
    <!-- Hero Section -->
    <section class="hero">
      <div>
        <div class="status-pill mono">
          <span class="dot"></span>
          <span>Lớp 11T2 • THPT Chuyên Bến Tre (Vĩnh Long)</span>
        </div>
        <h1>
          Xin chào, mình là <br />
          <span class="highlight-stem">Nguyễn Tuấn Thanh</span>
        </h1>
        <p class="hero-desc">
          Mình là học sinh lớp <strong>11T2</strong> tại trường <strong>THPT Chuyên Bến Tre (tỉnh Vĩnh Long)</strong>. Mình đam mê kết hợp tư duy logic của <span class="highlight-stem"><strong>STEM</strong></span>, góc nhìn sáng tạo qua ống kính <span class="highlight-photo"><strong>Nhiếp ảnh</strong></span> (<strong>Canon 5D3 + 50mm f/1.8 II</strong> &amp; <strong>Canon M200 + Lens Kit</strong>), <span class="highlight-creative"><strong>Thiết kế 3D &amp; Lập trình sáng tạo</strong></span> cùng tinh thần đồng đội ở vị trí <span class="highlight-volley"><strong>Chuyền 2 Bóng chuyền</strong></span>.
        </p>
        <div class="cta-group">
          <a href="#ky-nang" class="btn btn-primary">Khám phá năng lực &amp; đam mê</a>
          <a href="#tu-thien" class="btn btn-outline">Mã chuyển khoản từ thiện</a>
        </div>
      </div>

      <!-- Viewfinder Portrait Frame -->
      <div class="viewfinder">
        <div class="vf-header mono">
          <span class="vf-rec">● 5D3 / M200</span>
          <span>[ 50MM f/1.8 II • KIT ]</span>
          <span>RAW</span>
        </div>
        <div class="avatar-box">
          <img
            id="avatarImg"
            src="images/anh-dai-dien.jpg"
            alt="Ảnh đại diện Nguyễn Tuấn Thanh"
          />
          <div class="crosshair"></div>
        </div>
        <div class="vf-footer mono">
          <span>ISO 100</span>
          <span>f/1.8</span>
          <span>50MM / KIT</span>
        </div>
      </div>
    </section>

    <!-- About & Academic Info -->
    <section id="gioi-thieu">
      <div class="section-header">
        <span class="section-tag mono">// 01. HỒ SƠ CÁ NHÂN</span>
        <h2 class="section-title">Thông tin cơ bản</h2>
      </div>
      <div class="info-grid">
        <div class="info-card">
          <div class="info-label">Họ và tên</div>
          <div class="info-value">Nguyễn Tuấn Thanh</div>
        </div>
        <div class="info-card">
          <div class="info-label">Lớp &amp; Trường</div>
          <div class="info-value">11T2 • THPT Chuyên Bến Tre</div>
        </div>
        <div class="info-card">
          <div class="info-label">Địa phương</div>
          <div class="info-value">Tỉnh Vĩnh Long</div>
        </div>
        <div class="info-card">
          <div class="info-label">Số điện thoại liên hệ</div>
          <div class="info-value mono"><a href="tel:0974093831">0974093831</a></div>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section id="ky-nang">
      <div class="section-header">
        <span class="section-tag mono">// 02. NĂNG LỰC &amp; ĐAM MÊ</span>
        <h2 class="section-title">Năng lực &amp; Đam mê nổi bật</h2>
      </div>
      <div class="skills-grid">
        <!-- STEM Card -->
        <div class="skill-panel stem">
          <div class="panel-title">
            <span>⚙️</span>
            <span>Kỹ năng STEM &amp; Kỹ thuật</span>
          </div>
          <p class="panel-desc">
            Vận dụng kiến thức Khoa học, Công nghệ, Kỹ thuật và Toán học để xây dựng ý tưởng và giải quyết vấn đề thực tế.
          </p>
          <ul class="skill-list">
            <li>
              <strong>Tư duy Logic &amp; Giải quyết vấn đề</strong>
              Phân tích bài toán, thử nghiệm giả thuyết và tối ưu quy trình làm việc.
            </li>
            <li>
              <strong>Điện tử &amp; Lập trình cơ bản</strong>
              Làm quen với mạch điện, cảm biến, vi điều khiển và tư duy lập trình.
            </li>
            <li>
              <strong>Thiết kế &amp; Thực nghiệm mô hình</strong>
              Lên bản vẽ ý tưởng, lắp ráp và kiểm thử các sản phẩm STEM học đường.
            </li>
          </ul>
        </div>

        <!-- Photography Card -->
        <div class="skill-panel photo">
          <div class="panel-title">
            <span>📸</span>
            <span>Kỹ năng Nhiếp ảnh</span>
          </div>
          <p class="panel-desc">
            Ghi lại khoảnh khắc đời sống, thiên nhiên và góc nhìn nghệ thuật thông qua ánh sáng, bố cục và hậu kỳ.
          </p>
          <ul class="skill-list">
            <li>
              <strong>Bố cục &amp; Ánh sáng</strong>
              Áp dụng tỷ lệ khung hình, đường dẫn và tận dụng khẩu độ lớn f/1.8 cùng ánh sáng tự nhiên.
            </li>
            <li>
              <strong>Chụp ảnh Đời sống &amp; Sự kiện</strong>
              Lưu giữ hình ảnh trường lớp, hoạt động tập thể và cảnh sắc quê hương.
            </li>
            <li>
              <strong>Hậu kỳ &amp; Chỉnh màu</strong>
              Cân chỉnh độ sáng, tương phản và màu sắc để bức ảnh hài hòa, có chiều sâu.
            </li>
          </ul>
        </div>

        <!-- Volleyball Setter Card -->
        <div class="skill-panel volley" id="ky-nang-chuyen-hai">
          <div class="panel-title">
            <span>🏐</span>
            <span>Kỹ năng Chuyền 2 Bóng chuyền</span>
          </div>
          <p class="panel-desc">
            Đảm nhận vai trò <strong>Chuyền 2 (setter)</strong> trong bóng chuyền — điều phối nhịp độ tấn công và kết nối đồng đội trên sân.
          </p>
          <ul class="skill-list">
            <li>
              <strong>Chuyền bóng chuẩn xác &amp; Ổn định nhịp</strong>
              Kiểm soát lực, độ cao và điểm rơi để tạo đà tấn công thuận lợi cho đồng đội.
            </li>
            <li>
              <strong>Đọc tình huống &amp; Điều phối lối chơi</strong>
              Quan sát hàng chắn đối phương, phân phối bóng linh hoạt và giữ nhịp đội hình.
            </li>
            <li>
              <strong>Phản xạ &amp; Giao tiếp đồng đội</strong>
              Di chuyển bọc lót nhanh nhẹn, phối hợp ăn ý và giữ tinh thần gắn kết toàn đội.
            </li>
          </ul>
        </div>

        <!-- Creative 3D & Coding Card -->
        <div class="skill-panel creative" id="nang-luc-sang-tao">
          <div class="panel-title">
            <span>🧊</span>
            <span>Thiết kế 3D &amp; Lập trình sáng tạo</span>
          </div>
          <p class="panel-desc">
            Kết hợp mô hình hóa 3D, script tự động hóa và giao diện web tương tác để biến ý tưởng trực quan thành sản phẩm số.
          </p>
          <ul class="skill-list">
            <li>
              <strong>Dựng hình &amp; Kịch bản 3D</strong>
              Tạo hình khối, không gian và ánh sáng cho các mô hình kiến trúc, phương tiện và sản phẩm mẫu.
            </li>
            <li>
              <strong>Tự động hóa &amp; Viết mã hỗ trợ</strong>
              Viết đoạn mã gọn nhẹ để sinh mô hình, kiểm thử mạch/thiết bị và tối ưu thao tác.
            </li>
            <li>
              <strong>Trình bày trực quan &amp; Kể chuyện</strong>
              Xây dựng trang web, slide và nội dung sinh động giúp ý tưởng dễ tiếp cận với mọi người.
            </li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Camera Gear Section -->
    <section id="thiet-bi">
      <div class="section-header">
        <span class="section-tag mono">// 03. THIẾT BỊ NHIẾP ẢNH</span>
        <h2 class="section-title">Bộ máy ảnh đang sử dụng</h2>
      </div>
      <div class="gear-grid">
        <div class="gear-card">
          <span class="gear-tag mono">FULL-FRAME DSLR</span>
          <h3 class="gear-title">Canon EOS 5D Mark III (5D3)</h3>
          <div class="gear-lens mono">Ống kính: Lens 50mm f/1.8 II</div>
          <p class="panel-desc">
            Thân máy Full-frame kết hợp tiêu cự 50mm khẩu độ f/1.8 II cho chất ảnh nổi khối, làm chủ ánh sáng tốt và xóa phông chân dung mượt mà.
          </p>
        </div>

        <div class="gear-card">
          <span class="gear-tag mono">COMPACT MIRRORLESS</span>
          <h3 class="gear-title">Canon EOS M200</h3>
          <div class="gear-lens mono">Ống kính: Lens Kit</div>
          <p class="panel-desc">
            Máy ảnh nhỏ gọn, cơ động kết hợp Lens Kit đa dụng, thuận tiện mang theo hằng ngày để ghi lại khoảnh khắc nhanh gọn, linh hoạt.
          </p>
        </div>
      </div>
    </section>

    <!-- Gallery Section -->
    <section id="bo-suu-tap">
      <div class="section-header">
        <span class="section-tag mono">// 04. GÓC LƯU TRỮ</span>
        <h2 class="section-title">Khoảnh khắc Nhiếp ảnh &amp; STEM</h2>
      </div>
      <div class="gallery-grid">
        <div class="photo-card">
          <img src="https://images.unsplash.com/photo-1516035069371-29a1b244cc32?auto=format&fit=crop&w=800&q=80" alt="Canon 5D3 và Lens 50mm f/1.8 II" />
          <div class="photo-overlay">
            <span class="photo-meta mono">CANON 5D3 • 50MM f/1.8 II</span>
            <div class="photo-caption">Chân dung &amp; chiều sâu trường ảnh</div>
          </div>
        </div>
        <div class="photo-card">
          <img src="https://images.unsplash.com/photo-1452587925148-ce544e77e70d?auto=format&fit=crop&w=800&q=80" alt="Canon M200 và Lens Kit" />
          <div class="photo-overlay">
            <span class="photo-meta mono">CANON M200 • LENS KIT</span>
            <div class="photo-caption">Ghi hình gọn nhẹ mọi hành trình</div>
          </div>
        </div>
        <div class="photo-card">
          <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?auto=format&fit=crop&w=800&q=80" alt="Mạch điện tử STEM" />
          <div class="photo-overlay">
            <span class="photo-meta mono">STEM LAB • HARDWARE</span>
            <div class="photo-caption">Khám phá mạch điện tử &amp; công nghệ</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Charity QR Section -->
    <section id="tu-thien">
      <div class="section-header">
        <span class="section-tag mono" style="color: var(--accent-charity);">// 05. ĐÓNG GÓP &amp; TỪ THIỆN</span>
        <h2 class="section-title">Mã chuyển khoản từ thiện</h2>
      </div>
      <div class="charity-grid">
        <div class="qr-frame">
          <img
            id="charityQrImg"
            src="images/qr-tu-thien.jpg"
            alt="Mã QR chuyển khoản từ thiện Agribank Nguyễn Tuấn Thanh"
          />
        </div>
        <div>
          <h3 style="font-size: 1.25rem; font-weight: 700; margin-bottom: 8px;">Quét mã VietQR qua ứng dụng Ngân hàng</h3>
          <p style="color: var(--text-secondary); font-size: 0.94rem;">
            Hỗ trợ chuyển khoản nhanh Agribank và liên ngân hàng NAPAS 24/7. Vui lòng kiểm tra đúng thông tin người nhận trước khi chuyển.
          </p>
          <ul class="bank-details mono">
            <li><strong>Chủ tài khoản:</strong> NGUYEN TUAN THANH</li>
            <li><strong>Số tài khoản:</strong> 7104205433117</li>
            <li><strong>Ngân hàng:</strong> Agribank — Chi nhánh H. Bình Đại - Bến Tre</li>
          </ul>
          <button type="button" class="btn btn-outline" id="copyBankBtn">🏦 Sao chép STK &amp; Ngân hàng</button>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="lien-he">
      <div class="contact-box">
        <span class="section-tag mono">// 06. KẾT NỐI</span>
        <h2 class="section-title">Cùng giao lưu về Nhiếp ảnh, STEM &amp; Bóng chuyền</h2>
        <p>
          Liên hệ trực tiếp qua số điện thoại <strong>0974093831</strong>, sao chép nhanh thông tin giới thiệu hoặc ghé thăm Facebook / GitHub để cùng trao đổi nhé!
        </p>
        <div class="contact-actions">
          <a href="tel:0974093831" class="btn btn-primary">📞 Gọi 0974093831</a>
          <button type="button" class="btn btn-outline" id="copyInfoBtn">📋 Sao chép thông tin &amp; SĐT</button>
          <a href="https://www.facebook.com/share/1LZqzdeCnJ/" target="_blank" rel="noopener noreferrer" class="btn btn-outline">📘 Facebook cá nhân</a>
          <a href="https://github.com/" target="_blank" rel="noopener noreferrer" class="btn btn-outline">💻 GitHub cá nhân</a>
        </div>
        <div class="copy-feedback mono" id="copyFeedback" role="status" aria-live="polite"></div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>© 2026 <strong>Nguyễn Tuấn Thanh</strong> — Lớp 11T2, Trường THPT Chuyên Bến Tre (Vĩnh Long) • SĐT: 0974093831.</p>
    </div>
  </footer>

  <script>
    // 1. Ảnh QR từ thiện: ưu tiên images/qr-tu-thien.jpg, nếu chưa có thì hiện ảnh VietQR Agribank
    const charityQrImg = document.getElementById('charityQrImg');
    const vietQrFallbackUrl = 'https://img.vietqr.io/image/VBA-7104205433117-compact2.png?accountName=NGUYEN%20TUAN%20THANH';
    let qrFallbackUsed = false;

    charityQrImg.addEventListener('error', () => {
      if (!qrFallbackUsed) {
        qrFallbackUsed = true;
        charityQrImg.src = vietQrFallbackUrl;
      }
    });

    // 2. Chuyển đổi chế độ Sáng / Tối
    const themeToggle = document.getElementById('themeToggle');
    const htmlEl = document.documentElement;

    themeToggle.addEventListener('click', () => {
      const isDark = htmlEl.getAttribute('data-theme') === 'dark';
      const nextTheme = isDark ? 'light' : 'dark';
      htmlEl.setAttribute('data-theme', nextTheme);
      themeToggle.textContent = nextTheme === 'dark' ? '☀️ Sáng' : '🌙 Tối';
    });

    // 3. Mở / đóng menu trên điện thoại
    const menuToggle = document.getElementById('menuToggle');
    const mobileMenu = document.getElementById('mobileMenu');

    function closeMobileMenu() {
      mobileMenu.classList.remove('open');
      menuToggle.setAttribute('aria-expanded', 'false');
      menuToggle.textContent = '☰';
    }

    menuToggle.addEventListener('click', () => {
      const isOpen = mobileMenu.classList.toggle('open');
      menuToggle.setAttribute('aria-expanded', String(isOpen));
      menuToggle.textContent = isOpen ? '✕' : '☰';
    });

    mobileMenu.querySelectorAll('a').forEach((link) => {
      link.addEventListener('click', closeMobileMenu);
    });

    window.addEventListener('resize', () => {
      if (window.innerWidth > 820) {
        closeMobileMenu();
      }
    });

    // 4. Hàm sao chép có dự phòng
    const feedback = document.getElementById('copyFeedback');

    function showFeedback(message) {
      feedback.textContent = message;
      clearTimeout(showFeedback.timer);
      showFeedback.timer = setTimeout(() => {
        feedback.textContent = '';
      }, 3000);
    }

    async function copyTextWithFallback(text, successMsg) {
      try {
        if (navigator.clipboard && window.isSecureContext) {
          await navigator.clipboard.writeText(text);
          showFeedback(successMsg);
          return;
        }
      } catch (err) {}

      const textarea = document.createElement('textarea');
      textarea.value = text;
      textarea.style.position = 'fixed';
      textarea.style.opacity = '0';
      document.body.appendChild(textarea);
      textarea.focus();
      textarea.select();
      try {
        document.execCommand('copy');
        showFeedback(successMsg);
      } catch (err) {
        showFeedback('Không thể tự động sao chép, bạn hãy copy thủ công nhé.');
      }
      document.body.removeChild(textarea);
    }

    const copyBankBtn = document.getElementById('copyBankBtn');
    if (copyBankBtn) {
      copyBankBtn.addEventListener('click', () => {
        copyTextWithFallback(
          'STK: 7104205433117 | Chủ TK: NGUYEN TUAN THANH | Ngân hàng: Agribank CN H. Bình Đại - Bến Tre',
          'Đã sao chép thông tin tài khoản từ thiện!'
        );
      });
    }

    const copyInfoBtn = document.getElementById('copyInfoBtn');
    if (copyInfoBtn) {
      copyInfoBtn.addEventListener('click', () => {
        copyTextWithFallback(
          'Nguyễn Tuấn Thanh — 11T2, THPT Chuyên Bến Tre (Vĩnh Long) | SĐT: 0974093831',
          'Đã sao chép thông tin liên hệ!'
        );
      });
    }
  </script>
</body>
</html>
