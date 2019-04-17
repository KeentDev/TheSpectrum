<template>
  <div style="position: relative">
    <section class="splash-section-cntr col center">
      <div class="splash-hero-cntr row pull-bottom pull-left">
        <div class="hero-img-info">
          <div class="hero-title">
            The Spectrm Annual Fellowship Opening Ceremony
          </div>
        </div>
      </div>
      <div class="feat-section-cntr row">
        <div class="feat--full row --series">
          <FeaturedPreview />
          <FeaturedPreview />
          <FeaturedPreview />
        </div>
        <div class="feat--compact col">
          <div class="feat--compact-body row">
            <div class="feat--compact-divider" />
            <div class="feat--compact-content col pull-apart">
              <div class="compact-post">
                <div class="compact-title">
                  Instagram’s New Head of Product Is Betting Big on Commerce
                </div>
              </div>
              <div class="compact-post">
                <div class="compact-title">
                  Signs They’re Attracted To You
                </div>
              </div>
              <div class="compact-post">
                <div class="compact-title">
                  Is Social Media the New Smoking?
                </div>
              </div>
            </div>
          </div>
          <div class="feat--compact-cta section-cta">
            <span>MORE</span>
            <span>FEATURED</span>
          </div>
        </div>
      </div>
      <div class="section-cntr --trending col">
        <div class="section-title">
          TRENDING
        </div>
        <div class="section-body row y-center">
          <div class="hashtags-cntr row --series">
            <div class="hashtag">
              Grad'19
            </div>
            <div class="hashtag">
              Fellowship'19
            </div>
            <div class="hashtag">
              Animo64th
            </div>
            <div class="hashtag">
              SummerSplash19
            </div>
          </div>
          <div class="divider" />
          <div class="section-cta row">
            <span>MORE</span>
            <span>HASHTAGS</span>
          </div>
        </div>
      </div>
    </section>
    <div class="greetings-cntr col center">
      <div class="divider" />
      <div class="greetings-body col center">
        <div class="greetings-head">
          Good Morning.
        </div>
        <div class="greetings-info">
          <div class="breaking_news-info">
            No breaking news yet as of today, Monday.
          </div>
        </div>
      </div>
      <div class="divider" />
    </div>
    <main class="row x-center">
      <div class="cat-cntr row">
        <nav class="sidenav-cntr col">
          <li class="nav-item initial active">
            <a href="#l_speak">L'SPEAK</a>
          </li>
          <li class="nav-item">
            <a href="#editorial">EDITORIAL</a>
          </li>
          <li class="nav-item">
            <a href="#entertainment">FUN</a>
          </li>
          <li class="nav-item">
            <a href="#sports">SPORTS</a>
          </li>
          <li class="nav-item">
            <a href="#health">HEALTH</a>
          </li>
        </nav>
        <div class="col cat-post_list-cntr --series">
          <CategorySection section-head="l_speak" :cat-posts="posts" />
          <CategorySection section-head="editorial" :cat-posts="posts" />
          <CategorySection section-head="entertainment" :cat-posts="posts" />
          <CategorySection section-head="sports" :cat-posts="posts" />
        </div>
      </div>
      <div id="cat_popular" class="responsive-space--custom" />
      <div class="popular-cntr">
        <div class="-wrap col">
          <div class="section-head --popular">
            Popular on The Spectrum
          </div>
          <div class="section-body --popular --series">
            <div class="cat-post-body col">
              <div class="post-title">
                Why is Silicon Valley So Obsessed With the Virtue of Suffering?
              </div>
              <div class="post-footer col">
                <div class="post-author_category">
                  Katherine Co Sports
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
            <div class="cat-post-body col">
              <div class="post-title">
                7 Tax Experts on How to Ace Tax Season
              </div>
              <div class="post-footer col">
                <div class="post-author_category">
                  Alvin in Tips n' Tricks
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
            <div class="cat-post-body col">
              <div class="post-title">
                Strategies to Pull Yourself Out of a Bad Mood
              </div>
              <div class="post-footer col">
                <div class="post-author_category">
                  Marian in Wellness
                </div>
                <div class="post-info row">
                  <div class="post-info-time row">
                    <div class="post-date">
                      Mar 25
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
          </div>
        </div>
      </div>
      <div id="main" class="responsive-space" />
    </main>
  </div>
</template>

<script>
import FeaturedPreview from '~/components/FeaturedPreview'
import CategorySection from '~/components/CategorySection'

export default {
  components: {
    FeaturedPreview,
    CategorySection
  },
  data() {
    return {
      posts: [
        { title: 'title 1', id: 1 },
        { title: 'title 2', id: 2 }
      ]
    }
  }
}
</script>

<style lang="scss">

.cat-post_list-cntr {
  width: 100%;
  padding: 22px 32px;
  @include series-col(8rem);
  max-width: 642px;
  display: inline-flex;
}

.sidenav-cntr {
  // border-right: 1px solid #E4E4E4;
  padding-right: 18px;
  position: sticky;
  height: calc(100vh - 4rem);
  top: 2rem;
  display: inline-flex;
}

.cat-cntr {
  width: auto;
  position: sticky;
  top: 0px;
  flex-shrink: .2;
}

.nav-item {
  font-size: 14px;
  list-style: none;
  text-align: right;
  margin: 8px 0;
  transform-origin: right;
  transform: scale(1);
  opacity: .5;
  a{
    text-decoration: none;
    color: #222;
  }
  &.active{
    font-weight: 600;
    // margin: 22px 0;
    color: #222;
    opacity: 1;
  }
}

