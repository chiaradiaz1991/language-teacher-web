<template>
  <div class="contact-container">
    <h3>{{ $t("main.contact.title") }}</h3>
    <div class="container">
      <p>{{ $t("main.contact.corporate") }}</p>
      <div class="email-linkedin">
        <div class="icon-container">
          <img src="../../assets/mail.png" alt />
          <a href="mailto:gosia.valleau@gmail.com">{{
            $t("main.contact.mail")
          }}</a>
        </div>
        <div class="icon-container">
          <img src="../../assets/linkedIn.png" alt />
          <a href="https://www.linkedin.com/in/ma%C5%82gorzata-vailleau-wo%C5%82czyk-18a3601b4/" target="_blank">{{ $t("main.contact.linkedin") }}</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500;600;700;800;900&display=swap');
.contact-container {
  width: 280px;
  font-family: 'Work Sans', sans-serif;
  color: #325147;
  margin: 40px;
  padding-top: 25px;
}
.icon-container {
  align-items: center;
}
h3 {
  font-size: 20px;
  font-weight: 600;
}
p {
  font-size: 18px;
  /* background-color: #b3847c; */
}
img {
  width: 22px;
  height: 22px;
  margin-right: 10px;
}
a {
  font-size: 18px;
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
.email-linkedin {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}
@media (min-width: 768px) {
  .contact-container {
    padding-top: 0px;
  }
  .container {
    width: 700px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }
  .icon-container {
    margin-right: 50px;
  }
  .email-linkedin {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
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
    font-size: 20px;
  }
  a {
    font-size: 18px;
  }
}
</style>
