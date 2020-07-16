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
  width: 400px;
  font-family: 'futura std';
  color:#325147;
}
h3 {
  font-weight: 300;
  font-size: 28px;
}
p {
  font-size: 18px;
}
</style>