<script setup>
import { ref } from 'vue';
import HelloWorld from './components/HelloWorld.vue'
import { DevicePhoneMobileIcon } from '@heroicons/vue/24/solid'

const favoritePhotosOfHer = ref([
  {
    id: 1
  },
  {
    id: 2
  },
  {
    id: 3
  },
  {
    id: 4
  },
  {
    id: 5
  },
  {
    id: 6
  },
  {
    id: 7
  },
  {
    id: 8
  },
  {
    id: 9
  },
  {
    id: 11
  },
  {
    id: 12
  },
  {
    id: 13
  },
  {
    id: 14
  },
  {
    id: 15
  },
  {
    id: 16
  },
  {
    id: 17
  }
]);
</script>

<template>
  <div class="h-screen ">
    <div class="absolute bg-black" style="top:0; left:0; right:0; bottom:0; z-index: -3;">

    </div>
    <h1 class="text-7xl md:text-9xl text-transparent  text-center mt-3 hero-title fixed"
      style="transform: translate(-50%,-50%); top:45%; left:50%; z-index: -1;">
      <p class="-rotate-15 darumadrop-one-regular">Pat and Judy</p>
    </h1>


    <div class="overlay absolute" style="top:0; left:0; right:0; bottom:0; z-index: 1;">
      <img src="https://www.transparenttextures.com/patterns/asfalt-dark.png" alt="">
    </div>
    <div class="fixed w-120 md:w-140" style="transform: translate(-50%,-50%); top:50%; left:50%; z-index: -3;">
      <video autoplay muted loop id="hero-video">
        <source src="./assets/us.mp4" type="video/mp4">
        <source src="./assets/us.mp4" type="video/ogg">
      </video>
    </div>




  </div>

  <div class="flex justify-center bg-white p-10 p-md-20">
    <div class="container w-6xl">
      <div class="favorite-photos-section">
        <h3 class="text-4xl darumadrop-one-regular text-center mt-3">
          Favorite Photos of You
        </h3>
        <p class="my-4 text-center">
          These photos remind me of how much you truly mean to me. That smile, those sparkling eyes—everything about you
          makes me want to leap with joy!
        </p>
        <div class="photos-of-her-container flex align-top justify-center flex-wrap">
          <div class="photos-of-her m-2 w-3xs" v-for="photo in favoritePhotosOfHer" :key="photo.id" :style="{}">
            <img :src="'/src/assets/jude' + photo.id + '.webp'" alt="">
          </div>
        </div>
      </div>
      <div class="our-story-section py-120">
        <h3 class="text-4xl darumadrop-one-regular text-center mt-3">
           Our Story So Far
        </h3>
        <div class="my-60 flex flex-wrap  md:flex-row-reverse">
          <div class="w-full md:w-1/2 p-10 flex items-center justify-center">
            <DevicePhoneMobileIcon class="size-30 md:size-50 text-blue-700 rotate-30" />
          </div>
          <div class="w-full md:w-1/2 flex items-center justify-center md:px-20">
            <div>
              <h3 class="text-2xl darumadrop-one-regular mb-4">
                  July 2024
                </h3>
                <p>Fate do works in mysterious ways, I have never expect that I will find her from <span class="text-blue-700">facebook online dating</span>. Do I really like this girl? is this just infatuation that I am having? or shes the one.</p>
            </div>
          
          </div>
        
        </div>
        <div class="mt-120 flex flex-wrap">
          <div class="w-full md:w-1/2 flex justify-center">
            <div class="spotify-container rounded-md w-full md:w-100 bg-linear-65 from-amber-500 to-pink-500 p-5 md:p-10 flex" >
              <img src="./assets/elijah.webp" alt="" class="w-25 rounded-md">
              <div class="ml-5 flex items-center">
                <div>
                  <p class="text-2xl text-white font-bold">24/7, 365</p>
                  <p>Elijah Woods</p>
                </div>
                
              </div>
            </div>
          
          </div>
          <div class="w-full md:w-1/2 py-10 md:p-10 flex align-center justify-center">
              <p>Discovered this song as the same time of discovering her. "Seven minutes with you and it's heaven, Ain't hour that rolls by <span class="text-amber-700">I love you</span> 24/7, 3-6-5". </p>
          </div>
        </div>
        <div class="mt-120">
          <div class="flex flex-wrap  md:flex-row-reverse">
            <div class="w-full md:w-1/2 p-10 flex items-center justify-center p-10 md:p-20">
               <img src="./assets/history1.webp" alt="">
            </div>
            <div class="w-full md:w-1/2 flex items-center justify-center md:px-20">
              <div>
                <h3 class="text-2xl darumadrop-one-regular mb-4">
                  August 2024
                </h3>
                <p>I remember this day was the first time you hold my hands thightly its as if you're not gonna let it go and just like that I took a picture of us inside the <span style="color:#834080;">boat we were riding</span> haha.</p>
              </div>
            
            </div>
            
          </div>
        </div>

        <div class="mt-120 flex flex-wrap">
          <div class="w-full md:w-1/2 flex justify-center p-10 md:p-20">
            <img src="./assets/moving_picture.webp" alt="">
          </div>
          <div class="w-full md:w-1/2 py-10 md:p-10 flex items-center justify-center">
            <div>
              <h3 class="text-2xl darumadrop-one-regular mb-4">
                  September 2024
                </h3>
                <p>This was the month that we've accept each other wholeheartedly. Although I do feel a hint of doubt in your heart, you still chose to accept me, <span class="text-red-500"> my love</span> and took the risk of having a relationship with me. I wish I could erase that doubt, but we have a whole lifetime ahead of us to prove our love. </p>
            </div>
           
          </div>
        </div>

      </div>
    </div>
  </div>


  <!-- <div>
    <a href="https://vite.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" /> -->
</template>

<style scoped>
.my-60 {
  margin: 60px 0px 60px 0px;
}
.my-120{
  margin: 120px 0px 120px 0px;
}
.mt-120{
  margin:120px 0px 0px 0px;
}

.py-120{
  padding:120px 0px 120px 0px;
}

.hero-title {
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: white;
  min-width: 100%;
  animation: bigger .5s infinite alternate;

}

#hero-video {
  filter: sepia(70%) contrast(1.2) brightness(0.8);
  width: 500px;
  min-width: 100%;
}

.overlay {
  background: url('https://www.transparenttextures.com/patterns/asfalt-dark.png');
  /* Grainy texture */
  mix-blend-mode: overlay;
  opacity: 1;
  pointer-events: none;
  animation: flicker 0.1s infinite alternate;
}

@keyframes flicker {
  0% {
    opacity: 0.2;
  }

  100% {
    opacity: 0.3;
  }
}

@keyframes bigger {
  0% {
    scale: 1;
  }

  100% {
    scale: 1.009;
  }
}
</style>
