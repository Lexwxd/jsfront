<template>
  <div class="hello">
    <div class="firstcard">
      <div class="text">
        <h1>Сердюков Алексей Иванович</h1>
        <p>БСБО-05-19</p>
      </div>
      <img alt="Vue logo" src="../assets/Paul.jpg" />
      <p class="text">
        Это не военное преступление, если тебе было весело
      </p>
            <!-- <p class="text">
        Мы являемся 6-й танковой армией потому, что у нас в армии всего 6 танков
      </p> -->
    </div>
    <div class="secondcard">
      <form method="get">
      <div class="textar">
        <p>Ваше имя</p>
        <input required id="login"/>
        <p>Почта</p>
        <input required id="password"/>
        <p>Сопроводительное письмо</p>
        <textarea></textarea>
      </div>
      <div>
        <button class="Butt">Кто прочитал тот сдохнет</button>
      </div>
      </form> 
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  margin: 0px 10px;

  display: flex;
  flex-direction: row;
  border: 4px double black; /* Параметры границы */
  background: #fc3; /* Цвет фона */
  padding: 10px; /* Поля вокруг текста */
}
.firstcard {
  margin: 0px 100px;
  max-width: 40%;
  margin-left: auto;
  margin-left: 1.2em;
  border-radius: 25px;
  box-shadow: 0 0 10px aqua;
  background: rgb(27, 20, 20); /* Цвет фона */
}
.secondcard {
  float: left;
  margin: 0px 100px;
  max-width: 40%;
  order: 1;
  margin-right: auto;
  margin-right: 1.2em;
  border-radius: 25px;
  box-shadow: 0 0 10px aqua;
  background: rgb(102, 27, 27); /* Цвет фона */
}
.textar {
  clear: both;
  color: #13e21d;
  border: 10px;
  border-radius: 10px;
}
.textar input{
outline: none;
border: #13e21d;
}
.Butt {

  font-size: 0; line-height: 0;
  scale: 1x;
}

.Butt:hover {
  font-size: 10; line-height: 10;
  transform:scale(8);
}
img {
  height: 200px;
}

.text {
  color: #42b983;
}
.firstcard {
  color: #e21313;
}
</style>
