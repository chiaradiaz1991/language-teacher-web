<template>
  <div class="contact-container">
    <h3>{{ $t('main.contact.title')}}</h3>
    <div class="container">
      <div class="icon-container">
        <img src="../../assets/mail.png" alt />
        <a href="mailto:chiara.diaz1991@gmail.com">{{$t('main.contact.mail')}}</a>
      </div>
      <div class="icon-container">
        <img src="../../assets/linkedIn.png" alt />
        <a href="#" target="_blank">{{$t('main.contact.linkedin')}}</a>
      </div>
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
  font-weight: 500;
  font-size: 28px;
}
.container {
  display: flex;
  flex-direction: column;
}
a {
  font-size: 20px;
  text-decoration: none;
  color: #325147;
  align-self: center;
}
a:visited {
  color: #325147;
}
a:hover {
  color: #b3847c;
}
a:active {
  color: #325147;
}
.icon-container {
  display: flex;
  flex-direction: row;
  margin-bottom: 15px;
}
img {
  width: 25px;
  height: 25px;
  margin-right: 10px;
}

@media (max-width: 425px) {
.contact-container {
    width: 300px;
  }
  h3 {
  font-size: 24px;
  }
}
@media (max-width: 1024px) {
  .contact-container {
    width: 300px;
  }
}
</style>