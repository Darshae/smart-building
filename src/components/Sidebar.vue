<template>
  <div class="sideBar">
    <i class='bx bx-loader-circle' ></i>
    <hr>
    <ul>
      <li :class="{ 'active': selectedOption === 'overview' }" @click="chosenClick('overview')"><i class='bx bx-street-view'></i>Overview</li>
      <li :class="{ 'active': selectedOption === 'buildings' }" @click="chosenClick('buildings')"><i class='bx bx-building-house'></i>Buildings</li>
      <li :class="{ 'active': selectedOption === 'heatingSchedule' }" @click="chosenClick('heatingSchedule')"><i class='bx bxs-calendar'></i>Heating Schedule</li>
    </ul>
  </div>
</template>

<script>

import { ref} from 'vue';

export default {
  setup() {
    const selectedOption = ref('overview');

    const chosenClick = (option) => {
      selectedOption.value = option;
    };

    return { selectedOption, chosenClick };
  }
}
</script>

<style>
  .sideBar{
    border: 1px white solid;
    border-radius: 5px;
    width: 200px;
    height: 90svh;
    padding: 25px;
  }

  .sideBar i{
    margin-right: 5px;
    color: hsl(0, 0%, 70%);
    font-size: 1.2em;
  }

  .sideBar ul{
    list-style: none;
    padding: 5px 0px;
    margin: 0;
  }

  .sideBar li{
    text-align: left;
    margin: 10px 0px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1.1em;
    padding: 5px;
  }

  .sideBar li:hover{
    cursor: pointer;

  }

  li.active{
    background:hsl(191, 100%, 46%);
    border-radius: 5px;
    color: white;
  }

  li.active i {
    color: white;  /* Add the desired color for the 'i' element here */
  }

</style>