<script setup>
import arrowIcon from '@/assets/svg/arrow.svg'
import downloadIcon from '@/assets/svg/download.svg'
const sendEmail = () => {
  window.location.href = 'mailto:ejazulhaq8281@gmail.com'
}
</script>

<template>
  <div class="header__rightnav">
    <button @click="sendEmail" class="btn-green"><arrowIcon />{{ $t('header.button.btn1') }}</button>
    <router-link to="/cv">
      <button class="btn-blue"><downloadIcon />{{ $t('header.button.btn2') }}</button>
    </router-link>
  </div>
</template>

<style scoped>
.header__rightnav {
  display: flex;
  flex-direction: column;
  gap: 12px;
}
a {
  width: 100%;
}
a:hover {
  text-decoration: none;
}

@media (max-width: 768px) {
  .header__rightnav {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>
