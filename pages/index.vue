<template>
  <div class="container">
    <div>
      <Logo />
      <vue-flip active-click class="card">
        <template v-slot:front> <div class="front1">front</div> </template>
        <template v-slot:back> <div class="back1">back</div> </template>
      </vue-flip>
    </div>
  </div>
</template>

<script>
import VueFlip from 'vue-flip'
export default {
  name: 'index',
  components: { VueFlip }
}
</script>

<style lang="scss" scoped>
.card {
  width: 300px;
  height: 300px;
  margin-left: auto;
  margin-right: auto;
}
.back1 {
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  width: 300px;
  height: 300px;
  background-color: #ffc107;
}
.front1 {
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  width: 300px;
  height: 300px;
  background-color: #673ab7;
}
</style>
