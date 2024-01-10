<template>
  <div class="home">
    <div class="sideBarHome">
      <SideBar/>
    </div>
    <div class="content">
      <div>
        <Searchbar/>
      </div>
      <div class="mainContent">
        <MainContent/>
      </div>
    </div>
    
  </div>
</template>

<script>
import MainContent from '../components/MainContent.vue'
import Searchbar from '../components/Searchbar.vue'
import SideBar from '../components/SideBar.vue'

export default {
  name: 'HomeView',
  components: {
    SideBar,
    Searchbar,
    MainContent
  }
}
</script>

<style>
  body{
    background-color: hsl(0, 0%, 95%);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .home{
    display: flex;
    align-content: center;
    justify-content: center;
    background: hsl(260, 23%, 97%);
    margin: 5px;
  }

  .sideBarHome{
    background: white;
    border-radius: 5px;
    
  }

  .content{
    flex-grow: 1;
    margin: 20px 10px 10px 25px;
  }

  .mainContent{
    margin-top: 15px;
  }
</style>