<template>
  <div
    class="sm:mx-auto sm:w-4/5 m-5 p-5 space-y-5 text-white text-center rounded-2xl bg-gradient-to-r from-green-400 to-blue-500"
  >
    <div class="text-5xl">Cao Duc An</div>
    <div class="">A FULL STACK DEVELOPER</div>
    <div class="flex justify-center space-x-5">
      <div v-for="i in data" :key="i.icon">
        <a :href="i.url" class="btn btn-primary btn-outline btn-circle">
          <OtherVIcon class-icon="text-2xl" :icon="i.icon" />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>

import { library } from "@fortawesome/fontawesome-svg-core";
import { faBars } from "@fortawesome/free-solid-svg-icons";
import {
  faTwitter,
  faFacebook,
  faStackOverflow,
  faGithub
} from "@fortawesome/free-brands-svg-icons";
library.add(faBars, faTwitter, faFacebook, faStackOverflow, faGithub);
const data = [
  {
    icon: "fa-brands fa-facebook",
    url: "https://www.facebook.com/atjpta",
  },
  
  {
    icon: "fa-brands fa-github",
    url: "https://github.com/atjpta",
  },
];
</script>

<style>
</style>