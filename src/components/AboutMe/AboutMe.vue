<template>
  <div class="about-me-container">
    <h3>{{$t('main.aboutMe.title')}}</h3>
    <p>{{ $t('main.aboutMe.description') }}</p>
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.about-me-container {
  width: 300px;
  font-family: 'futura std';
  color:#325147;
}
h3 {
  font-weight: 500;
  font-size: 28px;
}
p {
  font-size: 18px;
}
@media (max-width: 425px) {
  .about-me-container {
    width: 300px;
  }
  .header-image {
    width: 300px;
  }
  h3 {
    font-size: 24px;
  }
  p {
    font-size: 16px;
  }
}
@media (max-width: 1024px) {
  .about-me-container {
    width: 300px;
  }
}
</style>