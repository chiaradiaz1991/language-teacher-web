<template>
  <div class="languages-container">
    <h3>{{ $t('main.languages.title') }}</h3>
    <div class="lang-main-container">
      <div class="lang-container">
        <p>{{ $t('main.languages.pl') }}</p>
        <img src="../../assets/pl.png" alt />
      </div>
      <div class="lang-container">
        <p>{{ $t('main.languages.en') }}</p>
        <img src="../../assets/en.png" alt />
      </div>
      <div class="lang-container">
        <p>{{ $t('main.languages.de') }}</p>
        <img src="../../assets/de.png" alt />
      </div>
      <div class="lang-container">
        <p>{{ $t('main.languages.fr') }}</p>
        <img src="../../assets/fr.png" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.languages-container {
  width: 300px;
  font-family: "futura std";
  color: #325147;
  margin-bottom: 30px;
}
h3 {
  font-weight: 500;
  font-size: 28px;
}
img {
  width: 50px;
  margin: auto;
}
.lang-main-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 300px;
}
.lang-container {
  display: flex;
  flex-direction: column;
}
p {
  font-size: 18px;
}

@media (max-width: 425px) {
.languages-container {
    width: 300px;
  }
  h3 {
  font-size: 24px;
  }
  p {
    font-size: 16px;
    text-align: center;
  }
  .lang-main-container {
    display: flex;
    flex-wrap: wrap;
  }
  .lang-container {
    margin-right: 20px;
  }
}
@media (max-width: 1024px) {
  .lang-main-container {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>