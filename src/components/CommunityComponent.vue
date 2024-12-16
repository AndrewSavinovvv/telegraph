<script setup>
import img from "@/assets/img/icon.png";
</script>

<template>
  <div class="community">
    <div class="community__left">
      <h1>Sharing Cool Stuff With Your <br> Community</h1>
      <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour</p>
      <p>
        If you are going to use a passage of Lorem Ipsum, you <br> need to be sure there isn't anything.
      </p>
    </div>
    <div class="community__right">
      <div class="community__item">
        <img :src="img" alt="Security by Default" />
        <h4>Security by Default</h4>
        <p class="community_item__p">It is a long established fact that a reader will be distracted by the readable content.</p>
      </div>
      <div class="community__item">
        <img :src="img" alt="Security by Default" />
        <h4>Security by Default</h4>
        <p class="community_item__p">It is a long established fact that a reader will be distracted by the readable content.</p>
      </div>
      <div class="community__item community__item--right">
        <img :src="img" alt="Security by Default" />
        <h4>Security by Default</h4>
        <p class="community_item__p">It is a long established fact that a reader will be distracted by the readable content.</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.community {
  display: flex;
  align-items: center;
  gap: 111px;
}

.community__left {
  width: 40%;
}

.community__right {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.community__item {
  width: 260px;
  height: 249px;
  box-shadow: 0 0 25px 0 rgba(0, 0, 0, 0.03);
  padding: 20px 30px;
}

.community__item img {
  margin-bottom: 30px;
}

.community__item h4 {
  margin-bottom: 15px;
}

.community_item__p {
  opacity: 80%;
  color: #00194A;
  font-size: 14px;
  line-height: 26px;
  font-weight: 300;
}
.community__right {
  position: relative;
}
 .community__right .community__item--right {
  align-self: center;
  position: absolute;
  top: 175px;
  right: -340px;
   width: 260px;
   height: 249px;
}

.community h4 {
  color: #00194A;
  font-weight: 500;
  font-size: 18px;
  line-height: 21px;
  margin-top: 20px;
}

.community__left h1 {
  color: #00194A;
  font-weight: 500;
  font-size: 35px;
  margin-bottom: 30px;
}

.community__left p {
  color: #00194A;
  font-size: 18px;
  font-weight: 300;
  margin-bottom: 30px;
}
</style>