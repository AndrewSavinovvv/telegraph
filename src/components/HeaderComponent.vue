<script setup>

</script>

<template>
  <header>
    <div class="logo">
      Telegraph
    </div>
    <button class="logo__btn">
      Try Beta
    </button>
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  padding-top: 50px;
}
.logo {
  color: #FF0043;
  font-size:20px;
  font-weight: 700;
  line-height:23px;
}
.logo__btn {
  background: #FF0043;
  border: none;
  color: white;
  padding: 15px 20px;
  border-radius: 23px;
  cursor: pointer;
}
</style>