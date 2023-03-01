<template>
  <div class="content">
    <div>
      <h2 class="text-center my-font my-text">Save the date!</h2>
      <p class="text-center text-justify my-second-font my-text">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
      </p>
    </div>

    <div class="row justify-between">
      <q-card class="my-card col-md-5 col-sm-12 col-xs-12">
        <img src="../assets/img/photo_2023-02-27_21-37-31.jpg" />
        <q-card-section>
          <div class="text-h6">Invierno en Madrid</div>
          <div class="text-subtitle2">Parque del retiro</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          {{ lorem }}
        </q-card-section>
      </q-card>
      <!-- <div class="col-2"></div> -->
      <q-card class="my-card col-md-5 col-sm-12 col-xs-12">
        <img class="foto2" src="../assets/img/photo_2023-02-27_21-37-33.jpg" />
        <q-card-section>
          <div class="text-h6">Invierno en Sevilla</div>
          <div class="text-subtitle2">Plaza de España</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          {{ lorem }}
        </q-card-section>
      </q-card>
    </div>
    <div class="row my-card">
      <q-card class="col-lg-6 col-sm-12 col-xs-12">
        <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3062.5583120107744!2d-4.0482176845455005!3d39.86173029712945!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xd6a0b19ac3f21df%3A0xf0e9eb90cd922f24!2sCigarral%20del%20%C3%81ngel!5e0!3m2!1ses!2ses!4v1677695471817!5m2!1ses!2ses"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
        <q-card-section>
          <div class="text-h6">Lugar del encuentro</div>
          <div class="text-subtitle2">El Cigarral del Ángel</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          {{ lorem }}
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>

<script setup></script>

<style lang="sass" scoped>
.content
  width: 80%
  margin: auto

div
  color: #56473c

.my-card
  margin-top: 2em

.map
  width: 100%
  padding: 15px
  height: 30em

img
  max-height: 22em
  padding: 15px
  object-fit: cover
  object-position: 0 23%

p
  font-size: 1.2em
  letter-spacing: 0.1rem

@media only screen and (max-width: $breakpoint-sm-max)
  .content
    width: 90%
  .map
    width: 100%
    padding: 15px
    height: 300px

  p
    font-size: .8em
    letter-spacing: 0.1rem

@media only screen and (max-width: $breakpoint-xs-max)
  .title
    font-size: 3em
</style>
