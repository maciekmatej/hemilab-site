<template>
  <header>
    <div class="menu-wrapper">
      <div class="logo">
        <img src="~@/assets/hemilab-logo.png" alt="hemilab logo" />
      </div>
      <nav>
        <ul class="list">
          <li class="list-item"><button class="start-btn">start</button></li>
          <li class="list-item">
            <a @click="activeTab = 'aktualności'" href="#">aktualności</a>
          </li>
          <li class="list-item">
            <a @click="activeTab = 'o nas'" href="#">o nas</a>
          </li>
          <li class="list-item">
            <a @click="activeTab = 'oferta'" href="#">oferta</a>
          </li>
          <li class="list-item">
            <a @click="activeTab = 'kontakt'" href="#">kontakt</a>
          </li>
          <li class="list-item lang">
            <button @click="langBtnActve" class="lang-btn">
              <img src="~@/assets/earth-icon.png" />język
            </button>
            <div v-if="langBtn" class="lang-menu">
              <a href="#">Polski</a>
              <a href="#">Angielski</a>
            </div>
          </li>
        </ul>
      </nav>
    </div>
    <div class="navigation-bar">
      <span>home</span>
      <span> > {{ activeTab }}</span>
    </div>
  </header>
  <main>
    <div class="flex-wrapper">
      <h1>{{ activeTab }}</h1>
      <section class="flex">
        <div class="img-wrapper">
          <img src="~@/assets/img1.png" alt="product image" />
        </div>
        <article class="big-article">
          <h2>CEE Retail Summit</h2>
          <p>
            CEE Retail Summit 13 - 14 marca 2018<br />
            Zapraszamy na prezentację naszego<br />
            innowacyjnego urządzenia<br />
            dwufunkcyjnego Spinakerr DF.
          </p>
          <button>Czytaj więcej ></button>
        </article>
      </section>
    </div>
    <div class="grid-wrapper">
      <section class="grid">
        <article class="small-article">
          <img src="~@/assets/img2.png" alt="product image" />
          <h3>Lorem Ipsum</h3>
          <p>
            Lorem ipsum dolor sit amet<br />
            enim. Etiam ullamcorper.<br />
            Suspendisse a pellentesque<br />
            dui, non felis.
          </p>
          <button>Czytaj więcej ></button>
        </article>
        <article class="small-article">
          <img src="~@/assets/img2.png" alt="product image" />
          <h3>Lorem Ipsum</h3>
          <p>
            Lorem ipsum dolor sit amet<br />
            enim. Etiam ullamcorper.<br />
            Suspendisse a pellentesque<br />
            dui, non felis.
          </p>
          <button>Czytaj więcej ></button>
        </article>
        <article class="small-article">
          <img src="~@/assets/img2.png" alt="product image" />
          <h3>Lorem Ipsum</h3>
          <p>
            Lorem ipsum dolor sit amet<br />
            enim. Etiam ullamcorper.<br />
            Suspendisse a pellentesque<br />
            dui, non felis.
          </p>
          <button>Czytaj więcej ></button>
        </article>
        <article class="small-article">
          <img src="~@/assets/img2.png" alt="product image" />
          <h3>Lorem Ipsum</h3>
          <p>
            Lorem ipsum dolor sit amet<br />
            enim. Etiam ullamcorper.<br />
            Suspendisse a pellentesque<br />
            dui, non felis.
          </p>
          <button>Czytaj więcej ></button>
        </article>
      </section>
      <div class="pagination">
        <button class="page-number">1</button>
        <button class="page-number">2</button>
        <button class="page-number">3</button>
        <button class="page-number">4</button>
        <button class="page-number">5</button>
        <button class="page-number">6</button>
        <button class="page-number">7</button>
        <button class="page-number">8</button>
        <button class="page-number">9</button>
      </div>
    </div>
  </main>
  <footer>
    <section class="info">
      <h2 class="info-text">info</h2>
      <div class="flex-container">
        <ul class="info-list">
          <li><b>Oferta</b></li>
          <li>Systemy samoobsługowe</li>
          <li>Cyfrowa Mapa Sklepu</li>
          <li>eCommerce picking cart</li>
          <li>Sprzedaż automatyczna</li>
        </ul>
        <ul class="info-list">
          <li><b>Firma</b></li>
          <li>O nas</li>
          <li>Partnerzy</li>
          <li>Kontakt</li>
          <li>Realizacje</li>
        </ul>
        <div class="ctn">
          <div><b>Aktualności</b></div>
          <div class="media-wrapper">
            <img src="~@/assets/youtube-logo.png" alt="youtube" />
            <img src="~@/assets/linkedin-logo.png" alt="linkedin" />
          </div>
        </div>
      </div>
      <div class="container">
        <img src="~@/assets/hemilab-logo.png" alt="hemilab logo" />
        <p>
          Copyright © 2017 HemiLab sp. z o.o. sp. k.<br />
          Wszelkie prawa zastrzeżone.
        </p>
      </div>
    </section>
    <section class="partners">
      <div class="partners-flex">
      <h3 class="partners-header">partnerzy</h3>
      <div class="media-wrapper">
        <img src="~@/assets/danler-logo.png" alt="danler" />
        <img src="~@/assets/mago-logo.png" alt="mago" />
      </div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      activeTab: 'aktualności',
      currentPage: 1,
      langBtn: false,
    };
  },
  methods: {
    langBtnActve() {
      this.langBtn = !this.langBtn;
    },
  },
};
</script>

<style>

</style>
