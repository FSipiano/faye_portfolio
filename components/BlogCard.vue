<template>
<div class="relative bg-gray-50 pt-10 pb-10 px-4 sm:px-6 lg:pt-24 lg:pb-28 lg:px-8">
  <div class="absolute inset-0">
    <div class="bg-white h-1/3 sm:h-2/3">
    </div>
  </div>
  <div class="relative hover:opacity-50 max-w-7xl mx-auto">
   <a :href=post.url>
    
    <div class="mt-4 max-w-lg mx-auto grid gap-5 lg:grid-cols-3 lg:max-w-none">
      <div class="flex flex-col rounded-lg shadow-lg overflow-hidden">
        <div class="flex-shrink-0">
          <img class="h-48 w-full object-cover" :src=post.cover_image>
        </div>
        <div class="flex-1 bg-white p-6 flex flex-col justify-between">
          <div class="flex-1">
            <p class="text-sm font-medium text-grey-500">
              <a class="font-semibold">
                {{post.description}}
              </a>
            </p>
            <a href="#" class="block mt-2">
              <p class="text-xl font-semibold text-gray-900">
                  {{post.title}}
              </p>
              <p class="mt-3 text-base text-gray-500">
             
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