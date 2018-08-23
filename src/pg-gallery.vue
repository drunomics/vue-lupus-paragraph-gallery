<template>
  <div class="paragraph paragraph--gallery">
    <div class="paragraph__title">
      {{ dataName }}
    </div>
    <lupus-slider
      arrows="1"
      bullets="1"
      autoplay="0"
    >
      <lupus-slider-slide
        v-for="image in images"
      >
        <img 
          :alt="image.alt" 
          :src="image.src"
        >
      </lupus-slider-slide>
    </lupus-slider>
  </div>
</template>
<script>
import { LupusSlider, LupusSliderSlide } from 'vue-lupus-slider';
export default {
  name: 'PgGallery',
  components: {
    'lupus-slider': LupusSlider,
    'lupus-slider-slide': LupusSliderSlide,
  },
  props: {
    dataName: { type: String, default: () => '' },
    dataImages: { type: String, default: () => ''}
  },
  computed: {
    images() {
      return JSON.parse(this.dataImages);
    },
  },
};
</script>
