<template>
  <div :id="sectionHead" class="cat-section col --series">
    <CategoryPost v-for="post in catPosts" :key="post.id" :title="post.title" :excerpt="post.excerpt" />
  </div>
</template>

<script>
import CategoryPost from '~/components/CategoryPost.vue'

export default {
  components: {
    CategoryPost
  },
  props: {
    sectionHead: {
      default: '',
      type: String
    },
    catPosts: {
      default: () => {},
      type: [Object, Array]
    }
  }
}
</script>

<style lang="scss" scoped>
.cat-section {
  @include series-col(3.5rem);
}
</style>
