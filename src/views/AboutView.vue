<template>
  <div class="about">
    <div class="name">{{ text }}</div>
    <button @click="changeTextTH">change to thai</button>
    <br>
    <button @click="changeTextENG">change to english</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: 'Narongkiad'
    }
  },
  methods: {
    changeTextTH() {
      this.text = 'ณรงค์เกียรติ';
    },
    changeTextENG() {
      this.text = 'Narongkiad';
    }
  }
}
</script>


<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}

.name{
  color: aqua;
  text-align: center;
  font-size: 50px;
}
</style>