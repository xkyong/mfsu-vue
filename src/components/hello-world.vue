<template>
  <div class="hello-world">
    <img src="@/assets/vue.svg" class="logo" alt="Vue logo" />
    <h3 class="title">{{ msg }}</h3>
    <el-button type="primary" @click="sayHello">sayHello</el-button>
    <el-button @click="changeMsg">changeMsg</el-button>
  </div>
</template>
<script setup>
import { ref } from 'vue'

const msg = ref('hello mfsy-vue!')

const sayHello = () => {
  msg.value = 'hello mfsy-vue!'
  console.log(msg.value)
}

const changeMsg = () => (msg.value = 'hello kai!')
</script>
<style lang="scss" scoped>
.hello-world {
  .logo {
    width: 100px;
    height: 100px;
  }

  .title {
    color: #000;
    font-size: 40px;
  }
}
</style>
