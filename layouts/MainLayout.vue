<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-primary text-secondary" height-hint="98">
      <q-toolbar>
        <q-toolbar-title class="text-center my-font title">
          <router-link style="text-decoration: none; color: inherit" to="/home">
            <strong> Antonio y Paulina </strong>
          </router-link>
        </q-toolbar-title>
      </q-toolbar>

      <q-tabs align="center" class="my-second-font text-secondary">
        <q-route-tab to="/home" label="Inicio" />
        <q-route-tab to="/page2" label="Agenda de celebraciones" />
        <q-route-tab to="/page3" label="Alojamientos" />
        <q-route-tab to="/page3" label="Turismo" />
        <q-route-tab to="/food" label="Donde comer" />
        <q-route-tab to="/page3" label="R.S.V." />
        <q-route-tab to="/page3" label="FAQ" />
      </q-tabs>
    </q-header>

    <q-page-container class="bg-default">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup></script>
<style lang="sass" scoped>
.title
  font-size: 6em

@media only screen and (max-width: $breakpoint-sm-max)
  .title
    font-size: 4em
@media only screen and (max-width: $breakpoint-xs-max)
  .title
    font-size: 3em
</style>
