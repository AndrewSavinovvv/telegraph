<script setup>
import { defineProps } from 'vue';

defineProps({
  title: {
    type: String,
    required: true
  },
  text: {
    type: String,
    required: true
  },
  count: {
    type: Number,
    required: true
  }
});
</script>

<template>
  <div class="message">
    <img class="message__image" src="@/assets/img/profile.png" alt="Profile">
    <div class="message__content">
      <div class="message__header">
        <h1 class="message__title">{{ title }}</h1>
        <div class="message__header-time">11:39 PM</div>
      </div>
      <div class="message__footer">
        <p class="message__text">{{ text }}</p>
        <p v-if="count" class="message__count">{{ count }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.message {
  position: relative;
  top: -220px;
  left: 128px;
  display: flex;
  padding: 10px;
  border-radius: 10px;
  width: 391px;
  height: 80px;
  gap: 0 !important;
  padding-top: 0 !important;
  background: white;
  margin-bottom: 15px;
}

.message__image {
  width: 60px;
  height: 60px;
  margin-right: 15px;
}


.message__content {
  display: flex;
  flex-direction: column;
  flex: 1;
}


.message__header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 8px;
}


.message__footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}


.message__title {
  font-size: 18px;
  font-weight: 500;
  color: #00194A;
}


.message__header-time {
  color: #00194A;
  font-weight: 300;
  font-size: 14px;
}


.message__text {
  font-size: 14px;
  font-weight: 300;
  color: #00194A;
  margin-top: 5px;
}


.message__count {
  font-size: 12px;
  font-weight: 500;
  color: white;
  border-radius: 8px;
  padding: 5px;
  background: #FF0043;
}

</style>