<template>
     <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Layanan Komparasi</h2>
        </div>
      </div>
      <div class="row">

        <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in portfolioJSON" :key="key">
          <a class="portfolio-link" data-toggle="modal" href="#portfolioModal1">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <img class="img-fluid" src="img/portfolio/01-thumbnail.jpg" alt="">
          </a>
          <div class="portfolio-caption">
            <h4>{{ obj.caption }}</h4>
            <p class="text-muted">{{ obj.title }}</p>
          </div>
        </div>
        
      </div>
    </div>
  </section>
</template>

<script>
export default {
    data: () => ({
        portfolioJSON: [
            {
                img: '/something/random/img.jpg',
                caption: 'Voucher Game Online',
                title: 'Steam Wallet #0'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Voucher Game Online',
                title: 'STEAM Wallet #1'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Voucher Game Online',
                title: 'STEAM Wallet #2'
            }
        ]
    })
}
</script>

<style lang="css">

</style>


