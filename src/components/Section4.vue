<template>
  <div class="bkg">
    <h1>Adestrar seu pet é totalmente possível.</h1>

    <div class="content">
        <div class="TextContent">
            <p>Muitos tutores acolhem filhotes em seus lares sem compreender completamente a extensão dos cuidados e ensinamentos essenciais que serão necessários para o desenvolvimento saudável do pet. Como resultado, enfrentam desafios relacionados aos comportamentos inadequados do filhote.</p>
        </div>
        <div class="ImgContent">
            <img :src="image" alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {
name:'Section4',
data(){
    return{
        image:'./images/pets.png',
    }
}
}
</script>

<style scoped>
.bkg{
    background-color: #DBEEF4;
    height: auto;
    padding: 3%;
    
}

.bkg h1{
    color: #292a2c;
    font-weight: bold;
    font-size: 4em;
    text-align: center;
}

.content{
    display: flex;
    flex-direction: row;
    color: #292a2c;
    justify-content: center;
    align-content: center;
    justify-items: center;
    align-items: center;
    padding: 5%;
}
.TextContent{
    width: 50%;
    margin: 0 auto;
    text-align: left;
    font-size: 26px;

}
.ImgContent{
    width: 50%;
    text-align: center;
}

@media only screen and (max-width: 869px)  {

    .bkg{
    background-color: #DBEEF4;
    height: auto;
    padding: 3%;
    
}

.bkg h1{
    color: #292a2c;
    font-weight: bold;
    font-size: 2em;
    text-align: center;
}

.content{
    display: flex;
    flex-direction: column;
    color: #292a2c;
    justify-content: center;
    align-content: center;
    justify-items: center;
    align-items: center;
}
.TextContent{
    width: 100%;
    margin: 0 auto;
    text-align:center;
    font-size: 26px;

}
.ImgContent{
    width: 100%;
}
.ImgContent img{
    width: 100%;
}
}

</style>