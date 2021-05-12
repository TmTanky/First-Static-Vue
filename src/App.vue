<template>
  <the-header> </the-header>
    <div id="app">

      <introduction></introduction>
      <introduction-2></introduction-2>
      <contact></contact>

    </div>
  <the-footer> </the-footer>
</template>

<script>
import TheHeader from './components/header/TheHeader.vue'
import TheFooter from './components/footer/TheFooter.vue'
import Introduction from './components/introduction/Introduction.vue'
import Introduction2 from './components/introduction/Introduction2.vue'
import Contact from './components/contacts/Contacts.vue'

export default {
  components: { TheHeader, TheFooter, Introduction, Introduction2, Contact }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  min-height: 100vh;
}

</style>
