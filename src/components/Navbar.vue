<template>
  <div class="header container-fluid">
      <div class="container">
          <div class="navbar__wrapper d-flex justify-content-between align-items-center">
              <div class="navbar__logo">
                 <router-link to="/" class="logo"><h2>VueFinance</h2></router-link>
              </div>
              <nav class="navbar__items">
                  <ul class="d-flex pt-3 justify-content-between align-items-center">
                      <li><router-link to="/" class="nav__item">Home</router-link></li>    
                      <li><router-link to="/" class="nav__item">About Us</router-link></li>    
                      <li><router-link to="/" class="nav__item">Track your Finances</router-link></li>    
                      <li><router-link to="/" class="nav__item">Invest</router-link></li>    
                      <li><router-link to="/signin" class="nav__item signin">Sign In</router-link></li>    
                      <li><router-link to="/signup" class="nav__item signup">Sign Up</router-link></li>    
                  </ul>
              </nav>
              <div class="navbar__toggler d-none">
                  <i class="fa fa-bars"></i>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
mounted(){
    this.fixNav()
},
 methods:{
        showNav:function(){
            const nav = document.querySelector('.nav__links');
            nav.classList.toggle('show__nav');
        },
        fixNav:function(){
             const nav = document.querySelector('.header');
            window.onscroll = function(){
                if (window.pageYOffset > 120) {
                    nav.classList.add('fix__nav');
                }else{
                    nav.classList.remove('fix__nav');
                }
            }
        },
 },
created(){
    window.onscroll
}
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/colors';
.header{
    background: #fff;
    //Logo
    .logo{
        text-decoration: none;
        // .logo-img{
        //    height: 20px;
        //    font-weight: bold;
        // }
        h2{
            color: $primary-color;
            font-weight: bolder;
            font-size: 1.7rem;
            text-decoration: none;
            padding-top: .7rem;
        }
    }
    //UL
    ul{
        li a{
             color: $primary-color;
             text-transform: capitalize;
             font-weight: bold;
             opacity: .7;
             font-size: 1rem;
             margin: 0 1rem;
             text-decoration: none;
             display: inline-block;
        }
        .signin{
            border: 1px solid $primary-color;
            padding: .6rem 1.7rem;
            border-radius: 3px;
            opacity: 1;
            transition: all ease-in-out .5s;
             &:hover{
                background: $primary-color;
                color:#fff;
            }
        }
         .signup{
            background: $primary-color;
            padding: .6rem 1.7rem;
            border-radius: 3px;
            color: #fff;
            opacity: 1;
            transition: all ease-in-out .5s;
             &:hover{
                background: transparent;
                border: 1px solid $primary-color;
                color: $primary-color;
            }
        }
    }
}

//FIX NAV ON SCROLL
.fix__nav{
    position: fixed;
    top: 0; 
    z-index: 100;
    background: #fff;
    padding: .3rem 0;
    transition: all ease-in-out .5s;
    box-shadow: 0px 0px 5px rgba(0,0,0,0.17);
}
</style>