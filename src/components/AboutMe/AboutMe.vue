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
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500;600;700;800;900&display=swap');
.about-me-container {
  width: 280px;
  font-family: 'Work Sans', sans-serif;
  color:#325147;
  margin: 40px;
}
h3 {
  font-size: 20px;
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
    font-size: 20px;
  }
  p {
    font-size: 16px;
    line-height: 27px;
  }
}
</style>