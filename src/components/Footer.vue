<script>
export default {};
</script>
<template>
  <footer>
    <div class="flex big__box justify-center">
      <div class="box__1">
        <div class="imgDivBox">
          <img src="../img/logo.png" alt="logo__footer" />
        </div>
        <h2>
          Delivering the best coffee life since 1996. From coffee geeks to ones.
        </h2>
        <h1>CoffeeStyle Inc. © 1996</h1>
      </div>
      <div class="box__2">
        <h1>Menu</h1>
        <ul>
          <li><a class="a__1 hover:underline" href="#">Home</a></li>
          <li><a class="a__2 hover:underline" href="#">Our Products</a></li>
          <li><a class="a__3 hover:underline" href="#">About</a></li>
          <li><a class="a__4 hover:underline" href="#">Contact</a></li>
          <li><a class="a__5 hover:underline" href="#">Styleguide</a></li>
        </ul>
      </div>
      <div class="box__3">
        <h1>Follow Us</h1>
        <ul>
          <li><a class="a__11 hover:underline" href="#">Facebook</a></li>
          <li><a class="a__22 hover:underline" href="#">Instagram</a></li>
          <li><a class="a__33 hover:underline" href="#">Pinterest</a></li>
          <li><a class="a__44 hover:underline" href="#">Twitter</a></li>
        </ul>
      </div>
      <div class="box__4">
        <h3>Contact Us</h3>
        <h2>We’re Always Happy to Help</h2>
        <h1>us@coffeestyle.io</h1>
        <h4>Powered by Webflow</h4>
      </div>
    </div>
  </footer>
</template>


<style scoped>
.big__box {
  padding: 100px 250px 59px 250px;
}
.box__1 h2 {
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 22px;
  width: 258px;
  margin-top: 22px;
  color: rgba(29, 31, 46, 0.7);
}
.box__1 h1 {
  margin-top: 80px;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 22px;
  color: rgba(29, 31, 46, 0.3);
}
.box__2 {
  margin-left: 55px;
}
.box__2 h1,
.box__3 h1,
.box__4 h3 {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #1d1f2e;
}
.box__3 {
  margin-left: 79px;
}
.box__2 ul,
.box__3 ul {
  margin-top: 22px;
}
.box__2 ul li a,
.box__3 ul li a {
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 22px;
  color: rgba(29, 31, 46, 0.7);
}
.a__2,
.a__3,
.a__4,
.a__5,
.a__11,
.a__22,
.a__33,
.a__44 {
  margin-top: 10px;
}
.box__4 {
  margin-left: 97px;
}
.box__4 h2 {
  font-style: normal;
  font-weight: 400;
  margin-top: 22px;
  font-size: 14px;
  line-height: 22px;
  color: rgba(29, 31, 46, 0.7);
}
.box__4 h1 {
  margin-top: 16px;
  font-style: normal;
  font-weight: 400;
  font-size: 23px;
  line-height: 36px;
  color: #1d1f2e;
}
.box__4 h4 {
  margin-top: 55px;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 22px;
  color: rgba(29, 31, 46, 0.3);
}

@media (max-width: 1326px) {
  .big__box {
    padding: 130px 100px 59px 130px;
  }
}
@media (max-width: 1146px) {
  .big__box {
    padding: 100px 100px 59px 100px;
  }
}
@media (max-width: 1034px) {
  .box__2 {
    margin-left: 30px;
  }
  .box__3 {
    margin-left: 30px;
  }
  .box__4 {
    margin-left: 50px;
  }
}
@media (max-width: 1034px) {
  .big__box {
    padding: 50px 50px 59px 50px;
  }
}
@media (max-width: 812px) {
  .big__box {
    padding: 50px 20px 59px 20px;
  }
}
@media (max-width: 750px) {
  .big__box {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .box__4,
  .box__3,
  .box__2,
  .box__1 {
    text-align: center;
  }
  .imgDivBox {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .box__1 h1 {
    margin-top: 0px;
  }
  .box__2 {
    margin-top: 10px;
    margin-left: 0px;
  }
  .box__3 {
    margin-top: 10px;
    margin-left: 0px;
  }
  .box__4 {
    margin-top: 10px;
    margin-left: 0px;
  }
  .box__1 h2 {
      margin-top: 10px;
  }
   .box__2 ul,.box__3 ul {
      margin-top: 5px;
  }
  .box__4 h2{
      margin-top: 5px;
  }
  .box__4 h1,.box__4 h4{
      margin-top: 5px;
  }
}
</style>