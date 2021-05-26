<template>
<section>

<ul>
    <li v-for="post in posts" :key="post.title">
      <!-- {{ item.name }} - {{ item.price }} -->
      <BlogCard :post="post">
</BlogCard>
    </li>
  </ul>

</section>
</template>
<script>
import BlogCard from '~/components/BlogCard.vue';

export default {
  
data() {
return {
    posts: []
}
 },
 async fetch() {
      this.posts = await fetch(
        'https://dev.to/api/articles?username=javascriptcoff1&per_page=5'
      ).then(res => res.json())
    }
  }

</script>

