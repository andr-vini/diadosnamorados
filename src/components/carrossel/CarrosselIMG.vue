<script setup>
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import { ref } from 'vue';

const carrossel = ref(null);
const images = [{
  'id': 1,
  'url': '/src/assets/img/img1.jpeg'
},
{
  'id': 2,
  'url': '/src/assets/img/img2.jpeg'
},
{
  'id': 3,
  'url': '/src/assets/img/img3.jpeg'
},
// {
//   'id': 4,
//   'url': '/src/assets/img/img4.jpeg'
// },
{
  'id': 5,
  'url': '/src/assets/img/img5.jpeg'
},
{
  'id': 6,
  'url': '/src/assets/img/img6.jpeg'
},
{
  'id': 7,
  'url': '/src/assets/img/img7.jpeg'
},
{
  'id': 8,
  'url': '/src/assets/img/img8.jpeg'
},
{
  'id': 9,
  'url': '/src/assets/img/img9.jpeg'
},
{
  'id': 10,
  'url': '/src/assets/img/img10.jpeg'
},
{
  'id': 11,
  'url': '/src/assets/img/img11.jpeg'
},
{
  'id': 12,
  'url': '/src/assets/img/img12.jpeg'
},
{
  'id': 13,
  'url': '/src/assets/img/img13.jpeg'
},
{
  'id': 14,
  'url': '/src/assets/img/img14.jpeg'
},
{
  'id': 15,
  'url': '/src/assets/img/img15.jpeg'
},
{
  'id': 16,
  'url': '/src/assets/img/img17.jpeg'
},
{
  'id': 17,
  'url': '/src/assets/img/img17.jpeg'
}
];

const config = {
  gap: 5,
  autoplay: 2000,
  wrapAround: true,
}


</script>

<template>
  <div>
    <Carousel v-bind="config" ref="carrossel">
      <Slide v-for="image in images" :key="image.id">
        <img :src="image.url" alt="image" class="max-h-[400px] rounded-xl" />
      </Slide>
    </Carousel>
  </div>
</template>
