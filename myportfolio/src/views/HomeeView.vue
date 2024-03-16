<template>
<div class="herosection">
<div class="blackback"></div>
<div class="mypic">
    <img :src="profileimg" alt="" class="pic">
</div>

</div>
</template>

<script>
import profileimg from "../assets/profileimg.png" 
export default{
data(){
    return{
    profileimg: profileimg,
    }
}
}
</script>

<style scoped>

.herosection{
    width: 100vw;
    height: 100vh;
    display: grid;
    grid-template-columns: 1fr 0.5fr 1fr;
    grid-template-rows:0.5fr 1fr 0.5fr 1fr;
}
.blackback{
    width: 100%;
    height: 100%;
    background-color: #151719;
    border-radius: 100% 0% 100% 0% / 81% 57% 43% 19% ;
    grid-column: 1 / 4;
    grid-row: 3 / 5;
}

.mypic{
    grid-column: 1 / 3;
    grid-row: 2 / 5;
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: start;
    align-items: end; 
}

.pic{
    height: 100%;
}
</style>
<!-- width: 100%;
 -->