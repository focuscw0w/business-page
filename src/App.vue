<template>
  <Navigation @scrollToSection="scrollToSection($event)" />
  <div class="introduction-screen w-screen h-screen" ref="home">
    <div class="relative flex h-screen items-end container-lg container-style">
      <div class="mb-8">
        <h1 class="inline-block md:text-7xl text-6xl font-bold highlighted-color mb-6">
          <span class="bg-black px-4 pt-3">Silná technika</span>
        </h1>
        <h1 class="md:text-7xl text-6xl leading-snug md:leading-tight font-bold highlighted-color mb-3">
          <span class="bg-black px-4 pt-3">Neohraničené možnosti</span>
        </h1>
      </div>
    </div>
  </div>
  <!-- new section --->
  <section
    class="container-lg container-style justify-between items-center flex flex-col md:flex-row gap-5 py-24"
  >
    <div>
      <img src="./assets/images/Ornament.svg" alt="ornament" />
      <h3 class="heading-style">Kontaktuje nás</h3>
      <p>Odpovieme Vám v najrýchlejšom možnom čase</p>
    </div>
    <div class="border-solid border-black border-2 py-2 px-12">
      <span class="text-sm heading-color">dusanmajchrak78@gmail.com</span>
    </div>
  </section>
  <!-- new section -->
  <section class="py-24 grey-background" ref="whyUs">
    <div class="container-lg container-style">
      <img src="./assets/images/Ornament.svg" alt="ornament" />
      <h3 class="heading-style">Prečo my?</h3>
      <p>
        Sal din hug og lat den ri og renna med blinde augo vil du vegen finna
      </p>
      <div class="flex flex-col items-center md:flex-row gap-8 mt-20">
        <div class="box-style md:w-1/3">
          <img
            class="mb-8"
            src="./assets/images/speed_FILL0_wght400_GRAD0_opsz48.svg"
            alt="speed icon"
          />
          <h4 class="mb-2 text-3xl">Rýchlosť dodania</h4>
          <p class="text-lg">
            Naša firma poskytuje rýchle a efektívne služby, čím vám ušetrí čas a
            zabezpečí promptné dokončenie projektov.
          </p>
        </div>
        <div class="box-style md:w-1/3">
          <img
            class="mb-8"
            src="./assets/images/verified_FILL0_wght400_GRAD0_opsz48.svg"
            alt="verified icon"
          />
          <h4 class="mb-2 text-3xl">Spoľahlivosť</h4>
          <p class="text-lg">
            Sme spoľahlivým partnerom, ktorý sa môžete spoľahnúť na kvalitu a
            bezproblémové vykonávanie práce.
          </p>
        </div>
        <div class="box-style md:w-1/3">
          <img
            class="mb-8"
            src="./assets/images/thumb_up_FILL0_wght400_GRAD0_opsz48.svg"
            alt="thumb up icon"
          />
          <h4 class="mb-2 text-3xl">Precíznosť</h4>
          <p class="text-lg">
            Sme spoľahlivým partnerom, ktorý sa môžete spoľahnúť na kvalitu a
            bezproblémové vykonávanie práce.
          </p>
        </div>
      </div>
    </div>
  </section>
  <!-- new section -->
  <section class="container-lg container-style py-24" ref="ourMachines">
    <img src="./assets/images/Ornament.svg" alt="ornament" />
    <h3 class="heading-style">Naše stroje</h3>
    <p>Sal din hug og lat den ri og renna med blinde augo vil du vegen finna</p>
  </section>
  <!-- new section -->
  <section class="mb-8 md:mb-0">
    <div class="flex md:flex-row flex-col gap-5">
      <div
        class="md:w-1/4 w-100 h border-solid border-2 border-white truck-preview-1"
      ></div>
      <div
        class="md:w-1/4 border-solid border-2 border-white truck-preview-2"
      ></div>
      <div
        class="md:w-1/4 border-solid border-2 border-white truck-preview-3"
      ></div>
      <div
        class="md:w-1/4 border-solid border-2 border-white truck-preview-4"
      ></div>
    </div>
  </section>
  <!-- footer -->
  <footer class="footer-background py-24" ref="contact">
    <div
      class="container-lg container-style flex flex-col md:flex-row gap-8 justify-between"
    >
      <img class="h-20 md:h-auto" src="./assets/images/Logo_svg_majchrak.svg" alt="logo majchrak" />
      <div class="flex flex-col md:flex-row items-start ml-8 md:ml-0">
        <div class="mb-5 md:mb-0">
          <p class="text-white mb-4 font-bold text-2xl">Adresa</p>
          <ul>
            <li class="text-color-emphasized text-lg">Zakamenné 925</li>
            <li class="text-color-emphasized text-lg">Zakamenné</li>
            <li class="text-color-emphasized text-lg">02956</li>
          </ul>
        </div>
        <div class="md:ml-24 mb-5 md:mb-0">
          <p class="text-white mb-4 font-bold text-2xl">Údaje o spoločnosti</p>
          <ul>
            <li class="text-color-emphasized text-lg">IČO: 35379448</li>
            <li class="text-color-emphasized text-lg">DIČ: 1020083207</li>
          </ul>
        </div>
        <div class="md:ml-24 mb-5 md:mb-0">
          <p class="text-white mb-4 font-bold text-2xl">Kontakt</p>
          <ul>
            <li class="text-color-emphasized text-lg">
              Email: dusanmajchrak78@gmail.com
            </li>
            <li class="text-color-emphasized text-lg">Telefon: 0910 123 456</li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
  <!-- copyright -->
  <div class="bg-black py-5">
    <p class="text-base text-center text-color-emphasized">
      © 2016-2022 Dušan Majchrák. Všetky práva vyhradené. Vytvorené Jakubom
      Rončákom
    </p>
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue";
export default {
  name: "Home",
  components: { Navigation },
  methods: {
    scrollToSection(sectionName) {
      this.$refs[sectionName].scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>
