<template>
  <div class="section3">
    <div class="content">
        <h1>Somente hoje você paga este valor para a ter acesso a todo conteudo do curso de adestrador de pets</h1>

        <h2>4x de R$9,98</h2>
        <h2>ou</h2>
        <h2>R$ 49,90 a vista</h2>
        <button class="btnStart">Comprar</button>

    </div>
  </div>
</template>

<script>
export default {
name:'Section3'
}
</script>

<style scoped>

.section3{
    background-color:#F4BC28;
    padding: 3%;
    display: flex;
    justify-content: center;
    align-content: center;
    height: 1000px;
    justify-items: center;
    align-items: center;
}

.content{
    background-color: #3A8ADB;
    height: auto;
    width: 1240px;
    justify-content: center;
    border-radius: 20px;
    text-align: center;
    padding: 5%;
    color: #fff;
}

.content h1{
    font-weight: bold;
    margin-bottom:2% ;
    font-size: 3em;
}
.content h2{
    font-size: 4em;
    font-weight: bold;
}

.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    width: 400px;
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

@media only screen and (max-width: 869px)  {
    .section3{
    background-color:#F4BC28;
    padding: 3%;
    display: flex;
    justify-content: center;
    align-content: center;
    height: auto;
    justify-items: center;
    align-items: center;
}

.content{
    background-color: #3A8ADB;
    height: auto;
    width: 100% !important;
    justify-content: center;
    border-radius: 20px;
    text-align: center;
    padding: 10%;
    color: #fff;
}

.content h1{
    font-weight: bold;
    font-size: 22px;
}
.content h2{
    font-size: 2em;
    font-weight: bold;
}

.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    width: 100%;
    padding: 2%;
    font-size: 26px;
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
}
</style>