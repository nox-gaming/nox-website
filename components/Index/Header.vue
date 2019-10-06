<template>
  <!-- Photo by Florian Olivo on Unsplash -->
  <section class="video-container bg-tex">
    <div class="mt-20">
      <img src="/img/logo.png" alt="logo" />
      <h1 class="title">Nox-Gaming</h1>
      <h2 class="subtitle">Communauté Francophone Multigaming</h2>
      <h3>Jouez, partagez, vivez avec des joueurs/joueuses avec les mêmes passions.</h3>
      <div class="links mt-10">
        <a
          href="https://discord.gg/wvPYPk3"
          class="bg-orange-500 hover:bg-orange-400 text-white font-bold py-2 px-4 border-b-4 border-orange-700 hover:border-orange-500 rounded"
        >Rejoignez-nous</a>
        <a
          class="bg-orange-500 hover:bg-orange-400 text-white font-bold py-2 px-4 border-b-4 border-orange-700 hover:border-orange-500 rounded"
          href="/chart.pdf"
        >Charte de communauté</a>
      </div>
    </div>

    <figure>
      <video
        autoplay="true"
        loop="true"
        muted="true"
        poster="https://d3hmvhl7ru3t12.cloudfront.net/img/pages/home/header-video-poster-4d6f8aee9fd809779b1c36242f81c4c3d5afe3ef77a3d6bc3cd6248aab1980f89e80b41c14c56e5d5e4d06098f874b74d88a1932adf6e6f84da56dbcd8c10e72.jpg"
        data-js="header-video"
      >
        <source
          src="https://d3hmvhl7ru3t12.cloudfront.net/video/pages/home/header-20316a38f7cfb65480e84592386095445e3ed800accf65f4d638a11b89ce9ce7d95c0062f9ab760b36963383893bed79f199013acc3b549c8bf320eb696be33c.webm"
          type="video/webm"
        />
        <source
          src="https://d3hmvhl7ru3t12.cloudfront.net/video/pages/home/header-82b9abce067992beedde6d103b6241d616a7ee97cc0d4f3126277098c2e4b09004325f25c6a245656096bd333c880b0032e2cbdbed9d2514220e20718482e95b.mp4"
          type="video/mp4"
        />
      </video>
    </figure>
  </section>
</template>

<script>
name: 'Header'
</script>

<style>
.bg-orange-400 {
  background-color: theme('colors.accentDarker');
}
.bg-orange-500 {
  background-color: theme('colors.accent');
}
.border-orange-700 {
  background-color: theme('colors.accent');
}
.border-orange-500:hover {
  background-color: blue;
}

section {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  text-align: center;
  color: white;
  overflow-y: hidden;
}
figure {
  position: absolute;
  top: 0;
  z-index: -999;
  background: linear-gradient(
    90deg,
    rgba(0, 0, 0, 0.8) 100%,
    transparent 50.1%
  );
}
video {
  mix-blend-mode: overlay;
}
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'bigNoodle', 'Quicksand', 'Source Sans Pro', -apple-system,
    BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  letter-spacing: 1px;
}
@font-face {
  font-family: bigNoodle;
  src: url('/fonts/BIG_NOODLE_TITLING.TTF');
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.bg-tex {
  background-blend-mode: darken;
  /* background-color: #040109; */
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='8' height='8' viewBox='0 0 8 8'%3E%3Cg fill='%23ed8936' fill-opacity='0.07'%3E%3Cpath fill-rule='evenodd' d='M0 0h4v4H0V0zm4 4h4v4H4V4z'/%3E%3C/g%3E%3C/svg%3E");
}
</style>