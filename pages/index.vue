<template>
  <div class="wrap">
    <section class="card introduction">
      <div class="introduction_name">
        <h1 class="font_ja">山下 浩一郎</h1>
        <p class="font">Kouichiro Yamashita</p>
      </div>
      <ul class="introduction_links font">
        <li>
          <TwitterLogo class="snsLogo" />
          <a href="https://twitter.com/nnjyami" target="_blank">
            nnjyami
          </a>
        </li>
        <li>
          <InstagramLogo class="snsLogo" />
          <a href="https://instagram.com/nnjyami" target="_blank">
            nnjyami
          </a>
        </li>
        <li>
          Blog:
          <a href="https://kyotokoto.jp" target="_blank">
            kyotokoto.jp
          </a>
        </li>
        <li>
          Mail:
          <a href="mailto:y@179.jp" target="_blank">
            y@179.jp
          </a>
        </li>
      </ul>
    </section>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/IMG_2487.jpg" />
        <figcaption>日常生活の中で web を使うと、<br />もっと楽しくなることを探しています。</figcaption>
      </figure>
    </div>
    <section class="card role">
      <h2 class="font_ja">好きなこと</h2>
      <ul>
        <li>デザインエンジニア
          <ul>
            <li>Interface・UI</li>
            <li>エンジニアリング（JS・PHP）</li>
          </ul>
        </li>
        <li>日々のなんでもない写真を撮るのが好き</li>
        <li>自家焙煎コーヒー</li>
        <li>猫飼ってます <a href="https://twitter.com/poncho_neko">@poncho_neko</a></li>
        <li>京都に住んでます</li>
        <li>自然の中で遊ぶのが好き</li>
      </ul>
    </section>
    <section class="card role">
      <h2 class="font">Background</h2>
      <ul>
        <li>15年前〜: Webデザイナー（デザイン・コーディング）</li>
        <li>5年前〜: オウンドメディア立ち上げ・CMS開発（PHP）</li>
        <li>2年前〜: Webアプリケーション開発（Sass・Vue）</li>
        <li>1年前〜: プロダクトマネージャー</li>
      </ul>
    </section>
    <section class="card role">
      <h3 class="font_ja">悩み</h3>
      <ul>
        <li>
          社内の数多いステークホルダーから合意を取ること
          <ul>
            <li>何人もいて、多忙</li>
            <li>エンジニア的な気質で、どうにか効率化できないかと思ってしまう</li>
            <li>無関心だが移譲はされない</li>
            <li>意思決定フローが長い...</li>
          </ul>
        </li>
        <li>ユーザー価値の視覚化 → 合意</li>
        <li>ビルドトラップに陥りがち</li>
        <li>会社文化的に非プロダクト企業</li>
        <li>
          セルフブランディング非統一問題<br />(nnjyami, 179, undermountain)
        </li>
        <li>ZEKU か LOLO か</li>
      </ul>
    </section>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1009282.JPG" />
      </figure>
    </div>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1009771.JPG" />
      </figure>
    </div>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1000053.JPG" />
      </figure>
    </div>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1000172.JPG" />
      </figure>
    </div>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1004277.JPG" />
      </figure>
    </div>
    <div class="card">
      <figure class="card_img">
        <img src="@/assets/img/L1008797.JPG" />
      </figure>
    </div>
  </div>
</template>

<script>
import TwitterLogo from '../components/TwitterLogo.vue';

export default {
  name: "IndexPage",
  components: { TwitterLogo }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  background-color: rgb(250, 250, 243);
  color: rgb(67, 63, 63);
  font-size: 24px;
  font-family: "Sawarabi Mincho", serif;
}

ul {
  list-style-position: inside;
}

ul li {
  margin-bottom: 0.7rem;
}

ul ul {
  margin: 0.7rem 0 1.4rem 2rem;
}

h2,
h3 {
  margin-bottom: 1rem;
}

figcaption {
  font-size: 1rem;
  color: rgba(67, 63, 63, .6);
  text-align: right;
}

a {
  color: rgb(40, 133, 219);
  text-decoration: none;
}

.font {
  font-family: 'Assistant', sans-serif;
}

.font_ja {
  font-family: "Sawarabi Mincho", serif;
}

.card {
  max-width: 900px;
  margin: 0 auto 1rem;
  padding: 8rem;
}

.card img {
  box-shadow: 0 0 14px rgba(0, 0, 0, .3);
  width: 100%;
}

.card_img img {
  border-radius: 0.5rem;
}

.introduction {}

.introduction_name {
  margin-bottom: 2rem;
  padding-top: 2rem;
}

.introduction_name h1 {
  font-feature-settings: "palt";
  letter-spacing: 0.2em;
}

.introduction_name p {
  font-size: 1.2rem;
  letter-spacing: 0.15em;
}

.introduction_links {
  font-size: 0.95rem;
  list-style: none;
}

.introduction_links li {
  align-items: center;
  display: flex;
  font-feature-settings: "palt";
  letter-spacing: 0.1rem;
}

.snsLogo {
  display: inline-block;
  width: 1rem;
  height: 16px;
  margin-right: 0.4rem;
}

@media (max-width: 767px) {
  body {
    font-size: 18px;
  }

  ul ul {
    margin: 0.7rem 0 1.4rem 1.4rem;
  }

  .card {
    margin: 0 auto 3.5rem;
    padding: 1rem;
  }

  .introduction {
    padding-top: 9rem;
  }

  .introduction_name h1 {
    font-size: 2.1rem;
  }
}
</style>