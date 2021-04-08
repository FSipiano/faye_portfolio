<template>
  <section class="page">
    <Navbar class="py-5 px-12"></Navbar>
    <div class="container">
      <div>
        <h1 class="title lg:text-6xl">Faye_Sipiano</h1>

        <h2 class="subtitle"> Developer Advocate at <a class ="subtitle underline"
        href="https://raycast.com">Raycast
        </a></h2>

        <div class="links">
            <a
            href="https://dev.to/javascriptcoff1"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-black hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Dev.to
          </a>
          <a
            href="https://www.youtube.com/channel/UCQap2rd2RT364EyxJsx9GYw?view_as=subscriber"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-red-700 hover:bg-red-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
            >
              Youtube
          </a>
          <a
            href="https://twitter.com/javascriptcoff1"
            target="_blank"
            rel="noopener noreferrer"
            class="ml-3 font-bold inline-flex items-center px-4 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-blue-700 hover:bg-blue-400 focus:outline-none focus:ring-2 focus:ring-offset-2; focus:ring-indigo-500"
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
        <p class="paragraph pt-24 px-36 sm: px-6">
          Hi, I'm Faye. I love learning about coding and writing about what I have learned.
          I also ride horses, enjoy roadtrips and cooking.
        </p>         
        <p class="paragraph pt-6 sm: px-6 pb-4">I have written copy for multiple
          industries, including Education, Transport and have won award entries in Finance.
          I also specialise in explaining difficult technological concepts in an accessible way.
          You can view my blog posts by following the Dev link above.
        </p>
        <div class="justify-center mt-4 flex-shrink-0 flex md:mt-0 md:ml-4 mb-10">
          <ContactButton
          ></ContactButton>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
   data() {
      return {
        title: 'Faye_Sipiano - Home'
      }
    },
    head() {
      return {
        title: this.title,
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'My custom description'
          }
        ]
      }
    },

  components: {

  },
};
</script>

<style>
/* .container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto
} */

.page {
  background-color: #e2d8d896;
}

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
  font-size: 60px;
  color: #35495e;
  letter-spacing: 2px;
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
  font-size: 28px;
  color: #000000;
}
</style>
