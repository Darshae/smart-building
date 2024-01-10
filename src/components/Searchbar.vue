<template>
  <div class="searchBar">
    <div class="search">
        <i class='bx bx-search' ></i>
        <input type="text" placeholder="Search (Ctrl+/)">
    </div>
    <div class="misc">
        <div class="hold">
            <img src="../assets/Flags/us.png" alt="">
        </div>
        <div class="hold">
            <i class='bx bx-moon' ></i>
        </div>
        <div class="hold">
            <i class='bx bx-customize'></i>
        </div>
        <div class="hold">
            <i class='bx bx-bell' ></i>
        </div>
        <div class="hold">
            <img src="../assets/avatar-1.png" alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .searchBar{
        background: white;
        border-radius: 5px;
        height: 40px;
        padding: 5px 15px;
        display: flex;
        align-items: center;
        justify-content: space-between;    
    }

    .search{
        display: flex;
        align-items: center;
        height: 100%;
        width: 100%;
        flex-grow: 1;
    }

    .search i{
        font-size: 1.5em;
        margin-right: 5px;
    }

    .search input{
        border: none;
        height: 80%;
        font-size: 1em;
        width: 80%;
    }

    .search input:focus{
        outline: none;
        border-bottom: 2px solid black;
    }

    .misc{
        height: 100%;
        display: flex;
        align-items: center;
    }

    .hold{
        width: 25px;
        height: 25px;
        overflow: hidden;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 8px;
    }

    .hold:last-child{
        width: 30px;
        height: 30px;
    }

    .hold i{
        font-size: 1.5em;
    }

    img{
        object-fit: cover;
        object-position: center;
        width: 30px;
    }
</style>