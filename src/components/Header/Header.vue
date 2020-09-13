<template>
  <div class="header-container">
    <img src="../../assets/gosia-profile.png" alt="" class="header-image"/>
    <p>{{ $t('main.header') }}</p>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500;600;700;800;900&display=swap');
.header-container {
  display: flex;
  flex-direction: column;
}
.header-image {
  width: 180px;
  margin: auto;
  margin-top: 60px;
  margin-bottom: 30px;
  border-radius: 50%;
}
p {
  font-family: 'Work Sans', sans-serif;
  font-weight: 300;
  background-color: #EED7CE;
  min-width: 300px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #B3847C;
  font-size: 18px;
  margin: auto;
  padding: 3px;
}
@media (min-width: 768px) {
  p {
    font-size: 26px;
  }
}
@media (min-width: 1024px) {
  .header-image {
    width: 220px;
  }
}
</style>