<template>
  <div class="about-me-container">
    <h3>{{$t('main.aboutMe.title')}}</h3>
    <p>{{ $t('main.aboutMe.description.paragraph-a') }}</p>
    <br/>
    <p>{{ $t('main.aboutMe.description.paragraph-b') }}</p>
    <br/>
    <p>{{ $t('main.aboutMe.description.paragraph-c') }}</p>
    <br/>
    <p>{{ $t('main.aboutMe.description.paragraph-d') }}</p>
    <br/>
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.about-me-container {
  width: 280px;
  font-family: 'futura std';
  color:#325147;
  margin: 40px;
}
h3 {
  font-size: 22px;
  font-weight: 600;
}
p{
  font-size: 16px;
}
@media (min-width: 768px) {
  br {
    display: none;
  }
  p {
    font-size: 16px;
  }
}
@media (min-width: 1024px) {
  .about-me-container {
    width: 400px;
  }
  h3 {
    font-size: 22px;
  }
  p {
    font-size: 16px;
    line-height: 27px;
  }
}
</style>