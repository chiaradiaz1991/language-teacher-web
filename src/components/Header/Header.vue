<template>
  <div class="header-container">
    <img src="../../assets/photo.png" alt="" class="header-image"/>
    <p>{{ $t('main.header') }}</p>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
.header-container {
  display: flex;
  flex-direction: column;
}
.header-image {
  width: 180px;
  margin: auto;
  margin-top: 60px;
  margin-bottom: 30px;
}
p {
  font-family: 'futura std';
  font-weight: 100;
  background-color: #EED7CE;
  width: 300px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #B3847C;
  font-size: 26px;
  margin: auto;
  padding: 3px;
}
/* @media (max-width: 425px) {
  .header-image {
    width: 300px;
  }
} */
</style>