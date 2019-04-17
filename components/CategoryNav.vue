<template>
  <div class="row center">
    <div class="cat-nav-cntr row center">
      <div class="cat-nav-wrap row y-center">
        <div class="current-category row y-center pull-right">
          L'SPEAK
        </div>
        <div class="divider" />
        <div class="category-list row y-center pull-left">
          <div class="cat-item">
            Cat 1
          </div>
          <div class="cat-item">
            Cat 2
          </div>
          <div class="cat-item">
            Cat 3
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .cat-nav-cntr {
    height: 3rem;
    width: 100%;
    box-shadow: 1px 6px 28px -26px rgba(0,0,0,.2), 1px 3px 36px -4px rgba(0,0,0,.18);
  }

  .cat-nav-wrap {
    max-width: $max-width;
    width: 100%;
    height: 100%;
    // outline: 1px solid red;
  }

  .current-category {
    max-width: $main-outer_space;
    width: 100%;
    font-size: 20px;
    font-weight: 600;
    color: #212121;
    line-height: 1em;
    margin-bottom: -4px;
  }

  .cat-item {
    line-height: 1em;
    margin-bottom: -4px;
  }

  .divider {
    height: 19px;
    width: 1px;
    background-color: $divider-color;
    margin: 0 $gutter;
    flex-shrink: 0;
  }
</style>
