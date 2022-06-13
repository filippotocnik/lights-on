<script setup lang="ts">
// zelena #99FF00
// temno siva iz vizitke #191919
// crna #000000
</script>

<template>
  <div class="main">
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
      <div></div>
    </div>
  </div>
</template>

<style>
.main {
  display: flex;
  justify-content: center;
  align-items: center;
}

.content-info > * {
  margin-bottom: 20px;
}

.logo {
  margin-bottom: 40px;
}

.logo img {
  width: 200px;
}
</style>
