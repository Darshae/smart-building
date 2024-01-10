<template>
  <div class="statistics-tab">
    <div class="headerStats">
        <h3>Statistics</h3>
        <span>Updated 1 Month Ago</span>
    </div>
    <div class="statsMain">
        <div>
            <div class="icon-hold-1">
                <i class='bx bx-cloud-light-rain' ></i>
            </div>
            <div>
                <h4>230g</h4>
                <p>Total Saving</p>
            </div>
        </div>
        <div>
            <div class="icon-hold-2">
                <i class='bx bx-wind' ></i>
            </div>
            <div>
                <h4>134 KG</h4>
                <p>Total co2 Saving</p>
            </div>
        </div>
        <div>
            <div class="icon-hold-3">
                <i class='bx bxl-tailwind-css'></i>
            </div>
            <div>
                <h4>1234 KW/h</h4>
                <p>Total KW/h Saved</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .statistics-tab{
        background: white;
        border-radius: 5px;
        padding: 20px;
    }

    .headerStats{
        display: flex;
        justify-content: space-between;
    }

    .headerStats h3{
        margin: 0;
    }

    .statsMain{
        display: flex;
        align-items: center;
        column-gap: 25%;
        margin-top: 10px;
    }

    .statsMain>div{
        display: flex;
        align-items: center;
        column-gap: 10px;
    }

    .icon-hold-1,
    .icon-hold-2,
    .icon-hold-3
    {   
        padding: 8px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .icon-hold-1 {
        background: hsl(146, 62%, 95%);
        color: hsl(145, 60%, 84%);
    }

    .icon-hold-2 {
        background: hsl(190, 85%, 95%);
        color: hsl(190, 83%, 76%);
    }

    .icon-hold-3 {
        background: hsl(51, 100%, 88%);
        color:  hsl(51, 100%, 40%);
    }

    .statistics-tab p, h4{
        margin: 0;
        text-align: left;
    }

    .statistics-tab p, span{
        font-size: 0.8em;
        color: gray;
    }

    .statistics-tab i{
        font-size: 1.7em
    }
</style>