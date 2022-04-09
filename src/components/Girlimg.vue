<script>
export default {
  data() {
    return {
      toggle: false,
    };
  },
  methods: {
    toogleFunction() {
      this.toggle = !this.toggle;
        if(this.toggle){
        document.querySelector("body").style.overflow = "hidden";
      }
        else{
          document.querySelector("body").style.overflow = "initial";
        }
      
    },
    //   countUp: function() {
    
    // }

  
  },
};
</script>
<template>
  <header class="header__w">
    <nav class="flex items-center justify-center nav__content">
      <div class="relative logo__box">
        <img
          class="absolute w-full h-full object-cover"
          src="../img/logo.png"
          alt="logo"
        />
      </div>
      <div class="flex items-center menus__box">
        <ul
          :style="[toggle ? { left: '0' } : { left: '-100%' }]"
          class="flex items-center menus__ul"
        >
          <li>
            <a class="block uppercase hover:underline a__tag__1" href="#"
              >Home</a
            >
          </li>
          <li>
            <a class="block uppercase hover:underline a__tag__2" href="#"
              >Our Products</a
            >
          </li>
          <li>
            <a class="block uppercase hover:underline a__tag__3" href="#"
              >Blog</a
            >
          </li>
          <li>
            <a class="block uppercase hover:underline a__tag__4" href="#"
              >About</a
            >
          </li>
          <li>
            <a class="block uppercase hover:underline a__tag__5" href="#"
              >Contact</a
            >
          </li>
          <li>
            <a class="block uppercase hover:underline a__tag__6" href="#"
              >Styleguide</a
            >
          </li>
        </ul>
        <div class="flex items-center cart__Div">
          <div class="cursor-pointer">
            <img src="../img/beg.png" alt="beg" />
          </div>
          <a href="#" class="block cart__a uppercase hover:underline">Cart</a>
          <div class="cursor-pointer">
            <img src="../img/zero.png" alt="zero" />
          </div>
        </div>
        <div @click="toogleFunction" class="flex items-center burger__box">
          <button v-if="toggle">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
          <button v-else>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
        </div>
      </div>
    </nav>
  </header>
</template>
<style scoped>
@import "../assets/base.css";

.header__w {
  padding: 38px 230px;
  margin: 0 auto;
  font-family: "Karla";
}
.menus__box {
  margin-left: 90px;
}
.menus__ul li a {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 2px;
  color: #1d1f2e;
}
.a__tag__2,
.a__tag__3,
.a__tag__4,
.a__tag__5,
.a__tag__6 {
  margin-left: 30px;
}
.burger__box {
  display: none;
}
.logo__box {
  width: 112px;
  height: 24px;
}
.cart__Div {
  margin-left: 50px;
}
.cart__a {
  padding: 0px 12px;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 2px;
  color: #1d1f2e;
}

@media (max-width: 1340px) {
  .a__tag__2,
  .a__tag__3,
  .a__tag__4,
  .a__tag__5,
  .a__tag__6 {
    margin-left: 20px;
  }
  .menus__box {
    margin-left: 30px;
  }
}
@media (max-width: 1233px) {
  .header__w {
    padding: 30px 180px;
  }
  @media (max-width: 1145px) {
    .header__w {
      padding: 30px 120px;
      margin: 0 auto;
    }
    .menus__box {
      margin-left: 20px;
    }
  }
  @media (max-width: 1017px) {
    .cart__Div {
      margin-left: 30px;
    }
  }
  @media (max-width: 996px) {
    .cart__a {
      padding: 0px 10px;
      font-size: 10px;
      line-height: 15px;
      letter-spacing: 1px;
    }
    .menus__ul li a {
      font-size: 10px;
      line-height: 15px;
      letter-spacing: 1px;
    }
  }
  @media (max-width: 916px) {
    .header__w {
      padding: 20px 70px;
      margin: 0 auto;
    }
  }
  @media (max-width: 780px) {
    .nav__content {
      justify-content: space-between;
    }
    .burger__box {
      display: block;
      display: flex;
      z-index: 20;
      justify-content: center;
      align-items: center;
    }
    .logo__box {
      z-index: 20;
    }
    .header__w {
      padding: 15px 20px;
      margin: 0 auto;
    }
    .menus__ul {
      position: fixed;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: #efa145ff;
      width: 100%;
      height: 100%;
      z-index: 18;
      top: 0;
      left: -100%;
      transition: 0.2s ease;
    }
    .a__tag__2,
    .a__tag__3,
    .a__tag__4,
    .a__tag__5,
    .a__tag__6 {
      margin-top: 10px;
      margin-left: 0px;
    }
    .menus__ul li a {
      font-size: 12px;
      line-height: 18px;
      letter-spacing: 2px;
      text-align: center;
    }
    .cart__Div {
      display: none;
    }
  }
}
</style>