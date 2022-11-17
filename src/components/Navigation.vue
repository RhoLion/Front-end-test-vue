<template>
    <div class="bg-secondary shadow-lg md:flex justify-between m">
      <!-- LOGO -->
      <span class="ml-48 mt-4 mb-2">
        <img src="../assets/logo.png"  alt="Logotipo">
      </span>
      <!-- MENU -->
        <ul class="md:flex md:items-center mr-48 mb-4 ">
          <li class="md:mx-4" v-for="link in Links" :key="link">
            <a href="link.link"  class="font-semibold text-primary-300 hover:text-primaryVariant-300">{{link.name}}</a>
          </li>
        </ul>
      </div>
</template>
<script>
export default {
  setup(){
    const Links = [
      {name : 'Home', link : '#'},
      {name : 'Category', link : '#'},
      {name : 'About Me', link : '#'},
      {name : 'Search', link : '#'},
    ]
    return {Links}
  }
}
</script>
