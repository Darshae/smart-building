<template>
  <div class="featuredTab">
    <div class="image-tab">
        <div class="img-hold">
            <img src="../../assets/Buildings/1.jpg" alt="building-1">
        </div>
        <h3>Building 1</h3>
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
    <div class="indicator-tab">
        <div class="indicator-1">
            <p>Key Performance indicators</p>
            <div>
                <div>
                    <ul>
                        <li><span>10</span>/10 heating thermostat active</li>
                        <li><span>5</span>/5 heating thermostat active</li>
                        <li><span>0</span>/20 Windows Open</li>
                        <li><span>10</span>/10 Room temp Reduced</li>
                        <li><span>5</span>/5 Activities iauntihid</li>
                    </ul>
                </div>
                <div class="divButton">
                    <button>View Building</button>
                </div>
            </div>
            
        </div>
        <div class="indicator-2">
            <p>Alarms</p>
            <div>
                <ul>
                    <li><i class='bx bx-bell' ></i> Dining room</li>
                    <li><i class='bx bx-bell' ></i> Bed room</li>
                </ul>
                <div class="`divButton`">
                    <button>View Room</button>
                </div>
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
    .featuredTab{
        background: white;
        border-radius: 5px;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 30px;
        padding: 15px;
        text-align: left;
    }

    .featuredTab p{
        margin: 0;
    }

    .featuredTab h4{
        color: hsl(191, 85%, 60%);
        margin: 5px 0;
        text-align: left;
    }

    .featuredTab h3{
        font-size: 1.1em;
        margin: 0;
        text-align: left;
        margin: 5px;
    }

    .image-tab{
        display: flex;
        flex-direction: column;
        gap: 2px;
    }

    .img-hold{
        height: 170px;
        width: 390px;
    }

    .img-hold img{
        height: 100%;
        width: 100%;
        object-fit: cover;
        object-position: center;
        border-radius: 5px;
    }

    .info-tab{
        display: flex;
        justify-content: space-between;
        gap: 10px;
    }

    .info-tab>div{
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        border: 1px solid hsla(0, 0%, 87%, 0.5);
        border-radius: 5px;
        padding: 5px;
        width: 25%;
    }

    .info-tab h4{
        font-size: 1.2em;
        letter-spacing: 0.2px;
        margin-bottom: 10px;
    }
    
    .info-tab p{
        font-size: 0.8em;
        color: gray;
    }

    .indicator-tab p{
        color: gray;
        font-size: 0.8em;
        font-weight: bold;
    }

    .indicator-1,
    .indicator-2{
        display: flex;
        flex-direction: column;
        border: solid 1px hsla(0, 0%, 87%, 0.5);
        border-radius: 5px;
        padding: 10px;
        margin: 10px 0;
    }

    .indicator-1>div, 
    .indicator-2>div{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .indicator-1 ul{
        list-style: disc;
        display: flex;
        flex-wrap: wrap;
        padding: 5px 0px;
        margin: 0;
    }

    .indicator-1 li{
        margin: 15px 50px 0px 20px;
        letter-spacing: 0.5px;
    }

    .indicator-2 ul{
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding: 5px 0px;
        margin: 0;

    }

    .indicator-1 span{
        font-size: 1.2em;
        color: black;
        font-weight: bold;
    }

    .indicator-2 li{
        display: flex;
        align-items: center;
        margin: 0;
        font-weight: 600;
    }

    .indicator-2 i{
        color: hsl(29, 100%, 66%);
        font-size: 1.2em;
        background: hsl(30, 100%, 94%);
        border-radius: 5px;
        padding: 5px;
        margin: 5px 10px 5px 0px;
    }

    .featuredTab button{
        white-space: nowrap;
        color: white;
        background: hsl(245, 82%, 67%);
        border: none;
        border-radius: 5px;
        padding: 12px 20px;
        font-size: 1em;
        letter-spacing: 1.5px;
    }
</style>