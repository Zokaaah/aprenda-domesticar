<template>
  <div class="bannerbkg">

    <div class="banner">
        <h1>Aprenda a<br/>domesticar seu pet</h1>
        <button class="btnStart">Quero começar</button>
    </div>

  </div>
  <b-container>

  <div class="stats">
    <div v-for="(item) in Stats" :key="item.id" class="icones" >
                        <img  :src="item.icon" alt="">
                        <br/>
                        <h3>{{item.name}}</h3>
                    </div>

  </div>
</b-container>
</template>

<script>
export default {
name:'Banner',

data(){
    return{
        Stats:[
                    {id:1, name:'Pagamento seguro', icon:'./images/pagseguro.png'},
                    {id:2, name:'Acesso seguro', icon:'./images/acesseguro.png'},
                    {id:3, name:'Garantia 7 dias', icon:'./images/garantia.png'},
                ],
    }
}

}
</script>

<style scoped>
.banner{
   justify-content: center;
   align-items: center;
   justify-items: center;
   align-content: center;
   margin:0 auto !important;
   font-weight: bold !important;
    
}

.bannerbkg{
    background-image: url(../assets/banner.png); 
    height: 780px;
    width: 100%;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    text-align: center;

}

h1{
    color: #fff;
    font-size: 80px;
    font-weight: bold !important;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin-top: -20px;
}
.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    padding: 2%;
    font-size: 32px;
    border: none;
    cursor: pointer;
    transition: all 0.3s;
    -webkit-transition: width 1s;
    transition: width 1s;
    -webkit-transition: all .5s;
    -moz-transition: all .5s;
    transition: all .5s;
}
.btnStart:hover{
    transform: scale(1.1);

}
.stats{
    background-color: #292a2c;
    text-align: center;
    display: flex;
    flex-direction: row;
    justify-content: center;
    height: 250px;


}
.icones{
    margin-top: 2%;
    margin-bottom: 2%;

    width: 35%;
}

h3{
    font-weight: bold;
    font-size: 1.2em;
}


@media only screen and (max-width: 869px)  {

    .stats{
    background-color: #292a2c;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
    align-items: center;
    height: 100%;
padding: 5%;

}
.icones{
    margin-top: 2%;
    margin-bottom: 2%;

    width: 35%;
}

h1{
    color: #fff;
    font-size: 40px;
    font-weight: bold !important;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin-top: -20px;
}
}



</style>