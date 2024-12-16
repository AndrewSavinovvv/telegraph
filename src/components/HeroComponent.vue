<script setup>

</script>

<template>
  <div class="hero">
    <div class="hero__left">
      <h1>Simple. Secure.
        Reliable messaging.</h1>
      <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum.</p>
      <button></button>
    </div>
    <div class="hero__right">
      <img src="@/assets/img/Group%206.png" alt="">
    </div>
  </div>
</template>

<style scoped>
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.hero__left h1 {
  color: #00194A;
  font-weight: 500;
  font-size: 60px;
  line-height: 85px;
}
.hero__left {
  width: 50%;
}
.hero__left p {
  color:#00194A ;
  font-size: 18px;
  line-height: 28px;
  font-weight: 300;
}
.hero__left button {
  background: #FF0043;
  width: 275px;
  height: 60px;
  border: none;
  border-radius: 30px;
  margin-top: 50px;
}
.hero__right{
  width: 50%;
}
</style>