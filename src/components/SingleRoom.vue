<template>
  <div class="singleRoom">
    <div class="headerChosenRoom">
        <p>Room 1</p>
        <span><i class='bx bx-bell' ></i>0</span>
        <div>
            <span>Status:</span>
            <span class="ok">OK</span>
        </div>
    </div>
    <div class="chosenRoomImg">
        <img src="../assets/Room/1.jpg" alt="Room 1">
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
    </div>
</template>

<script>
export default {

}
</script>

<style>
    .singleRoom{
        padding: 20px;
        background: white;
        border-radius: 5px;
    }

    .headerChosenRoom{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .chosenRoomImg{
        margin-top: 15px;
        height: 600px;
        width: 100%;
    }

    .chosenRoomImg img{
        height: 100%;
        width: 100%;
        border-radius: 5px;
    }

    .headerChosenRoom i{
        color: orange;
        font-size: 1.2em;
        background: hsl(39, 92%, 86%);
        border-radius: 5px;
        padding: 5px;
        margin-right: 2px
    }
</style>