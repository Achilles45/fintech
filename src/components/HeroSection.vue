<template>
  <div class="hero__section">
      <div class="hero__contents container">
          <div class="row">
              <div class="col-md-6 text">
                  <h1>Invest. Budget. Learn</h1>
                  <p>VueFinance helps you access different safe and high yielding investment vehicles, make better investment decisions and track your finances.</p>
                  <router-link to="/sds" class="hero__btn">Get Started  <i class="fas fa-long-arrow-alt-right 7x"></i></router-link>
              </div>
              <div class="col-md-6">
                  <img src="../assets/image/img2.svg" class="img-fluid" alt="">
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
.hero__section{
    margin-top: 10rem;
    .text{
        h1{
            font-weight: 900;
            color:$primary-color;
            padding-bottom: 1rem;
            font-size: 2.9rem;
        }
        p{
            color: $primary-color;
            font-weight: 400;
            line-height: 1.6;
            font-size: 1.03rem;
            opacity: .7;
            padding-bottom: 1.7rem;
        }
        .hero__btn{
            background: $primary-color;
            color:#fff;
            text-decoration: none;
            padding: 1.2rem 3.9rem;
            border-radius: 4px;
            transition: all ease-in-out .5s;
            &:hover{
                padding: 1.2rem 4rem;
            }
            .fa-long-arrow-alt-right{
                animation-name: animate;
                animation-duration: 3s;
                animation-iteration-count: infinite;
                animation-direction: alternate;
            }
        }
    }
}

//Animation for button arrow
@keyframes animate {
    from{
        opacity: 0;
    }
    to{
        transform: translateX(30px);
        opacity: 1;
    }
}
</style>