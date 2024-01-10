<template>
  <div class="main-content">
    <HomeTabs/>
    <!--<SingleBuilding/>-->
    <!--<SingleRoom/>-->
    <!--<RoomStats/>-->
  </div>
</template>

<script>
import HomeTabs from './HomeTabs/HomeTabs.vue'
import SingleBuilding from './SingleBuilding.vue'
import SingleRoom from './SingleRoom.vue'
import RoomStats from './RoomStats.vue'

export default {
  components: {
    HomeTabs,
    SingleBuilding,
    SingleRoom,
    RoomStats
  }
}
</script>

<style>
  
</style>