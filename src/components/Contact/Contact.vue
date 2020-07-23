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
  width: 280px;
  font-family: "futura std";
  color: #325147;
  margin: 40px;
  padding-top: 25px;
}
.icon-container {
  align-items: center;
}
h3 {
  font-size: 25px;
  font-weight: 600;
}
img {
  width: 22px;
  height: 22px;
  margin-right: 10px;
}
a {
  font-size: 26px;
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
@media (min-width: 768px) {
  .contact-container {
    padding-top: 0px;
  }
  .container {
    width: 700px;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
  }
  .icon-container {
    margin-right: 50px;
  }
}

@media (min-width: 1024px) {
  .contact-container {
    width: 600px;
  }
  .container {
    justify-content: space-between;
  }
  h3 {
    font-size: 30px;
  }
  a {
    font-size: 26px;
  }
}
</style>