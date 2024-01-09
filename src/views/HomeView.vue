<template>
  <div class="home">
    <p>Hello</p>
    <Sidebar/>
  </div>
</template>

<script>
import Sidebar from '../components/Sidebar.vue'


export default {
  name: 'HomeView',
  components: {
    Sidebar
  }
}
</script>
