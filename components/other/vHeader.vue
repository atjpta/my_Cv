<template>
  <div>
    <div class="bg-base-200 pt-1 text-xl">
      <div>
        <div class="md:w-4/5 mx-auto flex justify-between pb-1">
          <nuxt-link to="/" class="btn btn-ghost"> mycv </nuxt-link>

          <!-- pc -->
          <div class="hidden sm:flex">
            <div >
              <nuxtLink
              :to="i.url"
              v-for="i in menu"
              :key="i.url"
              class="btn btn-primary btn-ghost "
            >
              <!-- các tbn -->
              <OtherVIcon class-icon="text-2xl mr-1" :icon="i.icon" />

              {{ i.title }}
            </nuxtLink>
            </div>
          </div>
          <!-- mobie -->
          <div class="flex sm:hidden">
            <nuxtLink
              :to="i.url"
              v-for="i in menu"
              :key="i.url"
              class="btn btn-primary btn-ghost"
            >
              <!-- các tbn -->
              <OtherVIcon class-icon="text-2xl" :icon="i.icon" />
            </nuxtLink>
          </div>
          <OtherVTheme2 />
        </div>
      </div>
      <div class=" pb-2">
        <div
          class="animate-ping border-b-2 border-blue-500 h-1 w-2/5 mx-auto"
        ></div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { icon } from "@fortawesome/fontawesome-svg-core";

const menu = ref([
  {
    url: "/about",
    title: "about",
    icon: "fa-solid fa-address-card",
    datatip: "about",
  },
  {
    url: "/project",
    title: "project",
    icon: "fa-solid fa-layer-group",
    datatip: "project",
  },
  {
    url: "/skill",
    title: "skill",
    icon: "fa-solid fa-laptop-code",
    datatip: "skill",
  },
]);
</script>



<style scoped>
.router-link-exact-active {
  color: white;
  background: rgb(120, 0, 255);
}
</style>