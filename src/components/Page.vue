<script setup lang="ts">
// zelena #99FF00
// temno siva iz vizitke #191919
// crna #000000

const logos = [
  {
    imgPath: '/img/logos/vertigo-bird.jpg',
    link: 'https://vertigo-bird.com',
  },
  {
    imgPath: '/img/logos/intra-lighting.png',
    link: 'https://www.intra-lighting.com',
  },
  {
    imgPath: '/img/logos/nemo-lighting.png',
    link: 'https://www.nemolighting.com',
  },
  {
    imgPath: '/img/logos/luceplan.png',
    link: 'https://www.luceplan.com',
  },
  {
    imgPath: '/img/logos/olev.png',
    link: 'https://www.olevlight.com/en/',
  },
  {
    imgPath: '/img/logos/rotaliana.jpg',
    link: 'https://www.rotaliana.it/en/',
  },
  {
    imgPath: '/img/logos/acb.png',
    link: 'https://www.acbiluminacion.com/en/',
  },
]
</script>

<template>
  <div class="main">
    <div class="top">
      <div class="content">
        <div class="content-info">
          <div class="logo">
            <img src="/img/lightson-logo.jpg" />
          </div>
          <div>Internetna stran je v izdelavi.</div>
          <div>
            Našli nas boste lahko na:
            <br />
            Jelenčeva ulica 1, 4000 Kranj vhod B3, IBI center
          </div>
          <div>
            Zaenkrat se nahajamo na:
            <br />
            Šuceva ulica 25, 4000 Kranj, Rona poslovni center
          </div>
          <div>
            Kontakt
            <br />
            <a href="mailto:kristof@lightson.si">kristof@lightson.si</a>
            <br />
            040837750
          </div>
        </div>
      </div>
    </div>
    <div class="bottom">
      <div class="logos">
        <div v-for="logo in logos" class="logo">
          <a :href="logo.link">
            <img :src="logo.imgPath" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 100vh;
}

.top {
  flex: 3;
  display: flex;
  justify-content: center;
  align-items: center;
}

.bottom {
  flex: 1;
  width: 100%
}

.content-info > * {
  margin-bottom: 20px;
}

.logo {
  margin-bottom: 40px;
}

.logo img {
  width: 260px;
}

.logos {
  display: flex;
  flex-wrap: wrap;
}

.logos .logo {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.logos .logo a img {
  max-width: 60px;
}
</style>
