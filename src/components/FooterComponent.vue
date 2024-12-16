<script setup>

</script>

<template>
  <footer>
    <div class="footer__tele">
      © Telegraph. 2020 — All rights reserved.
    </div>
    <div class="footer__social">
      <ul>
        <li>Twitter</li>
        <li>Instagram</li>
        <li>Facebook</li>
      </ul>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: space-between;
  padding-top: 81px;
}
.footer__social ul {
  display: flex;
  gap: 50px;
}
.footer__social ul li {
  color: #00194A;
  font-size: 16px;
  font-weight: 500;
  line-height: 18px;
}
.footer__tele{
  color: #00194A;
  font-size: 18px;
  font-weight: 500;
}
</style>