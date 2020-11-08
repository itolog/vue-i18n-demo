<template>
<div id="nav">
  <router-link :to="{ name: 'Home', params: { lang: this.$i18n.locale }}">
    {{ $t('menu.home') }}
  </router-link>

  <br>
  
  <router-link :to="{ name: 'About', params: { lang: this.$i18n.locale }}">
    {{ $t('menu.about') }}
  </router-link>
</div>
</template>