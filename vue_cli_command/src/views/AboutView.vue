<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <Button type="primary">Primary</Button>

<div class="carousel">
   <Carousel v-model="value" loop>
      <CarouselItem v-for="item in 4" :key="item">
          <div class="demo-carousel">
             <img :src="require(`@/assets/image/0${item}.png`)" >
          </div>
      </CarouselItem>
    </Carousel>
</div>
   
</template>


<script>
    export default {
        data () {
            return {
                value: 0
            }
        }
    }
</script>