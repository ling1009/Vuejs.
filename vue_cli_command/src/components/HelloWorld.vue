
// ~~~~~~~~~~~~~~~~~~~~ HelloWorld 組件 ~~~~~~~~~~~~~~~~~~~~  
<template>
  <div class="hello">
    <div class="img" v-for="item in 4" :key="item">
      <img :src="require(`@/assets/image/0${item}.png`)" >
    </div>

    <div>
      <p>{{ title }}</p>
      <h1>{{ msg }}</h1>
      <p>消費滿1500免運</p>
      <select>
        <option>尺寸</option>
        <option>S</option>
        <option>M</option>
        <option>L</option>
      </select>

      <button>加入購物車</button>
      <button>立即購買</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: String,
    msg: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

 .img{
  width: 30%;
 }

 img{
  width: 100%;
  height: 100%;
 }
</style>
