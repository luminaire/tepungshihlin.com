<template>
  <div>
    <section class="main__jumbotron">
      <img src="/reseller-tepung-shihlin.png" alt="Belanja di TepungShihlin.com!" />
    </section>

    <section class="main__title">
      <h1>
        <strong>Reseller</strong><span>Program</span>
      </h1>
    </section>

    <section class="main__content">
      <p>Produk Tepung crispy taiwan merupakan salah satu produk yang cukup digemari, dan banyak dicari oleh konsumen indonesia, karena selain lebih hemat, pastinya lebih sehat juga</p>
      <p>Tentunya ini membuka peluang besar bagi para calon usahawan yang ingin ikut memasarkan produk ini.</p>
      <p>Bergabunglah menjadi mitra usaha reseller kami bersama dengan puluhan reseller lainnya, dapatkan penawaran harga diskon dengan margin yg sangat menarik khusus untuk anda!</p>
      <p>Dan ingat penawaran yang menarik selalu Terbatas!! 😉</p>
      <p>Klik link dibawah ini untuk informasi lebih lanjut!</p>
    </section>

    <section class="main__contact-us">
      <a href="tiny.cc/oivkgz">
        <img src="/tepung-shihlin-WA.svg" alt="Hubungi kami via WhatsApp!" />
      </a>
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  layout: 'default',
  head: {
    title: 'Reseller | TepungShihlin.com',
    meta: [
      { hid: 'description', name: 'description', content: 'TepungShihlin.com adalah website resmi dari produk tepung crispy taiwan blacklabel.' },
    ],
  },
})
</script>

<style lang="less" scoped>
.main__contact-us {
  display: block;
  width: 75%;
  margin: 32px auto;

  @media (min-width: 768px) {
    width: 50%;
  }
}
</style>
