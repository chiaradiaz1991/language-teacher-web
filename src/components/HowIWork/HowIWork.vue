<template>
  <div class="how-container">
    <h3>{{ $t("main.howIWork.title") }}</h3>
    <div class="icon-container">
      <div class="icon">
        <img src="../../assets/individual.png" class="img" alt />
        <p>{{ $t("main.howIWork.individual") }}</p>
      </div>
      <div class="icon">
        <img src="../../assets/remote.png" class="img" alt />
        <p>{{ $t("main.howIWork.online") }}</p>
      </div>
      <div class="icon">
        <img src="../../assets/resources.png" class="img" alt />
        <p>{{ $t("main.howIWork.resources") }}</p>
      </div>
      <div class="icon">
        <img src="../../assets/payment.png" class="img" alt />
        <p>{{ $t("main.howIWork.payment") }}</p>
      </div>
      <div class="icon">
        <img src="../../assets/fun.png" class="img" alt />
        <p>{{ $t("main.howIWork.learn") }}</p>
      </div>
      <div class="icon">
        <img src="../../assets/plan.png" class="img" alt />
        <p>{{ $t("main.howIWork.plan") }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500;600;700;800;900&display=swap");
.how-container {
  width: 280px;
  font-family: "Work Sans", sans-serif;
  color: #325147;
  margin: 40px;
  padding-top: 25px;
}
.img {
  width: 45px;
}
h3 {
  font-size: 20px;
  font-weight: 600;
}
.icon {
  text-align: center;
}
p {
  font-size: 16px;
}
@media (min-width: 768px) {
  .how-container {
    padding-top: 0px;
    width: 700px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  p {
    font-size: 16px;
    width: 180px;
  }
  .icon-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .icon {
    margin: 10px;
    align-self: center;
  }
}

@media (min-width: 1024px) {
  .how-container {
    width: 800px;
  }
  h3 {
    font-size: 20px;
  }
}
</style>
