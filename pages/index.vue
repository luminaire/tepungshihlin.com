<template>
  <div>
    <section class="main__jumbotron">
      <img src="/home-main-banner-tepung-shihlin.png" alt="Selamat Datang di TepungShihlin.com!" />
    </section>

    <section class="main__uvp-list clearfix">
      <div class="main__uvp-item">
        <img src="/tepung-shihlin-usp-1.png" alt="Sejak 2015" />
      </div>
      <div class="main__uvp-item">
        <img src="/tepung-shihlin-usp-2.png" alt="Resep asli Taiwan diproduksi oleh SDM lokal berpengalaman" />
      </div>
      <div class="main__uvp-item">
        <img src="/tepung-shihlin-usp-3.png" alt="Izin Edar P-IRT" />
      </div>
      <div class="main__uvp-item">
        <img src="/tepung-shihlin-usp-4.png" alt="10.000 ++ paket terjual" />
      </div>
    </section>

    <section class="main__title">
      <h1>
        <strong>About</strong><span>Us</span>
      </h1>
    </section>

    <section class="main__content">
      <p>
        <strong>TepungShihlin.com</strong> adalah website resmi dari produk tepung crispy taiwan blacklabel.
      </p>
      <p>
        <span>Pertama dimulai pada tahun 2015 di Tangerang, berbekal dgn resep asli dari Taiwan dan dikelola oleh SDM lokal yang berpengalaman di bidang nya masing-masing...</span>
        <NuxtLink to="/reseller">read more</NuxtLink>
      </p>
    </section>

    <section class="main__title">
      <h1>
        <strong>Shop</strong><span>Now</span>
      </h1>
    </section>

    <section class="main__shop-list clearfix">
      <div class="main__shop-item">
        <a href="https://www.tokopedia.com/tokohokiku">
          <img src="/tepung-shihlin-toped.png" alt="Belanja di Tokopedia!" />
        </a>
      </div>
      <div class="main__shop-item">
        <a href="https://shopee.co.id/blacklabel_id">
          <img src="/tepung-shihlin-shopee.png" alt="Belanja di Shopee!" />
        </a>
      </div>
    </section>

    <section class="main__title">
      <h1>
        <strong>Reseller</strong><span>Program</span>
      </h1>
    </section>

    <section class="main__content">
      <p>Produk Tepung crispy taiwan merupakan salah satu produk yang cukup digemari, dan banyak dicari oleh konsumen indonesia, karena selain lebih hemat, pastinya lebih sehat juga</p>
      <p>
        <span>Tentunya ini membuka peluang besar bagi para calon usahawan yang ingin ikut memasarkan produk ini...</span>
        <NuxtLink to="/reseller">read more</NuxtLink>
      </p>
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  layout: 'default'
})
</script>

<style lang="less" scoped>
.main__shop-list {
  margin: 0 -16px;

  .main__shop-item {
    margin: 8px 0;

    a {
      display: block;
    }

    img {
      width: 100%;
      height: auto;
    }

    @media (min-width: 768px) {
      margin: 0 0 32px;
    }
  }
}

.main__uvp-list {
  margin: 32px -16px 0;

  .main__uvp-item {
    display: block;
    width: 50%;
    float: left;
    padding: 0 32px;

    @media (min-width: 768px) {
      width: 25%;
    }

    img {
      width: 100%;
      height: auto;
      border-radius: 50%;
      background-color: #EEE;
    }
  }
}
</style>
