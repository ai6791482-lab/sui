<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>武舟會 日本武道会</title>
<style>
  /* 全体設定 */
  body, html {
    margin: 0; padding: 0;
    font-family: "Noto Serif JP", serif;
    background: #f9f9f9;
    color: #333;
    scroll-behavior: smooth;
  }

  /* ヘッダー */
  header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #111;
    color: #fff;
    padding: 1rem 2rem;
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  header .logo {
    width: 80px;
  }

  header h1 {
    margin: 0 2rem;
    font-size: 1.8rem;
  }

  nav {
    display: flex;
  }

  nav a {
    color: #fff;
    margin-left: 1.5rem;
    text-decoration: none;
    font-weight: bold;
    position: relative;
    transition: color 0.3s;
  }

  nav a::after {
    content: "";
    display: block;
    width: 0;
    height: 2px;
    background: #ffcccb;
    transition: width 0.3s;
    margin: 0 auto;
  }

  nav a:hover::after {
    width: 100%;
  }

  nav a:hover {
    color: #ffcccb;
  }

  /* セクション */
  .section {
    max-width: 1000px;
    margin: 4rem auto;
    padding: 2rem 3rem;
    background: #fff;
    border-left: 6px solid #800000;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    opacity: 0;
    transform: translateY(40px);
    transition: all 1s ease;
  }

  .section.show {
    opacity: 1;
    transform: translateY(0);
  }

  .section h2 {
    color: #800000;
    margin-bottom: 1rem;
  }

  .section p {
    line-height: 1.8;
  }

  /* フッター */
  footer {
    background: #111;
    color: #fff;
    text-align: center;
    padding: 2rem 1rem;
  }
</style>
</head>
<body>

<header>
  <img src="https://daikitakahashi811-cbsml.wordpress.com/wp-content/uploads/2025/07/img_0013.png" alt="道場ロゴ" class="logo">
  <h1>武舟會 日本武道会</h1>
  <nav>
    <a href="#home">ホーム</a>
    <a href="#philosophy">理念</a>
    <a href="#history">歴史</a>
    <a href="#activities">活動</a>
    <a href="#members">会員</a>
    <a href="#contact">お問い合わせ</a>
  </nav>
</header>

<section class="section" id="home">
  <h2>ホーム</h2>
  <p>武道とは単なる技術やスポーツではなく、尊敬、規律、調和を重んじる「心の道」です。</p>
</section>

<section class="section" id="philosophy">
  <h2>理念</h2>
  <p>• 武道の精神と技術の継承<br>
     • 国際交流<br>
     • 青少年の人格形成<br>
     • 世界平和への貢献</p>
</section>

<section class="section" id="history">
  <h2>歴史</h2>
  <p>剣道、柔道、空手道、合気道、弓道など、武道は何世代にも渡って継承されてきました。</p>
</section>

<section class="section" id="activities">
  <h2>活動</h2>
  <p>国際大会、交流イベント、指導者育成、加盟団体との協力を通じて、武道の発展と世界理解を推進しています。</p>
</section>

<section class="section" id="members">
  <h2>会員団体</h2>
  <p>国内外の武道団体が共通の理念のもとに参加し、協力しています。</p>
</section>

<section class="section" id="contact">
  <h2>お問い合わせ</h2>
  <p>入会・取材・問い合わせは以下まで:<br>📧 info@japanbudo.or.jp</p>
</section>

<footer>
  <p>&copy; 2025 武舟會 日本武道会 - All Rights Reserved</p>
</footer>

<script>
  // スクロールでフェードイン
  const sections = document.querySelectorAll('.section');
  window.addEventListener('scroll', () => {
    sections.forEach(sec => {
      const rect = sec.getBoundingClientRect();
      if(rect.top < window.innerHeight * 0.85){
        sec.classList.add('show');
      }
    });
  });
</script>

</body>
</html>
