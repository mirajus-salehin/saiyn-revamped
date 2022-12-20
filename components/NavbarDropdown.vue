<template>
  <li id="button_admin" class="relative nav-item group mb-1 md:mb-0">
    <a
      class="font-semibold whitespace-no-wrap"
      href=""
    >
      <span class="firstlevel">Amministra</span>
    </a>
    <ul
      class="
        absolute
        left-0
        top-0
        mt-10
        p-2
        rounded-lg
        shadow-lg
        bg-white
        z-10
        hidden
        group-hover:block
      "
    >
      <svg
        class="
          block
          fill-current
          text-white
          w-4
          h-4
          absolute
          left-0
          top-0
          ml-3
          -mt-3
          z-0
        "
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
      >
        <path
          d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"
        />
      </svg>
      <li
        class="
         mx-1
          px-4
          py-2
          whitespace-no-wrap
          rounded-md
          text-sm
          md:text-base
          text-black
          hover:text-green-700 hover:bg-gray-50
        "
      >
        <a
          class="px-2 py-1"
          href=""
        >
          <span class="">Funzioni ed opzioni</span>
        </a>
      </li>
      <li
        class="
         mx-1
          px-4
          py-2
          whitespace-no-wrap
          rounded-md
          text-sm
          md:text-base
          text-black
          hover:text-green-700 hover:bg-gray-50
        "
      >
        <a
          class="px-2 py-1"
          href=""
        >
          <span class="">Gestore Pacchetti</span>
        </a>
      </li>
      <li
        class="
         mx-1
          px-4
          py-2
          whitespace-no-wrap
          rounded-md
          text-sm
          md:text-base
          text-black
          hover:text-green-700 hover:bg-gray-50
        "
      >
        <a
          class="px-2 py-1"
          href=""
        >
          <span class="">Permessi</span>
        </a>
      </li>
    </ul>
  </li>
</template>

<script>
export default {}
</script>

<style>
.group:hover .group-hover\:block {
  display: block !important;
}
li {
  @apply list-none;
}
</style>
