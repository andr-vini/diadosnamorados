<script setup>
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import { ref } from 'vue';
import img1 from '@assets/img/img1.jpeg';
import img2 from '@assets/img/img2.jpeg';
import img3 from '@assets/img/img3.jpeg';
// import img4 from '@assets/img/img4.jpeg';
import img5 from '@assets/img/img5.jpeg';
import img6 from '@assets/img/img6.jpeg';
import img7 from '@assets/img/img7.jpeg';
import img8 from '@assets/img/img8.jpeg';
import img9 from '@assets/img/img9.jpeg';
import img10 from '@assets/img/img10.jpeg';
import img11 from '@assets/img/img11.jpeg';
import img12 from '@assets/img/img12.jpeg';
import img13 from '@assets/img/img13.jpeg';
import img14 from '@assets/img/img14.jpeg';
import img15 from '@assets/img/img15.jpeg';
import img16 from '@assets/img/img16.jpeg';
import img17 from '@assets/img/img17.jpeg';

const carrossel = ref(null);
const images = [{
  'id': 1,
  'url': img1
},
{
  'id': 2,
  'url': img2
},
{
  'id': 3,
  'url': img3
},
// {
//   'id': 4,
//   'url': img4
// },
{
  'id': 5,
  'url': img5
},
{
  'id': 6,
  'url': img6
},
{
  'id': 7,
  'url': img7
},
{
  'id': 8,
  'url': img8
},
{
  'id': 9,
  'url': img9
},
{
  'id': 10,
  'url': img10
},
{
  'id': 11,
  'url': img11
},
{
  'id': 12,
  'url': img12
},
{
  'id': 13,
  'url': img13
},
{
  'id': 14,
  'url': img14
},
{
  'id': 15,
  'url': img15
},
{
  'id': 16,
  'url': img16
},
{
  'id': 17,
  'url': img17
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
