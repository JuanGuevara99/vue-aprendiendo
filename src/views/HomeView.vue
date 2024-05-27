<template>
  <section id="home" class="d-flex align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 d-flex flex-column justify-content-center pt-4 pt-lg-0 order-2 order-lg-1" data-aos="fade-up" data-aos-delay="200">
          <h1>Productos 100% Boyacenses</h1>
          <p>Apoya a los diferentes microempresarios de nuestra región</p>
          <div class="container">
            <div class="row justify-content-start">
              <div class="col-lg-7">
                <router-link to="/store" href="" class="btn-general">Comprar ahora</router-link>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-6 order-1 order-lg-2 hero-img" data-aos="zoom-in" data-aos-delay="200">
          <img src="../images/campesina.png" class="home-img" alt="Imagen Campesina" @mouseover="zoomIn" @mouseleave="zoomOut">
        </div>
      </div>
    </div>
  </section>

<!--------------------- Productos ---------------------------->
<section class="bg0 p-t-23 p-b140">
  <div class="container">
    <div class="p-b-10">
      <h3 class="ltext-103 cl5">
        Nuestros productos
      </h3>
    </div>

    <div class="flex-w flex-sb-m p-b-52">
      <div class="flex-w flex-l-m filter-tope-group m-tb-10">
        <button class="stext-106 cl6 hov1 bor3 trans-04 m-r-32 m-tb-5 how-active1" data-filter="*">
						Todos los productos
					</button>
      </div>

      <div class="flex-w flex-c-m m-tb-10">
					<div class="flex-c-m stext-106 cl6 size-105 bor4 pointer hov-btn3 trans-04 m-tb-4 js-show-search">
						<i class="ri-search-line cl2 m-r-6 fs-15 trans-04 zmdi zmdi-search"></i>
						<i class="ri-fullscreen-exit-line cl2 m-r-6 fs-15 trans-04 zmdi zmdi-close dis-none"></i>
						Search
					</div>
				</div>

        <!-- Buscar product -->
				<div class="dis-none panel-search w-full p-t-10 p-b-15">
					<div class="bor8 dis-flex p-l-15">
						<button class="size-113 flex-c-m fs-16 cl2 hov-cl1 trans-04">
							<i class="zmdi ri-search-line "></i>
						</button>
						<input class="mtext-107 cl2 size-114 plh2 p-r-15" type="text" name="search-product" placeholder="Search">
					</div>	
				</div>
    </div>


    <div class="row isotope-grid">
      <div class="col-sm-6 col-md-4 col-lg-3 p-b-35 isotope-item">
					<div class="block2">
						<div class="block2-pic hov-img0">
							<img src="../images/img.png" alt="IMG-PRODUCT">

							<a href="#" class="block2-btn flex-c-m stext-103 cl2 size-102 bg0 bor2 hov-btn1 p-lr-15 trans-04 js-show-modal1">
								Ver más
							</a>
						</div>

						<div class="block2-txt flex-w flex-t p-t-14">
							<div class="block2-txt-child1 flex-col-l ">
								<a href="product-detail.html" class="stext-104 cl4 hov-cl1 trans-04 js-name-b2 p-b-6">
									Nombre
								</a>

								<span class="stext-105 cl3">
									$ 1.000
								</span>
							</div>

							<div class="block2-txt-child2 flex-r p-t-3">
								<a href="#" class="btn-addwish-b2 dis-block pos-relative js-addwish-b2">
                  <i class="ri-heart-line dis-block trans-04"></i>
                  <i class="ri-heart-fill trans-04 ab-t-l"></i>
								</a>
							</div>
						</div>
					</div>
				</div>
    </div>
  </div>
</section>

</template>

<script>
export default {
  name: 'HomeView',
  methods: {
    zoomIn(event) {
      event.target.style.transform = 'scale(1.03)';
    },
    zoomOut(event) {
      event.target.style.transform = 'scale(1)';
    },
  },
}

</script>

<style scoped>
a {
  text-decoration: none;
}

#home {
  padding-top: 80px;
  background: var(--primary-color2);
}

#home h1 {
  margin: 0 0 10px 0;
  font-size: 48px;
  font-weight: 700;
  line-height: 56px;
  color: var(--text-color2);
}

#home p {
  font-size: 20px;
  color: var(--text-color2);
}

.hero-img img {
  width: 80%;
  height: auto;
  transition: transform 0.3s ease;
}

@media (max-width: 768px) {
  #home p {
    margin-top: 15px;
    margin-bottom: 30px;
    line-height: 1.2;
  }

  #home h1 {
  font-size: 30px;
  line-height: 1.2;
}

  .btn-general {
    display: flex;
    justify-content: center;
    max-width: 60%;
    margin: 0 auto;
  }

  .hero-img {
    display: flex;
    justify-content: center;
  }
  .hero-img img {
    width: 70%;
  }

}

</style>
