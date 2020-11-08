<template>
  <div class="hello">
    <LocaleSwitcher /> 
    <h1>{{ $t('main.welcome', {company: 'Lokalise'}) }}</h1>
    <h2>{{ $t('main.new_message', {count: 10}) }}</h2>
     <p>{{ $d(new Date(), 'short') }}</p>
      <p>{{ $n(100, 'currency') }}</p>
  </div>
</template>

<script>
import LocaleSwitcher from './LocaleSwitcher';

export default {
  name: 'HelloWorld',
  components: {
LocaleSwitcher
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
