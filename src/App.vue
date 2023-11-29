<script>
import testata from './components/testata.vue'
import content from './components/content.vue'
import iconbar from './components/iconbar.vue'
import endsite from './components/endsite.vue'


export default{
  components: {
    testata,
    content, 
    iconbar,
    endsite
  }
}
</script>

<template>
    <testata/>
    <main>
      <content/>
      <iconbar/>
    </main>
    <endsite/>
</template>

<style scoped>

</style>
