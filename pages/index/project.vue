<template>
  <div class="w-4/5 mx-auto">
    <div class="text-center text-6xl mb-5 uppercase font-bold">My project</div>

    <div class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-4 ">

      <div v-for="i in data" :key="i.url">
        <div class="card h-96 bg-base-100 shadow-xl ">
        <figure class="px-10 mt-5">
          <img v-if="i.id == 1" src="~~/assets/image/blog.png" alt="ảnh mô tả" class="rounded-xl" />
          <img v-if="i.id == 2" src="~~/assets/image/chat.png" alt="ảnh mô tả" class="rounded-xl" />
          <img v-if="i.id == 3" src="~~/assets/image/battle_slime.png" alt="ảnh mô tả" class="rounded-xl" />
        </figure>
        <div class="card-body items-center text-center">
          <h2 class="card-title">{{i.title}}</h2>
          <p>
            {{i.content}}
          </p>
          <div class="card-actions">
            <a
              :href="i.url"
              class="btn btn-primary"
              >Read Now</a
            >
          </div>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const data = ref([
  {
    id : 1,
    title: "wblog",
    content: " it is web blog Information Technology, u can post blog, question, comment,...",
    img: "~~/assets/image/blog.png",
    url: "https://github.com/atjpta/ct466_wblog.git",
  },
  {
    id : 2,
    title: "wbchat",
    content: "it is web chat real time 1:1, u can chat freely with each other",
    img: "../../assets/image/blog.png",
    url: "https://github.com/atjpta/wbchat-app",
  },
  {
    id : 3,
    title: "game battle slime",
    content: "it is game 2d turn base in android, u can win?",
    img: "~~/assets/image/battle_slime.png",
    url: "https://drive.google.com/drive/folders/1pvWwC-FYbT4aYTY47Lg9MewjmsPqrwft?usp=share_link",
  },
]);
</script>

<style>
</style>