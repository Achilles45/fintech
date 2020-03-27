<template>
  <div class="partners">
      <div class="container">
          <div class="row">
              <div class="col-12 text-center">
                  <h2>Companies in partnerhip with VueFinance</h2>
                  <p>A few trusted brands we work with</p>
                   <div class="image__holder pt-5">
                  <img src="../assets/image/flutterwave.png" class="img-fluid img" alt="">
                  <img src="../assets/image/paystack.png" class="img-fluid img" alt="">
                  <img src="../assets/image/mastercard.png" class="img-fluid img" alt="">
                  <img src="../assets/image/visa.png" class="img-fluid img" alt="">
                  <img src="../assets/image/verve.png" class="img-fluid img" alt="">
              </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/styles/colors';
.partners{
    padding: 4rem 0;
    h2{
        font-weight: 900;
        color:#00093a;
    }
    p{
        color:#1f2441;
        opacity: .7;
        font-size: 1.1rem;
    }
    .image__holder{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
        grid-gap: 2rem;
        text-align: center;
        margin-bottom: 4rem;
        .img{
            cursor: pointer;
        }
    }
}
</style>