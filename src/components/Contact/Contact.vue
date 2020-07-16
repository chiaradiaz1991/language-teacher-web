<template>
  <div class="contact-container">
    <h3>{{ $t('main.contact.title')}}</h3>
    <div class="container">
      <a href="mailto:chiara.diaz1991@gmail.com">{{$t('main.contact.mail')}}</a>
      <a href="#" target="_blank">{{$t('main.contact.linkedin')}}</a>
    </div>
  </div>
</template>

<style scoped>
.contact-container {
  width: 400px;
  font-family: "futura std";
  color: #325147;
}
h3 {
  font-weight: 300;
  font-size: 28px;
} 
.container {
  display: flex;
  flex-direction: column;
}
a {
  font-size: 18px;
  text-decoration: none;
  color: #325147;
  margin-top: 15px;
}
a:visited {
  color: #325147;
}
a:hover {
  color: #B3847C;
}
a:active {
  color: #325147;
}
</style>