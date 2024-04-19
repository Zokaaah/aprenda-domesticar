<template>
  <div class="content">
    <h1>Receba também um bônus se comprar hoje</h1>
    <div class="cards">
        <div v-for="(item) in Cards" :key="item.id" class="card" >
                      <h2 class="number">{{ item.id }}</h2><h2> {{ item.name }}</h2>
                      <br/>
                      <h3>{{item.desc}}</h3>
                  </div>
    </div>

    <div class="btnContent">
        <button class="btnStart">Quero comprar</button>
    </div>
  </div>
</template>

<script>
export default {
name:'Section5',

data(){
    return{
        Cards:[
                    {id:1, name:'Passeio perfeito', desc:'Neste módulo adicional, você será guiado na arte de proporcionar ao seu pet passeios seguros, divertidos e gratificantes. Exploraremos técnicas para ensinar seu pet a se comportar adequadamente durante os passeios, desde a familiarização com a coleira e guia até a prática de caminhadas sem puxar.'},
                    {id:2, name:'Obediência Avançada', desc:'Neste módulo avançado, mergulharemos em técnicas e conceitos que levarão o treinamento de seu pet a um nível superior de habilidade e compreensão. Você aprenderá a aprimorar comandos básicos, introduzindo variações e refinamentos que desafiarão o intelecto de seu pet.'},

                ],
    }}
}
</script>

<style scoped>



.cards{
    flex-direction: row !important;
    display: flex;
    padding: 5%;
    justify-content: center;
}

.number{
background-color: #3A8ADB;
  color: #fff;
  width: 80px;
  height: 80px;
  text-align: center;
  border-radius: 15px;
  line-height: 80px;
  justify-items: center;
  margin-bottom: 5%;
  font-size: 3em;

    
}
.card{
    margin-right: 3%;
    padding: 3%;
    color: #292a2c;
    width: 50%;
    background-color: #F5F5F5;
    box-shadow: 0 1px 1px rgba(0,0,0,0.12), 
              0 2px 2px rgba(0,0,0,0.12), 
              0 4px 4px rgba(0,0,0,0.12), 
              0 8px 8px rgba(0,0,0,0.12),
              0 16px 16px rgba(0,0,0,0.12);

    border-radius: 20px;
}

.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    width: auto;
    padding: 2%;
    font-size: 28px;
    border: none;
    cursor: pointer;
    transition: all 0.3s;
    -webkit-transition: width 1s;
    transition: width 1s;
    -webkit-transition: all .5s;
    -moz-transition: all .5s;
    transition: all .5s;
   float: left;
}
.btnStart:hover{
    transform: scale(1.1);

}

.btnContent{
    display: flex;
    justify-content: center;
    margin-bottom: 3%;
}

@media only screen and (max-width: 869px)  {
    .cards{
    flex-direction: column !important;
    display: flex;
    padding: 5%;
}

.card{
    margin-top: 3%;
    margin-right: 3%;
    padding: 8%;
    color: #292a2c;
    width: 100%;
    background-color: #F5F5F5;
    box-shadow: 0 1px 1px rgba(0,0,0,0.12), 
              0 2px 2px rgba(0,0,0,0.12), 
              0 4px 4px rgba(0,0,0,0.12), 
              0 8px 8px rgba(0,0,0,0.12),
              0 16px 16px rgba(0,0,0,0.12);
    border-radius: 20px;
}
}

</style>