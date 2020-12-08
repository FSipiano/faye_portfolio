<template>
  <div>
    <div>
      <nav class="hidden sm:flex" aria-label="Breadcrumb"></nav>
    </div>
    <div class="mt-2 md:flex md:items-center md:justify-between">
      <div class="flex-1 min-w-0">
        <p
          class="text-2xl font-bold leading-7 text-gray-900 sm:text-3xl sm:truncate py-5"
        >
          Front End Developer | Copywriter | UI Designer
        </p>
      </div>
      <div class="mt-4 flex-shrink-0 flex md:mt-0 md:ml-4">
        <nuxt-link to="~/pages/contact.vue"
          ><button
            type="button"
            class="ml-3 inline-flex items-center px-12 py-6 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-green-600 hover:bg-green-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Contact
          </button></nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>