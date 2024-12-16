<script setup>
import img from "@/assets/icon/icon.png"
import icon from "@/assets/icon/download.svg"

const platforms = [
  {
    name: "Android",
    description: "Lorem Ipsum is simply dummy text of the printing and typesetting.",
    image: img,
    footerText: "Try Beta For Free",
    footerIcon: icon
  },
  {
    name: "iOS",
    description: "Lorem Ipsum is simply dummy text of the printing and typesetting.",
    image: img,
    footerText: "Try Beta For Free",
    footerIcon: icon
  },
  {
    name: "Mac or Windows",
    description: "Lorem Ipsum is simply dummy text of the printing and typesetting.",
    image: img,
    footerText: "Try Beta For Free",
    footerIcon: icon
  }
];
</script>

<template>
  <div class="platform">
    <div class="platform__list">
      <div class="platform__item" v-for="(platform, index) in platforms" :key="index">
        <img :src="platform.image" :alt="platform.name" />
        <h4>{{ platform.name }}</h4>
        <p>{{ platform.description }}</p>
        <div class="platform__item__footer">
          <p>{{ platform.footerText }}</p>
          <img :src="platform.footerIcon" alt="Download" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.platform{
  padding-top: 80px;
}
.platform__list {
  display: flex;
  gap: 30px;
}
.platform__item {
  width: 360px;
  height: 272px;
  box-shadow: 0 0 25px 0 rgba(0, 0, 0, 0.03);
  padding: 30px;
}
.platform__item__footer {
  display: flex;
  justify-content: space-between;
}
.platform__item p {
  opacity: 80%;
  color: #00194A;
  font-size: 16px;
  line-height: 26px;
  font-weight: 300;
}
.platform__item__footer p {
  color: #00194A;
  font-weight: 400;
  font-size: 16px;
  line-height: 18px;
  text-decoration: underline;
  opacity: 49%;
  margin-bottom: 20px;
}
.platform__item h4 {
  color: #00194A;
  font-weight: 500;
  font-size: 22px;
  line-height: 26px;
  margin-top: 20px;
}
</style>