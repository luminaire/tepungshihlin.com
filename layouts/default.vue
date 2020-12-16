<template>
  <div class="container">
    <header>
      <NuxtLink to="/" class="header-logo">
        <img src="/tepung-shihlin-logo.svg" alt="Black Label" />
      </NuxtLink>

      <nav class="header-nav">
        <ul>
          <li>
            <NuxtLink to="/about-us">
              <span>About Us</span>
            </NuxtLink>
          </li>
          <li>
            <NuxtLink to="/shop-now">
              <span>Shop Now</span>
            </NuxtLink>
          </li>
          <li>
            <NuxtLink to="/reseller">
              <strong>Reseller</strong>
            </NuxtLink>
          </li>
        </ul>
      </nav>
    </header>

    <main>
      <Nuxt />
    </main>

    <footer>
      <p>copyright &copy; <strong>blacklabel</strong> {{ year }} </p>
    </footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  computed: {
    year () {
      return new Date().getFullYear();
    },
  },
})
</script>

<style lang="less">
@header-height: 64px;
@navigation-height: 36px;
@navigation-border-height: 4px;
@black: rgba(0, 0, 0, 0.05);
@yellow: #fdd100;

html, body {
  background-color: #fefefe;
  color: #222;
}

.container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

@media (min-width: 1024px) {
  .container {
    margin: 0 auto !important;
    max-width: 960px;
  }
}

@media (min-width: 1280px) {
  .container {
    margin: 0 auto !important;
    max-width: 960px;
  }
}

body {
  margin: 0;
}

header, footer {
  flex: 0 1 auto;
}

main {
  flex : 1;

  @media (min-width: 768px) {
    margin-top: (@header-height + @navigation-height) * -1;
  }
}

header {
  position: relative;
  display: block;
  width: 100%;
  height: @header-height + @navigation-height;
  background: @yellow;
  text-align: center;

  .header-logo {
    display: inline-block;

    img {
      width: auto;
      height: @header-height;
    }
  }

  nav {
    display: block;
    height: @navigation-height;
    line-height: @navigation-height;
    font-size: 20px;

    ul {
      > li {
        display: block;
        float: left;
        width: 33.33333333333%;
        height: @navigation-height;
        line-height: @navigation-height;
        padding: 0 4px;
        text-align: center;

        a {
          display: block;
          width: 100%;
          height: @navigation-height - @navigation-border-height;
          line-height: @navigation-height - @navigation-border-height;
          border-bottom: @navigation-border-height solid transparent;

          &:hover, &:focus {
            border-bottom-color: #222;
          }

          &:visited, &:active {
            border-bottom-color: transparent;
          }

          &.nuxt-link-active,
          &.nuxt-link-exact-active {
            border-bottom-color: #222 !important;
          }
        }
      }
    }

    strong {
      font-size: 28px;
    }
  }

  @media (min-width: 768px) {
    height: @header-height;
    background: @black;

    nav {
      position: absolute;
      top: (@header-height - @navigation-height) / 2;
      right: 0;

      ul {
        display: block;
        float: right;
        margin-right: 16px;

        > li {
          display: block;
          float: left;
          width: auto;
          margin-left: 16px;
        }
      }
    }
  }
}

section {
  padding: 0 16px;
}

.main__title {
  h1 {
    margin: 32px 0 16px;
    font-size: 24px;
  }
}

.main__content {
  p {
    line-height: 20px;
    margin-bottom: 16px;
  }

  ol {
    margin-bottom: 24px;
    padding-left: 24px;
    list-style-type: decimal;

    > li {
      padding-left: 8px;
      margin-bottom: 8px;
    }
  }
}

.main__jumbotron {
  padding: 0;

  img {
    width: 100%;
  }
}

.main__shop-list {
  display: block;

  @media (min-width: 768px) {
    margin: 48px -16px 32px;
  }

  .main__shop-item {
    display: block;
    width: 100%;
    float: left;
    padding: 0 16px;
    text-align: center;

    a {
      display: inline-block;
    }

    @media (min-width: 768px) {
      width: 50%;
    }

    @media (max-width: 767px) {
      margin: 32px auto;
    }
  }
}

.tokopedia {
  background-color: #4f9d4d;
}

.shopee {
  background-color: #e74f26;
}

footer {
  display: block;
  margin-top: 24px;
  padding: 0 16px;

  p {
    display: block;
    background-color: #FDD100;
    line-height: 24px;
    padding: 8px 0;
    border-radius: 24px 24px 0 0;
    text-align: center;
    font-size: 14px;
  }
}
</style>
