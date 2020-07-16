<template>
  <div class="how-container">
    <h3>{{$t('main.howIWork.title')}}</h3>
    <div class="icon-container">
      <div class="icon">
        <img src="../../assets/remote.png" alt />
        <p>{{ $t('main.howIWork.individual')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/remote.png" alt />
        <p>{{ $t('main.howIWork.online')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/fun.png" alt />
        <p>{{ $t('main.howIWork.learn')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/hour.png" alt />
        <p>{{ $t('main.howIWork.hours')}}</p>
      </div>
      <div class="icon-last">
        <img src="../../assets/payment.png" alt />
        <p>{{ $t('main.howIWork.payment')}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.how-container {
  width: 400px;
  font-family: "futura std";
  color: #325147;
}
.icon-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.icon {
  text-align: center;
  margin-bottom: 15px;
}
.icon-last {
  text-align: center;
  margin-bottom: 15px;
  margin: auto;
}
h3 {
  font-weight: 500;
  font-size: 28px;
}

@media (max-width: 425px) {
  .how-container {
    width: 300px;
  }
  .icon-container {
    display: flex;
    flex-direction: column;
  }
    h3 {
    font-size: 24px;
  }
  p {
    font-size: 16px;
  }
}
@media (max-width: 1024px) {
  .how-container {
    width: 300px;
  }
  .icon-container {
    display: flex;
    flex-direction: column;
  }
  /* .icon {
  text-align: left;
  } */
}
</style>