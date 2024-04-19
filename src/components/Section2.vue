<template>
  <div>
    <div class="banner">
       <h1>Nesse curso você aprenderá</h1>

       <b-container>

<div class="capitulos">
  <div v-for="(item) in Caps" :key="item.id" class="cards" >
                      <h2>{{ item.name }}</h2>
                      <br/>
                      <h3>{{item.desc}}</h3>
                  </div>
</div>
</b-container>
    </div>
  </div>
</template>

<script>
export default {
    name:'Section2',
    data(){
    return{
        Caps:[
                    {id:1, name:'Capítulo 1: Noções básicas de treinamento para pets', desc:'Neste módulo introdutório, você será imerso no mundo do adestramento de pets, descobrindo os fundamentos essenciais para estabelecer uma relação harmoniosa e eficaz com seu companheiro peludo.'},
                    {id:2, name:'Capítulo 2: Conhecendo seu pet', desc:'Neste capítulo, mergulharemos profundamente na compreensão individual do seu fiel amigo de quatro patas. Exploraremos as características únicas da personalidade, comportamento e linguagem corporal do seu pet.'},
                    {id:3, name:'Capítulo 3: Aprendendo sobre recursos e como usá-los', desc:'Neste capítulo, vamos explorar uma variedade de recursos que podem ser úteis no processo de treinamento do seu pet.'},
                    {id:4, name:'Capítulo 4: Dando ordens a seu pet', desc:'Neste capítulo, entraremos no cerne do treinamento: a comunicação eficaz entre você e seu pet por meio de comandos.'},

                ],
    }
}

}
</script>

<style scoped>
.banner{
    background-color: #3A8ADB;
    height: 1047px;
    padding: 3%;
}

h1{
    color: #fff;
    text-align: center;
    font-weight: bold;
    margin-bottom: 5%;
}

h2{
    font-weight: bold;
}

.capitulos{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    
}

.cards{
    height: 310px;
    width: 47%;
    background-color: #f4f4f4;
    border-radius: 14px;
    color: #2C3E50;
    text-align: center;
    justify-content: center;
    justify-items: center;
    align-content: center;
    align-items: center;
    margin-top: 3%;
    padding: 2%;
}

@media only screen and (max-width: 869px)  {
    .capitulos{
    display: flex;
    flex-direction: column;
    justify-content: center;
    
}

.cards{
    height: 310px;
    width: 100%;
    background-color: #f4f4f4;
    border-radius: 14px;
    color: #2C3E50;
    text-align: center;
    justify-content: center;
    justify-items: center;
    align-content: center;
    align-items: center;
    margin-top: 3%;
    padding: 2%;
    box-shadow: 0 1px 1px rgba(0,0,0,0.12), 
              0 2px 2px rgba(0,0,0,0.12), 
              0 4px 4px rgba(0,0,0,0.12), 
              0 8px 8px rgba(0,0,0,0.12),
              0 16px 16px rgba(0,0,0,0.12);
}
.banner{
    background-color: #3A8ADB;
    height: 100%;
    padding: 3%;
}
}


</style>