main {
  padding: 3rem 6rem;
}
#main {
  max-width: 2rem;
  width: 100%;
  flex-shrink: 4;
}

.section-head {
  &.--popular{
    font-size: 20px;
    font-weight: 600;
    color: #222;
    margin-bottom: 12px;
    &::after{
      content: '';
      display: block;
      width: 100%;
      height: 1px;
      background-color: rgba(black, .12);
      margin: 20px 0;
    }
  }
}

.section-body {
  &.--popular{
    @include series-col(32px);
  }
}

.--popular {
  .post-footer{
    margin-top: 6px;
  }
}

.popular-cntr {
  position: sticky;
  top: 2rem;
  height: calc(100vh - 4rem);
  flex-shrink: 1.5;
  .-wrap {
    max-width: 275px;
    width: 100%;
  }
  .post-title {
    font-size: 16px;
  }
}

#cat_popular {
  max-width: 4rem;
  width: 100%;
  flex-shrink: 4;
}

// SPLASH

.splash-section-cntr {
  background-color: #2A2A2A;
  padding: 0 2rem;
}

.splash-hero-cntr {
  height: 87vh;
  max-width: 1200px;
  width: 100%;
  background-color: #414141;
  padding: 2rem 2.5rem;
  box-sizing: border-box;
}

.hero-img-info {
  color: white;
}

.page-logo {
  font-family: 'Georgia', serif;
  font-size: 24px;
  font-weight: 600;
  margin-bottom: 2rem;
}

.hero-title {
  font-size: 20px;
  font-weight: 600;
  max-width: 370px;
  &::before{
    content: '';
    display: block;
    width: 2.5rem;
    height: 1px;
    background-color: white;
    opacity: .15;
    margin: 1rem 0;
  }
}

.feat-section-cntr{
  max-width: 1200px;
  width: 100%;
  margin: 2rem 0;
  box-sizing: border-box;
  padding-left: 2.25rem;
}

.feat--full{
  width: 100%;
  padding-bottom: 3rem;
  @include series-row(1rem);
}

.compact-title{
  color: #EFEFEF;
  font-size: 14px;
  font-weight: 500;
}

.feat--compact-cta{
  margin: 1rem 14px;
  margin-bottom: 0;
  span{
    &:last-child{
      margin-left: 0px !important;
    }
  }
}

.section-cta{
  font-size: 12px;
  font-weight: 600;
  color: #EFEFEF;
  & > span{
    &:last-child{
      color: #5DD0E9;
      margin-left: 3px;
    }
  }
}

.feat--compact-divider{
  width: 1px;
  height: 100%;
  background-color: rgba(white, .12);
  margin: 0 18px;
}

.feat--compact-content{
  max-width: 200px;
  width: 100%;
  padding: 14px 0;
}

.feat--compact-body{
  height: 100%;
}

.feat--compact{
  margin-left: 20px;
}

// TRENDING

.section-cntr{
  &.--trending{
    max-width: 1200px;
    width: 100%;
    padding: 0 2.25rem;
    box-sizing: border-box;
    .section-title{
      font-size: 14px;
      color: rgba(white, .75);
      position: relative;
      &::before{
        content: '#';
        display: block;
        font-weight: 500;
        font-size: 18px;
        color: rgba(white, .45);
        position: absolute;
        transform: translate(calc(-100% - 8px), -50%);
        top: 50%;
      }
    }
    .section-body{
      margin: 22px 0;
    }
    .hashtag{
      color: #999;
    }
    .hashtags-cntr {
      @include series-row(2rem);
    }
    .divider{
      width: 100%;
      height: 1px;
      background-color: rgba(white, .12);
      margin: 0 1rem;
    }
  }
}

// GREETINGS/BREAKING NEWS

.greetings-cntr{
  max-width: 1200px;
  margin: 0 auto;
  padding: 4rem 8rem;
  margin-top: 1rem;
  & > .divider {
    max-width: 5rem;
    width: 100%;
    height: 1px;
    background-color: #E1E1E1;
    &:first-child {
      max-width: 6.5rem;
    }
  }
}

.greetings-body{
  margin: 2rem 0;
}

.greetings-head{
  font-size: 24px;
  font-family: 'Georgia', serif;
  font-weight: 600;
  margin-bottom: 6px;
}

.greetings-head, .greetings-info {
  white-space: nowrap;
}

.breaking_news-info{
  color: #9F9F9F;
}

.breaking_news-cta{
  font-size: 14px;
  a{
    color: #999;
  }
}

@include upto-sm {
  main {
    padding: 3rem 0;
    flex-direction: column !important;
  }
  .cat-post_list-cntr {
    padding: 22px 1rem;
    max-width: auto;
    display: inline-block;
  }
  .sidenav-cntr {
    flex-direction: row;
    position: relative;
    height: auto;
    margin: 2rem 0;
    display: none;
  }
  .greetings-cntr{
    padding: 4rem 1rem;
    margin: 0;
  }
  .section-cntr{
    &.--trending{
      .section-body{
        flex-direction: column;
        align-items: flex-end;
      }
      .divider{
        max-width: 1rem;
        width: 1px;
        height: 1rem;
        margin: .75rem 6px;
      }
      .hashtags-cntr {
        flex-wrap: wrap;
      }
    }
  }
  .hashtag{
    line-height: 2em;
  }
  .cat-cntr {
    flex-direction: column;
  }
  .nav-item {
    flex-direction: inline-flex;
  }
}
</style>
