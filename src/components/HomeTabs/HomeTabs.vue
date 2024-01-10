<template>
  <div class="homeTabs"> 
    <Statistics/>
    <Featured/>
    <OptionBuildings/>
  </div>
</template>

<script>

import Statistics from './Statistics.vue'
import Featured from './Featured.vue'
import OptionBuildings from './OptionBuildings.vue'

export default {
    components: {
    Statistics,
    Featured,
    OptionBuildings
    }
}
</script>

<style>
    .homeTabs{
        display: flex;
        flex-direction: column;
        row-gap: 15px;
        width: 100% ;
    }
</style>