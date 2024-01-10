<template>
<div class="roomStats">
    <div class="statsHeader">
        <button>Back to building</button>
        <span>Room 442</span>
    </div>
    <div class="mainStats">
        <div>
            <div>
                <p>15°C</p>
                <i class='bx bxs-thermometer'></i>
            </div>
            <span>Humanity</span>
        </div>
        <div>
            <div>
                <p>15°C</p>
                <i class='bx bxs-thermometer'></i>
            </div>
            
            <span>Set Temperature</span>
        </div>
        <div>
            <div>
                <p>15°C</p>
                <i class='bx bx-droplet' ></i>
            </div>
            <span>Humanity</span>
        </div>
        <div>
            <div>
                <p>15°C</p>
                <i class='bx bx-bulb' ></i>
            </div>
            <span>Light Intensity</span>
        </div>
    </div>
    <div class="roomMisc1">
        <div>
            <div>
                <p>Active</p>
                <span>Heating Status</span>
            </div>
            <p class="green">Amet minim moliit non deserunt ullamco est sit aliqua deler do amet sint</p>
        </div>
        <div>
            <div>
                <p>Closed</p>
                <span>Windows Status</span>
            </div>
            <p class="red">Amet minim moliit non deserunt ullamco est sit aliqua deler do amet sint</p>
        </div>
    </div>
    <div class="roomMisc2">
        <div class="tempAndAlarm">
            <div class="temp">
                <div>
                    <p>15°C</p>
                    <i class='bx bxs-thermometer'></i>
                </div>
                <p>Today's Heating Program</p>
            </div>
            <div class="alarm">
                <div>
                    <p>7:45 am°C</p>
                    <i class='bx bx-time-five' ></i>
                </div>
                <p>Start</p>
            </div>
            <div class="alarm">
                <div>
                    <p>10:45 pm°C</p>
                    <i class='bx bx-time-five' ></i>
                </div>
                <p>End</p>
            </div>
        </div>
        <div class="selectNewProg">
            <span>Select New Programs</span>
            <div class="buttons">
                <p>Standard</p>
                <button @click="showDropDown" ><i class='bx bxs-chevron-down'></i></button>
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
    .roomStats{
        display: flex;
        flex-direction: column;   
    }

    .statsHeader{
        display: flex;
        align-items: center;
        gap: 15px;
        margin-bottom: 15px;
    }

    .statsHeader button{
        padding: 10px;
        border-radius: 8px;
        border: 2px solid hsl(192, 100%, 75%);
        color: hsl(192, 100%, 60%);
        font-weight: 600;
    }
    
    .statsHeader span{
        font-size: 1.5em;
        color: black;
        font-weight: bold;
    }

    .mainStats{
        display: flex;
        justify-content: space-between;
        gap: 15px;
    }

    .mainStats > div{
        width: 25%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        background: white;
        border-radius: 8px;
        padding: 20px;
        gap: 10px;
    }

    .mainStats > div > div{    
        display: flex;
        justify-content: space-between;
        align-items: center; 
    }
    
    .mainStats p{
        font-size: 1.5em;
        font-weight: 700;
        color: black;
    }

    .mainStats span{
        text-align: left;
        font-weight: 600;
    }

    .mainStats i{
        font-size: 1.5em;
    }

    .roomMisc1{
        display: flex;
        gap: 15px;
        margin-top: 20px;
    }

    .roomMisc1 > div{
        width: 50%;
        padding: 20px;
        background: white;
        border-radius: 8px;
        display: flex;
        align-items: center;
        gap: 20px;
    }

    .roomMisc1 > div > div{
        width: 50%;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    }

    .roomMisc1 > div > div p{
        color: hsl(199, 100%, 50%);
        background: hsl(194, 100%, 95%);
        border-radius: 3px;
        font-size: .8em;
        font-weight: 600;
        padding: 5px;
        margin-bottom: 5px;
    }

    .roomMisc1 > div > div span{
        white-space: nowrap;
        font-weight: 600;
    }

    p.green{
        color: green;
        background: hsl(120, 100%, 95%);
        padding: 10px;
        border-radius: 5px;
    }

    p.red{
        color: red;
        background: hsl(0, 100%, 95%);
        padding: 10px;
        border-radius: 5px;
    }

    .roomMisc2{
        background: white;
        margin-top: 20px;
        border-radius: 5px;
        padding: 20px;
    }

    .tempAndAlarm{
        margin-bottom: 30px;
        display: flex;
        gap: 20px;
    }

    .tempAndAlarm > div{    
        border: 1px solid #ddd; 
        border-radius: 5px;
        padding: 10px;
    }

    .tempAndAlarm > div > div{    
        display: flex;
        justify-content: space-between;
        align-items: center; 
    }

    .tempAndAlarm > div > div p{    
        font-weight: 600;
        font-size: 1.2em;
        color: black;
    }

    .tempAndAlarm > div p{    
        font-weight: 600;
    }

    .temp{
        width: 50%;
    }

    .alarm{
        width: 25%;
    }

    .selectNewProg{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 10px;
    }

    .selectNewProg button{
        border: none;
        background: none;
        border-left: 2px solid hsl(192, 100%, 75%);
        height: 100%;
        padding: 0 8px;
        font-weight: 800;
        color: hsl(192, 100%, 75%);
    }

</style>