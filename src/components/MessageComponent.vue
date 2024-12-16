<script setup>
import MessagesComponent from "@/components/MessagesComponent.vue";

const messages = [
  {
    title: "Wife",
    text: "It is a long established fact that a…",
    count: 10
  },
  {
    title: "Girlfriend",
    text: "It is a long established fact that a…",

  },
  {
    title: "Unknown Girl",
    text: "It is a long established fact that a…",
  }
];
</script>

<template>
  <div class="message">
    <div class="message__left">
      <img src="@/assets/img/hlopec.png" alt="">
    </div>
    <div class="message__right">
      <h1>Simple, Personal, Real Time Messaging</h1>
      <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
      <p> If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything.</p>
    </div>
  </div>
  <MessagesComponent
      v-for="(msg, index) in messages"
      :key="index"
      :title="msg.title"
      :text="msg.text"
      :class="{
    'message--second': index === 1,
    'message--third': index === 2
  }"
      :count="index === 0 ? msg.count : null"
      :style="{ marginLeft: `${index === 1 ? 30 : index === 2 ? 50 : 0}px` }"
  />
</template>

<style scoped>
.message {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 222px;
  padding-top: 165px;
}
.message__right h1 {
  color: #00194A;
  font-weight: 500;
  font-size: 35px;
  line-height: 50px;
}
.message__right p {
  color: #00194A;
  font-weight: 300;
  font-size: 18px;
  line-height: 28px;
  margin-top: 30px;
}

.message__left {
  position: relative;
}
.message__left:after {
  content: "";
  background: url(@/assets/img/Oval.png) no-repeat center/cover;
  position: absolute;
  top: -90px;
  left: -110px;
  width: 249px;
  height: 249px;
  z-index: -1;
}
</style>