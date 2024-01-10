<template>
    <div class="singleBuilding">
        <div class="buttons-togglers">
            <div class="buttons">
                <p>Building 1</p>
                <button @click="showDropDown" v-if="dropDown"><i class='bx bxs-chevron-up'></i></button>
                <button @click="showDropDown" v-else><i class='bx bxs-chevron-down'></i></button>
                <ul v-if="dropDown">
                    <li>Building 1</li>
                    <li>Building 2</li>
                    <li>Building 3</li>
                </ul>
            </div>
            <div class="togglers">
                <p>Global Commands:</p>
                <div>
                    <div class="toggle-button">
                    <span>Turn all heater</span>
                    <input type="checkbox" id="switch1"/>
                    <label for="switch1"></label>
                </div>
                <div class="toggle-button"> 
                    <span>Turn all lights</span>
                    <input type="checkbox" id="switch2"/>
                    <label for="switch2"></label>
                </div>
                </div>
            </div>
        </div>
        <div class="rooms">
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
            <div class="room-card">
                <div class="room-img">
                    <img src="../assets/Buildings/1.jpg" alt="building-1">
                </div>
                <div class="room-info">
                    <div>
                        <h4>Room 1</h4>
                        <span><i class='bx bx-bell' ></i>0</span>
                    </div>
                    <div>
                        <p>Status</p>
                        <p class="ok">OK</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { ref } from 'vue';

export default {
    setup(){
        let dropDown = ref(false);

        const showDropDown = () => {
            dropDown.value = !dropDown.value
        }

        return { dropDown, showDropDown }
    }
}
</script>

<style>
    .singleBuilding{
        border-radius: 5px;
        padding: 20px;   
    }

    .buttons-togglers{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .buttons{
        height: 80%;
        border: 2px solid hsl(192, 100%, 75%) ;
        border-radius: 5px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        background: white;
    }

    .buttons button{
        border: none;
        background: none;
        border-left: 2px solid hsl(192, 100%, 75%);
        height: 100%;
        padding: 0 8px;
        font-weight: 800;
        color: hsl(192, 100%, 75%);
    }

    .buttons ul {
        position: absolute;
        top: 100%;
        left: 0;
        background-color: white;
        border: 1px solid hsl(192, 100%, 75%);
        padding: 5px;
        border-radius: 5px;
        display: inline-block;
        width: 70%;
        color: hsl(192, 100%, 75%);
    }

    .buttons li {
        text-align: center;
    }

    .buttons p{
        font-size: 1.1em;
        color: black;
        padding: 8px 15px;
        color: hsl(192, 64%, 65%);
    }

    .togglers{
        display: flex;
        flex-direction: column;
        background: white;
        padding: 15px;
        border-radius: 5px;
    }

    .togglers p{
        margin-bottom: 10px;
    }

    .togglers div{
        display:  flex;
        align-items: center;
        margin: 0 10px 0 0;
    }

    input[type=checkbox]{
        height: 0;
        width: 0;
        visibility: hidden;
    }

    label {
        cursor: pointer;
        text-indent: -9999px;
        width: 45px;
        height: 20px;
        background: grey;
        display: block;
        border-radius: 100px;
        position: relative;
    }

    label:after {
        content: '';
        position: absolute;
        top: 5px;
        left: 5px;
        width: 10px;
        height: 10px;
        background: #fff;
        border-radius: 90px;
        transition: 0.3s;
    }

    input:checked + label {
        background: hsl(216, 100%, 62%);
    }

    input:checked + label:after {
        left: calc(100% - 5px);
        transform: translateX(-100%);
    }

    label:active:after {
        width: 20px;
    }

    .rooms{
        display: flex;
        justify-content: space-between;
        align-content: center;
        flex-wrap: wrap;
        margin-top: 30px;
        gap: 30px;
    }

    .room-card{
        background: white;
        padding: 20px;
        width: 27%;
        border-radius: 10px;
    }

    .room-img{
        height: 200px;
        width: 100%;
    }

    .room-img img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
        border-radius: 10px;
    }

    .room-info div{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 10px
    }

    .room-info i{
        color: orange;
        font-size: 1.2em;
        background: hsl(39, 92%, 86%);
        border-radius: 5px;
        padding: 5px;
        margin-right: 2px
    }

    .ok{
        color: hsl(120, 91%, 44%);
        font-size: 1em;
        background: hsl(130, 92%, 86%);
        border-radius: 5px;
        padding: 5px;
        margin-right: 2px
    }

</style>