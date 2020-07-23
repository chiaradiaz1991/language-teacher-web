<template>
  <div class="how-container">
    <h3>{{$t('main.howIWork.title')}}</h3>
    <div class="icon-container">
      <div class="icon">
        <img src="../../assets/individual.png" class="img" alt />
        <p>{{ $t('main.howIWork.individual')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/remote.png" class="img" alt />
        <p>{{ $t('main.howIWork.online')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/resources.png" class="img" alt />
        <p>{{ $t('main.howIWork.resources')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/plan.png" class="img" alt />
        <p>{{ $t('main.howIWork.plan')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/fun.png" class="img" alt />
        <p>{{ $t('main.howIWork.learn')}}</p>
      </div>
      <div class="icon">
        <img src="../../assets/payment.png" class="img" alt />
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
  width: 280px;
  font-family: 'futura std';
  color:#325147;
  margin: 40px;
  padding-top: 25px;
}
.img {
  width: 45px;
}
h3 {
  font-size: 25px;
  font-weight: 600;
}
.icon {
  text-align: center;
}
p{
  font-size: 20px;
}
</style>