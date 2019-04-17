<template>
  <nav class="site-nav row center">
    <div class="site-nav-wrap row pull-apart">
      <div class="row">
        <div class="site-logo row center">
          THE<span>S</span>PECTRUM
        </div>
        <div class="site-menu-items row --series">
          <div class="menu-item row center">
            THE SPECTRES
          </div>
          <div class="menu-item row center">
            TERMS OF USE
          </div>
        </div>
      </div>
      <div class="site-cta_options row center --series">
        <div class="menu-item site-search">
          SEARCH
        </div>
        <div class="menu-item site-cta-btn">
          <div>REACH US</div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.site-nav{
  background-color: #212121;
  height: $header-height;
  width: 100%;
  box-sizing: border-box;
  position: fixed;
  top: 0;
  box-sizing: border-box;
}

.site-nav-wrap{
  max-width: $max-width;
  width: 100%;
  height: 100%;
}

.site-logo{
  font-family: 'Georgia', serif;
  font-size: 21px;
  font-weight: 600;
  color: white;
  margin-right: 10px;
  white-space: nowrap;
  span {
    font-size: 23px;
    margin-bottom: 2px;
  }
}

.menu-item{
  font-size: 13px;
  font-weight: 600;
  color: rgba(white, .65);
}

.site-menu-items{
  margin: 0 22px;
  @include series-row(22px);
}

.site-cta_options{
  @include series-row(22px)
}

.site-cta-btn{
  background-color: #3483f7;
  padding: 5px 15px;
  border-radius: 5px;
  margin-top: -4px;
  color: white;
  & > div{
    margin-top: 4px;
  }
}
</style>
