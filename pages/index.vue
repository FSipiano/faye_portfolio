import Vue from 'vue'
import axios from 'axios'
import VueAxios from 'vue-axios'
import ContactButton from './components/ContactButton'
<template>
  <section class="page">
    <div class="container">
      <div>
        <ContactButton class="mt-10"
          ></ContactButton>
        <h1 class="title">Faye_Sipiano</h1>

        <h2 class="subtitle"> Freelance tech writer and community-builder
        </h2>
        <div class="links">
            <a
            href="https://dev.to/javascriptcoff1"
            target="_blank"
            rel="noopener noreferrer"
            class="mt-10 font-bold inline-flex px-3 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-black hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Dev.to
          </a>
          <a
            href="https://www.youtube.com/channel/UCQap2rd2RT364EyxJsx9GYw?view_as=subscriber"
            target="_blank"
            rel="noopener noreferrer"
            class="mt-2 font-bold inline-flex px-3 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-red-700 hover:bg-red-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
            >
              Youtube
          </a>
          <a
            href="https://github.com/FSipiano"
            target="_blank"
            rel="noopener noreferrer"
            class="mt-2 font-bold inline-flex px-3 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-black hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            GitHub
          </a>
          <a
            href="https://twitter.com/javascriptcoff1"
            target="_blank"
            rel="noopener noreferrer"
            class="mt-2 font-bold inline-flex px-3 py-2 border border-transparent rounded-md shadow-sm text-md font-medium text-white bg-blue-700 hover:bg-blue-400 focus:outline-none focus:ring-2 focus:ring-offset-2; focus:ring-indigo-500"
          >
              Twitter
          </a>
        </div>
         <div>
        <img class="profile"
        :src="profileImage">
        </div>
        <p class="paragraph pt-20 px-36 sm:px-6">
          Hi, I'm Faye.
        </p>
        <p class="paragraph pt-4 px-6 pb-4">I love learning about coding and writing about what I have learned.
          I also ride horses, enjoy roadtrips and cooking. 
          I have written copy for multiple
          industries, including Finance, NFT gaming, Science, Education and Transport, and have prepared winning submissions for awards in FinTech 
          as well as funding applications for tech start-ups.
        </p> 
        <p class="paragraph pt-4 px-6 pb-4">
          I specialise in explaining difficult technological concepts in a way that everyone can understand.
          Below is a selection of my recent posts.
          I also maintain an Open Source 
          <a class = "underline text-indigo-700"
          href= "https://github.com/FSipiano/newbieDictionary">
          Newbie Dictionary
          </a>
          on GitHub that aims to give newcomers a helping hand through the overwhelming jargon in this industry.
        </p>
        <div class="justify-center flex-shrink-0 flex md:mt-0 md:ml-4 mb-10">
        <BlogCardContainer
        ></BlogCardContainer>
        </div>
        <div class="justify-center flex-shrink-0 flex md:mt-0 md:ml-4 mb-10">
          <ContactButton
          ></ContactButton>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ContactButton from '~/components/ContactButton.vue';
import BlogCardContainer from '~/components/BlogCardContainer.vue';
export default {
   data() {
      return {
        title: 'Faye_Sipiano - Home',
        profileImage: require('@/static/profile.jpg')
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
    ContactButton,
    BlogCardContainer

  },
};
</script>

<style>
@media
 (max-width: 300px) { 
   .container { 
     max-width: 100%}
     }

.container { max-width: 80% }

.page {
  background-color: #d3cbcb96;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 400px;
  font-size: 48px;
  color: #35495e;
  letter-spacing: 2px;
}


.subtitle {
  font-size: 32px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  display: block;
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  margin-bottom: 45px;
}

.paragraph {

  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-size: 20px;
  color: #000000;
}

.profile {
  border-radius: 5%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 35%;
}
</style>
