<script setup>
import { CarrosselIMG } from '@components/carrossel'
</script>

<template>
  <main class="h-screen flex flex-col justify-center items-center bg-[#C8D9E6]">
    <div class="px-10 text-[#B7DOE1] ">
      <p class="text-center text-sm mb-3">Posso até não ser o cara que vai te escrever um poema, ou o que
        vai te escrever uma música. Mas eu sei que tenho o código certo pra te fazer feliz</p>
      <h1 class="text-center text-2xl font-bold">❤️ Te amo infinitamente ❤️</h1>
      <h1 class="text-center text-xl font-bold">❤️ Feliz dia dos namorados ❤️</h1>
      <h1 class="text-center text-lg font-bold"><span class="mr-4">❤️</span> Amor da minha vida <span
          class="ml-4">❤️</span></h1>
    </div>
    <CarrosselIMG />
    <div class="max-w-[300px] space-y-4 mt-4">
      <iframe style="border-radius:12px"
        src="https://open.spotify.com/embed/track/3eJMSq78dDaFb7VvhNFnq6?utm_source=generator" width="100%" height="152"
        frameBorder="0" allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
    </div>

  </main>
</template>
