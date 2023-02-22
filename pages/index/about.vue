<template>
  <div class="w-4/5 mx-auto">
    <div class="text-center text-6xl mb-5 uppercase font-bold">about me</div>
    <div class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-4">
      <!-- trái -->
      <div class="">
        <img
          class="  rounded-2xl bg-base-200 "
          src="~~/assets/image/avatar.jpg"
          alt=""
        />
      </div>
      <!-- giữa -->
      <div class="text-center  p-5 rounded-2xl bg-base-200 ">
        <div class="text-4xl mb-3">SUMMARY</div>
        <ul style="list-style-type: circle" class="text-left pl-5">
          <li>I am a final year student.</li>
          <li>I am currently majoring in Information Technology.</li>
          <li>my goal is to become a full stack developer.</li>
        </ul>
        <p class="text-left mt-5 indent-8">
          With the experience gained from self-study, I firmly believe that it will help the company grow more and more.
        </p>
        <a download
          href="~~/assets/CV_Cao_Duc_An_Fullstack_Developer.pdf"
          class="btn btn-primary btn-outline mt-5"
        >
          <OtherVIcon class-icon=" mr-1" icon="fa-solid fa-download" />
          my cv
        </a>
      </div>

      <!-- phải -->
      <div class="p-5 text-center rounded-2xl bg-base-200">
        <div class="text-4xl mb-5">CONTACT INFO</div>
        <div class="sm:flex-col">
          <div class="sm:text-left">
            <div class=" btn no-animation btn-ghost ">
            <OtherVIcon icon="fa-solid fa-location-dot" class-icon=" mr-3"></OtherVIcon>
            ninh kieu, can tho, viet nam
          </div>
          </div>
          <div class="sm:text-left">
            <div class="btn no-animation btn-ghost ">
            <OtherVIcon icon="fa-solid fa-phone" class-icon=" mr-3"></OtherVIcon>
            +84 342622915
          </div>
          </div>
          <div class="sm:text-left">
            <div class="btn no-animation btn-ghost ">
            <OtherVIcon icon="fa-solid fa-envelope" class-icon=" mr-3"></OtherVIcon>
            caoducan351@gmail.com
          </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>