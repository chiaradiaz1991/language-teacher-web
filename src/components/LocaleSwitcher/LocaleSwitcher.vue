<template>
  <div role="main" class="main-container">
    <div class="container-locale">
    <button v-for="locale in locales" :key="locale" @click="switchLocale(locale)" class="locale">{{ locale }}</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "LocaleSwitcher",
  methods: {
    switchLocale(locale) {
      if (this.$i18n.locale !== locale) {
        this.$i18n.locale = locale;
      }
    }
  },
  data() {
    return {
      locales: process.env.VUE_APP_I18N_SUPPORTED_LOCALE.split(",")
    };
  }
};
</script>

<style scoped>
.main-container {
  padding: 30px;
}
.container-locale {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
}
.locale {
  width: 40px;
  height: 40px;
  border: none;
  font-size: 25;
  cursor: pointer;
  margin-right: 20px;
  color: #325147;
  background-color: transparent;
  outline: none;
  font-size: 18px;
  font-family: 'futura std';
}
.locale:hover {
    background-color: #EED7CE;
    transition: 0.5s;
}
@media (max-width: 425px) {
  .container-locale{
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
}
</style>