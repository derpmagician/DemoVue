<template>
  <div class="about">
    <h1>Acerca de</h1>
    <Cabecera/>
  </div>
</template>

<script>
// @ is an alias to /src
import Cabecera from '@/components/resources/Cabecera.vue'

export default {
  name: 'about',
  components: {
    Cabecera
  }
}
</script>
