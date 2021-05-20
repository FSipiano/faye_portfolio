<template>
 <div class="relative px-6 py-6 page">
  <div class="relative pt-12 pb-16 px-4 sm:pt-16 sm:px-6 lg:px-8 lg:max-w-7xl lg:mx-auto lg:grid lg:grid-cols-2">
    <div class="lg:pr-8">
      <div class="max-w-md mx-auto sm:max-w-lg lg:mx-0">
        <h2 class="text-3xl font-extrabold tracking-tight sm:text-4xl">
          Let's work together to create your vision
        </h2>
        <p class="text-lg text-gray-700 sm:mt-3">
          I’d love to hear from you! Send me an email,
<a class="text-lg mb-6 text-indigo-600 text-decoration: underline sm:mt-3"
           href="https://twitter.com/JavaScriptCoff1">
        a DM on Twitter,
        </a>
     or use the form below and
          I'll respond as soon as I can!
        </p>

        <p class="text-lg text-gray-700 sm:mt-3">Email me at:</p>
        <a class="text-2xl mb-6 text-indigo-600 text-decoration: underline sm:mt-3"
        href="mailto:fayesipiano@outlook.com">
          fayesipiano@outlook.com
        </a>

        <form enctype=”multipart/form-data” action="https://formsubmit.co/fayesipiano@outlook.com" method="POST" class="mt-12 grid grid-cols-1 gap-y-6 sm:grid-cols-2 sm:gap-x-8">
          <div>
            <label for="first_name" class="block text-sm font-medium text-gray-700">First name</label>
            <div class="mt-1">
              <input
              type="text"
              name="first_name" id="first_name"
              autocomplete="given-name" required autofocus
              class="input border border-gray-700 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600">
            </div>
          </div>
          <div>
            <label for="last_name" class="block text-sm font-medium text-gray-700 required">Last name</label>
            <div class="mt-1">
              <input type="text" name="last_name" id="last_name" autocomplete="family-name" required
              class="input border border-gray-600 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600 required">
            </div>
          </div>
          <div class="sm:col-span-2">
            <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
            <div class="mt-1">
              <input id="email" name="email" type="email" required
              autocomplete="email"
              class="input border border-gray-600 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600">
            </div>
          </div>
          <div class="sm:col-span-2">
            <label for="company" class="block text-sm font-medium text-gray-700">Company</label>
            <div class="mt-1">
              <input
              type="text"
              name="company"
              id="company"
              autocomplete="organization" required
              class="input border border-gray-600 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600">
            </div>
          </div>
          <div class="sm:col-span-2">
            <div class="flex justify-between">
              <label
              for="phone"
              class="block text-sm font-medium text-gray-700">Phone</label>
              <span id="phone_description"
              class="text-sm text-gray-700">Optional</span>
            </div>
            <div class="mt-1">
              <input
              type="text"
              name="phone" id="phone"
              autocomplete="tel"
              aria-describedby="phone_description"
              class="input border border-gray-600 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600">
            </div>
          </div>
          <div class="sm:col-span-2">
            <div class="flex justify-between">
              <label
              for="how_can_we_help"
              required
              class="block text-sm  pr-6 font-medium text-gray-700">What did you have in mind?
                I can help you to design, develop and build, write, market and strategise
              </label>
              <span id="how_can_we_help_description" class="text-sm text-gray-700">Max. 500 characters</span>
            </div>
            <div class="mt-1">
              <textarea id="how_can_we_help"
              name="how_can_we_help"
              aria-describedby="how_can_we_help_description"
              rows="4"
              class="input border border-gray-600 appearance-none rounded w-full px-3 py-3 pt-5 pb-2 focus focus:border-indigo-600 focus:outline-none active:outline-none active:border-indigo-600"></textarea>
            </div>
          </div>
          <div class="text-right sm:col-span-2">
            <button
            type="submit"
            class="text-lg inline-flex font-bold items-center px-8 py-4 border border-transparent rounded-md text-white bg-green-700 hover:bg-green-600 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">
              Submit
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  data(){
   return {
        title: 'Faye_Sipiano - Contact'
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
    }
}
</script>
<style>
.page {
  background-color: #d3cbcb96;
}
</style>