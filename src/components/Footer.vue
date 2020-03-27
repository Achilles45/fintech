<template>
  <footer>
      <div class="container">
          <div class="row">
              <div class="col-md-3">
                  <h6 class="head">Company</h6>
                  <ul>
                      <li><router-link to="/about">About</router-link></li>
                      <li><router-link to="/">Blog</router-link></li>
                      <li><router-link to="/">Testimonials</router-link></li>
                      <li><router-link to="/">FAQs</router-link></li>
                  </ul>
              </div>
               <div class="col-md-3">
                  <h6 class="head">Features</h6>
                  <ul>
                      <li><router-link to="/">Investments</router-link></li>
                      <li><router-link to="/">Data Analysis</router-link></li>
                      <li><router-link to="/">Budgeting</router-link></li>
                  </ul>
              </div>
              <div class="col-md-3">
                  <h6 class="head">Legal</h6>
                  <ul>
                      <li><router-link to="/">Privacy Policy</router-link></li>
                      <li><router-link to="/">Terms & Conditions</router-link></li>
                  </ul>
              </div>
              <div class="col-md-3">
                  <h6 class="head">Contact Info</h6>
                  <div class="details">
                      <div class="first d-flex">
                          <i class="fa fa-map-marker"></i>
                          <div class="content">
                              <p class="pl-4">1 Jinojah Street, Off Peter Okoro Street Along Owhelogbo Road, Ozoro, Delta State, Nigeria</p>
                          </div>
                      </div>
                      <div class="first d-flex">
                          <i class="fa fa-envelope"></i>
                          <div class="content">
                              <p class="pl-4">hello@vuefinance.com</p>
                          </div>
                      </div>
                       <div class="first d-flex">
                          <i class="fa fa-phone"></i>
                          <div class="content">
                              <p class="pl-4">+234-8103-515-205</p>
                          </div>
                      </div>
                  </div>
              </div>
          </div><br>
          <hr>
          <div class="row">
              <div class="footer__bottom">
              <div class="col-12">
                  <small>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, repellendus debitis. Sunt quaerat, molestias ducimus totam, fugiat hic pariatur natus modi dolorem, aperiam voluptate sed doloremque repudiandae recusandae assumenda consequuntur saepe labore laudantium deleniti dolore reprehenderit porro impedit ut. Numquam veritatis totam quae eum repudiandae, vero ex doloremque explicabo dignissimos fugiat exercitationem sunt officiis ab, libero fuga sequi in ut? Quidem optio exercitationem sapiente quod dicta impedit ratione quisquam eligendi? Dolorum explicabo ut iure corporis voluptate! Quae laborum illum ad quidem facilis fugiat assumenda? Dolorum officia delectus saepe, laboriosam temporibus perspiciatis sunt omnis</small><br>
              </div><br>
              <div class="col-12 text-center">
                  <small class="copy">Copyright &copy;2020 All rights reserved. VueFinance. RC:12121</small>
              </div>
          </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/styles/colors';
footer{
    background: #f8f9fc;
    padding: 5rem 0;
    .head{
        color:#00093a;
        font-weight: 900;
        text-transform: uppercase;
        font-size: .9rem;
        padding-bottom: 1rem;
    }
    ul{
        li a{
            line-height: 2.7;
            color: #00093a;
            opacity: .6;
            font-weight: 400;
            font-size: 1.02rem;
        }
    }
    p{
        color:#00093a;
        opacity: .6;
        font-weight: 400;
        font-size: 1.02rem;
    }
    .fa-envelope, .fa-phone, .fa-map-marker{
        color:#00093a;
        opacity: .6;
        font-weight: bold;
    }
    .footer__bottom{
        small{
            color: #00093a;
            opacity: .5;
        }
        .copy{
            text-align: center !important;
        }
    }
}
</style>