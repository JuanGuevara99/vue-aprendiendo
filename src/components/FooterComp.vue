<template>
<!-- ============================================= -->
<!-- FOOTER -->
<!-- ============================================= -->
<footer>
    <div class="footer">
        <div class="container">
            <div class="row">
                <div class=" col-md-10 offset-md-1">
                    <ul class="conta">
                        <li><i class="ri-map-pin-2-line"></i> Tunja - Boyacá
                        </li>
                        <li><i class="ri-phone-line"></i> +57 3001948159</li>
                        <li><i class="ri-mail-send-line"></i><a> parasumerceboyaca@outlook.com</a></li>
                    </ul>
                </div>
                <div class="col-md-12">
                    <ul class="social_icon">
                        <li><a href="https://www.facebook.com/parasumerceboyaca"><i class="ri-facebook-circle-fill"></i></a></li>
                        <li><a href="https://www.instagram.com/parasumerceboyaca/"><i class="ri-instagram-line"></i></a></li>
                        <li><a href="https://www.linkedin.com/company/parasumerceboyaca/?viewAsMember=true"><i class="ri-linkedin-fill"></i></a></li>
                        <li><a href="https://wa.link/6axt2l"><i class="ri-whatsapp-line"></i></a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="copyright">
            <div class="container">
                <div class="row">
                    <div class="col-md-10 offset-md-1">
                        <p>Copyright 2024 All Right Reserved By <a href="#"> Para Sumercé</a></p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {}
</script>



<style scoped>
a {
  text-decoration: none;
}



.footer {
  background: #1e1a15;
  padding-top: 90px;
  text-align: center;
}

ul.conta {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

ul.conta li {
  color: #fff;
  text-align: left;
  padding-bottom: 20px;
  font-size: 18px;
  display: inline-flex;
  line-height: 30px;
}

ul.conta li:last-child {
  padding-right: 0;
}

ul.conta li i {
  padding-right: 15px;
  text-align: center;
  font-size: 33px;
  color: #fff;
}

ul.conta li a {
  color: #fff;
}

ul.social_icon {
  text-align: center;
}

.social_icon li {
  margin-right: 15px !important;
}

ul.social_icon li {
  display: inline-block;
  margin: 0 2px;
}

ul.social_icon li a i {
  background: #fff;
  width: 32px;
  height: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
  border-radius: 20px;
  color: #212120;
  transition: ease-in all 0.5s;
}

ul.social_icon li a i:hover {
  color: #EB9938;
  background: #fff;
  transition: ease-in all 0.5s;
}

.copyright {
  margin-top: 35px;
  padding-bottom: 25px;
}

.copyright p {
  border-top: #909090 solid 1px;
  color: #fff;
  font-size: 17px;
  line-height: 22px;
  text-align: center;
  padding-top: 25px;
  font-weight: normal;
}

.copyright a {
  color: #fff;
}

.copyright a:hover {
  color: #EB9938;
}

/* ====================================== */
/* MEDIA QUERIES PANTALLA PEQUEÑA */
/* ====================================== */
@media (max-width: 768px) {
  /* Footer */
  .footer {
    padding-left: 15px;
    padding-right: 15px;
  }
}
</style>
