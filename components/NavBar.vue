<template>
  <nav>
    <div class="flex justify-between items-center pt-6 pr-10">
      <div class="w-64 px-6">
        <img src="../assets/images/logo.png" alt="">
      </div>
      <div ref="menu" class="hidden md:flex justify-between space-x-4 pr-6">
        <a href="" class="nav-item">Research field</a>
        <a href="" class="nav-item">Lab facilities</a>
        <a href="" class="nav-item">Publications</a>
        <a href="" class="nav-item">Youth network</a>
        <NavbarDropdown />
        <a href="" class="nav-item">Partners</a>
      </div>

      <div class="flex md:hidden button">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6 transition-all"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </div>
    </div>
    <!--mobile menu-->
    <div class="mobile-menu hidden md:hidden mr-2 bg-white">
      <div class="flex flex-col gap-2">
        <a href="" class="nav-item">Research field</a>
        <a href="" class="nav-item">Research item</a>
        <a href="" class="nav-item">Lab facilities</a>
        <a href="" class="nav-item">Publications</a>
        <a href="" class="nav-item">Youth network</a>
        <a href="" class="nav-item">Partners</a>
        <NavbarDropdown />
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  mounted () {
    const button = document.querySelector('div.button')
    const menu = document.querySelector('div.mobile-menu')
    button.addEventListener('click', () => {
      menu.classList.toggle('hidden')
    })
  }
}
</script>

<style>
.nav-item {
  @apply px-6 py-2 hover:cursor-pointer hover:bg-green-700 hover:text-white rounded-xl font-bold transition duration-500;
}
.mobile-nav {
  @apply px-6 py-2 bg-white;
}
a.nuxt-link-active {
  @apply text-white font-bold;
}
.group:hover .group-hover\:block {
  display: block !important;
}
li{
  @apply list-none;
}
</style>
