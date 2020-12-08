<template>
  <section>
    <Navbar class="py-5 px-12"></Navbar>
    <div class="container">
      <div>
        <h1 class="title">Faye_Sipiano</h1>
        <h2 class="subtitle">Web developer</h2>
        <h3 class="subtitle">Copywriter</h3>
        <h4 class="subtitle">UI Designer</h4>
        <div class="links">
          <a
            href="https://www.youtube.com/channel/UCQap2rd2RT364EyxJsx9GYw?view_as=subscriber"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-red-600 hover:bg-red-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Youtube
          </a>
          <a
            href="https://twitter.com/javascriptcoff1"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-blue-500 hover:bg-blue-400 focus:outline-none focus:ring-2 focus:ring-offset-2; focus:ring-indigo-500"
          >
            Twitter
          </a>
          <a
            href="https://github.com/FSipiano"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-black hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            GitHub
          </a>
        </div>
        <p class="paragraph pt-24 px-36">
          Hi, I'm Faye. I love coding, writing, and driving. I also ride horses
          and cook.
        </p>
        <p class="paragraph pt-6">I write copy for multiple
          industries, including Education, Transport and have won award entries in Finance.
        </p>
        <p class="paragraph py-6">
          I design and build beautiful websites using Vue.js, Nuxt.js, and
          Tailwind.
        </p>
        <p class="paragraph pb-4">Let's work together to create your vision.</p>
        <div class="justify-center mt-4 flex-shrink-0 flex md:mt-0 md:ml-4">
          <nuxt-link to="./pages/contact.vue"
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
  </section>
</template>

<script>
export default {
  components: {

  },
};
</script>

<style>
/* .container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto
} */

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}

.paragraph {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-size: 24px;
  color: #000000;
}
</style>
