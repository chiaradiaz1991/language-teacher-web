<template>
  <div class="languages-container">
    <h3>{{ $t('main.languages.title') }}</h3>
    <div class="lang-main-container">
      <div class="lang-container">
        <img src="../../assets/pl.png" alt />
        <div class="bar">100%</div>
      </div>
      <div class="lang-container">
        <img src="../../assets/de.png" alt />
        <div class="bar">100%</div>
      </div>
      <div class="lang-container">
        <img src="../../assets/en.png" alt />
        <div class="bar" id="en">80%</div>
      </div>
      <div class="lang-container">
        <img src="../../assets/fr.png" alt />
        <div class="bar" id="fr">60%</div>
      </div>
            <div class="lang-container">
        <img src="../../assets/es.png" alt />
        <div class="bar" id="es">50%</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500;600;700;800;900&display=swap');
.languages-container {
  width: 280px;
  font-family: 'Work Sans', sans-serif;
  color: #325147;
  margin: 40px;
}
.lang-container {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}
h3 {
  font-size: 20px;
  font-weight: 600;
}
p {
  font-size: 16px;
}
img {
  width: 40px;
  height: 40px;
  box-shadow: 0px 4px 10px rgba(116, 78, 153, 0.2);
  border-radius: 50%;

}
.bar {
  width: 90%;
  padding-top: 3px;
  padding-bottom: 3px;
  color: #B3847C;
  font-size: 16px;
  font-weight: 600;
  text-align: center;
  background-color: #EED7CE;
  margin-left: 20px;
  animation: progressBarPlDe 3s ease-in-out;
  animation-fill-mode:both; 
}
#en {
  width: 70%;
  animation: progressBarEn 3s ease-in-out;
  animation-fill-mode:both; 
}
#fr {
  width: 50%;
  animation: progressBarFr 3s ease-in-out;
  animation-fill-mode:both; 
}
#es {
  width: 40%;
  animation: progressBarEs 3s ease-in-out;
  animation-fill-mode:both; 
}

@keyframes progressBarPlDe {
  0% { width: 0; }
  100% { width: 100%; }
}
@keyframes progressBarEn {
  0% { width: 0; }
  100% { width: 70%; }
}
@keyframes progressBarFr {
  0% { width: 0; }
  100% { width: 60%; }
}
@keyframes progressBarEs {
  0% { width: 0; }
  100% { width: 50%; }
}
@media (min-width: 1024px) {
  h3 {
    font-size: 20px;
  }
}
</style>