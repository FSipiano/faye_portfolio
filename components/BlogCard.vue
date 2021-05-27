<template>
<div class="relative bg-gray-50 pt-3 pb-2 px-4 sm:px-6 lg:pt-14 lg:pb-18 lg:px-8">
  <div class="absolute inset-0">
    <div class="bg-white h-1/3 sm:h-2/3">
    </div>
  </div>
  <div class="relative hover:opacity-50 max-w-7xl mx-auto">
   <a :href=post.url>
    
    <div class="mt-2 max-w-lg mx-auto gap-5 lg:grid-cols-3 lg:max-w-none">
      <div class="flex flex-col rounded-lg shadow-lg overflow-hidden">
        <div class="flex-shrink-0">
          <img class="h-48 w-full object-cover" :src=post.cover_image>
        </div>
        <div class="flex-1 bg-white p-6 flex flex-col justify-between">
          <div class="flex-1">
            <p class="text-sm font-medium text-grey-300">
              <a class="">
                {{ post.description }}
              </a>
            </p>
            <a href="#" class="block mt-2">
              <p class="text-xl font-semibold text-gray-900">
                  {{post.title}}
              </p>
              <p class="mt-3 text-base text-gray-500">
             {{ post.public_reactions_count }} reactions
              </p>
            </a>
          </div>
        </div>
      </div>
    </div>
    </a>
  </div>
</div>  
</template>
<script>
export default {
  props: [ 'post' ]

}
</script>

<style>


</style>