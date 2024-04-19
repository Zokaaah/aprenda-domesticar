<template>
  <div class="content">

    <div class="content1">
        <h1>Dúvidas?</h1>
        <p>Entre em contato comigo pelo whatsapp para retirar qualquer duvida</p>
    </div>

    <div class="content2">
       <button class="btnStart">Whatsapp</button>
    </div>
  </div>
</template>

<script>
export default {
name:'FooterVue'
}
</script>

<style scoped>

.content{
    background-color: #0E0C0C;
    color: #fff;
    padding: 5%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    text-align: center;
}

.content1{
    width: 50%;
    font-weight: bold;
}
.content1 h1{
    font-size: 36px;

}

.content2{
    width: 50%;
}
.content1 p{
    font-size: 22px;
}

.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    width: 400px;
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
}
.btnStart:hover{
    transform: scale(1.1);

}

@media only screen and (max-width: 869px)  {
 
    .content{
    background-color: #0E0C0C;
    color: #fff;
    padding: 7%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    overflow-x: hidden !important;
}

.content1{
    width: 100%;
    font-weight: bold;
}
.content1 h1{
    font-size: 26px;

}

.content2{
    width: 100%;
}
.content1 p{
    font-size: 18px;
}

.btnStart{
    background-color: #18AC39;
    color: #fff;
    font-weight: bold;
    border-radius: 14px;
    margin-top: 5%;
    width: auto;
    padding: 2%;
    font-size: 24px;
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