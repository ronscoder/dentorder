<template>
  <div class="container">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide
        caption=""
        text=""
        v-bind:img-src="cimages[0]">
        <h1>Fixed Partial Denture
          </h1></b-carousel-slide>

      <b-carousel-slide v-bind:img-src="cimages[1]">
        <h1>Fixed Partial Denture
          </h1>
      </b-carousel-slide>

    </b-carousel>
  </div>
</template>

<script>
import c1 from "../assets/1.jpg";
import c2 from "../assets/5.jpg";
  export default {
    data() {
      return {
        slide: 0,
        sliding: null,
        cimages: [c1, c2]
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>
<style scoped>
.container{
    width: 100%;
    overflow:scroll;
    /* box-shadow: 0 0 4px 0px; */
}
</style>
