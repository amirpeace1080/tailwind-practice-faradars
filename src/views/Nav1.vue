<template>
  <div class="bg-cyan-400">
    <nav class="p-5 bg-white shadow md:flex md:items-center md:justify-between">
      <div class="flex justify-between items-center">
        <span class="text-2xl font[Poppins] cursor-pointer">
          <img
              class="h-10 inline"
              src="data:image/png;base64,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"
              alt="">
          TailwindCss
        </span>
        <span class="text-3xl cursor-pointer md:hidden mx-2 block" @click="showMenu =! showMenu">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd" />
          </svg>
        </span>
      </div>

      <ul v-show="showMenu" class="md:flex md:items-center z-[-1] md:z-auto absolute bg-white w-full left-0 md:w-auto md:py-0 py-4 md:pl-0 pl-7 md:opacity-100 opacity-0 top-[400] transition-all ease-in duration-500">
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-xl hover:text-cyan-500 duration-500">HOME</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-xl hover:text-cyan-500 duration-500">SERVICE</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-xl hover:text-cyan-500 duration-500">ABOUT</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-xl hover:text-cyan-500 duration-500">CONTACT</a>
        </li>
        <li class="mx-4 my-6 md:my-0">
          <a href="#" class="text-xl hover:text-cyan-500 duration-500">BLOG'S</a>
        </li>

        <button class="bg-cyan-400 text-white text[Poppins] duration-500 px-6 py-2 hover:bg-cyan-500 rounded">Get Started</button>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Nav1",
  data() {
    return{
      showMenu: true,
    }
  }
}
</script>

<style scoped>

</style>