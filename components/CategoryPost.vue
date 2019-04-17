<template>
  <div class="cat-post-cntr row pull-apart">
    <div class="space-wrapper row">
      <div class="cat-post-body col">
        <div class="post-title">
          {{ title }}
        </div>
        <div class="post-desc" v-html="excerpt" />
        <div class="post-footer col">
          <div class="post-author_category">
            Katherine Co in here and Sports
          </div>
          <div class="post-info row">
            <div class="post-info-time row">
              <div class="post-date">
                Mar 29
              </div>
              <div class="post-read_time">
                6 min
              </div>
            </div>
            <div class="post-hashtags row">
              <div class="post-hashtag">
                #SufferNoMore
              </div>
            </div>
          </div>
        </div>
      </div>
      <div id="cat-post" class="responsive-space" />
    </div>
    <div class="cat-post-thumbnail" />
  </div>
</template>

<script>
export default {
  props: {
    title: {
      default: "Oops.. This Post's title has been stolen by a monkey",
      type: String
    },
    excerpt: {
      default: '',
      type: String
    }
  }
}
</script>

<style lang="scss" scoped>
#cat-post {
  width: 5rem;
  flex-shrink: 10;
}

@include upto-sm {
  .post-title{
    font-size: 1rem;
  }
}
</style>
