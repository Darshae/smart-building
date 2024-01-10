<template>
  <div class="optionBuildings">
    <div>
        <div class="img-hold">
            <img src="../../assets/Buildings/2.jpg" alt="building-1">
        </div>
        <h5>Building 1</h5>
        <div class="info-tab">
            <div>
                <h4>100%</h4>
                <p>Active</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Alarms</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Saving</p>
            </div>
        </div>
    </div>
    <div>
        <div class="img-hold">
            <img src="../../assets/Buildings/3.jpg" alt="building-1">
        </div>
        <h5>Building 1</h5>
        <div class="info-tab">
            <div>
                <h4>100%</h4>
                <p>Active</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Alarms</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Saving</p>
            </div>
        </div>
    </div>
    <div>
        <div class="img-hold">
            <img src="../../assets/Buildings/4.jpg" alt="building-1">
        </div>
        <h5>Building 1</h5>
        <div class="info-tab">
            <div>
                <h4>100%</h4>
                <p>Active</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Alarms</p>
            </div>
            <div>
                <h4>230g</h4>
                <p>Saving</p>
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
    .optionBuildings{
        justify-content: space-between;
        border-radius: 5px;
        display: flex;
        gap: 50px;
    }

    .optionBuildings>div{
        background: white;
        padding: 20px;
        border-radius: 5px;
    }

    .optionBuildings h5 {
        font-size: 1.1em;
        text-align: left;
        margin: 10px 5px;
    }

    .optionBuildings p{
        margin: 0;
    }

    .optionBuildings h4{
        color: hsl(191, 85%, 60%);
        margin: 5px 0;
        text-align: left;
    }

</style>