<template>
  <div class="container">
    <div class="main-picture">
      <img src="@/assets/images/main.png" />
    </div>
    <div class="main-info">
      <div class="main-info-title">
        <br>
        <p>왕종원 ♥ 김지예</p>
      </div>
      <div class="main-info-location">
        <p>2023년 1월 14일 토요일 12시</p>
        <p>웨딩바이이명원</p>
      </div>
      <div class="divide-line"></div>
      <div class="main-greeting">
        <div class="main-greeting-title">
          <p>왕대환 ∙ 김정국의 <span>장남</span> 종원</p>
          <p>김동식 ∙ 송미숙의 <span>차녀</span> 지예</p>
          <p>결혼합니다</p>
        </div>
        <div class="main-greeting-text">
          <p>함께 있을 때 가장 나다운 모습이 되고</p>
          <p>함께 있을 때 미래를 꿈꾸게 하는 사람을 만났습니다</p>
          <br>
          <p>그 사람과 같은 곳을 바라보며</p>
          <p>평생 함께 걷고자 합니다</p>
          <br>
          <p>저희 두 사람의 첫걸음에 함께 하시어</p>
          <p>축복해 주시면 감사하겠습니다</p>
        </div>
      </div>
      <div class="divide-line"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container{
  max-width:768px;
  margin:0 auto;
  width:96%;
}
.main-picture {
  display: flex;
  align-items: center;
  justify-content: center;
}
.main-picture img {
  width: 100%;
}
.main-info {
  width: 100%;
}
.main-info-title p {
  justify-content: center;
  align-items: center;
  display: flex;
  font-size: 2rem;
  letter-spacing: 0.8rem;
  font-weight: bold;
}
.main-info-location p {
  font-size: 1.5rem;
  text-align: center;
  margin: 0;
}
.divide-line {
  margin: 3rem 3rem;
  border: 0.7px solid rgb(218, 218, 218);
}
.main-greeting {
  margin: 0 auto;
  padding: 0 2.3rem;
}
.main-greeting-title {
  padding-bottom: 4rem;
}
.main-greeting-title p {
  letter-spacing: 0.3rem;
  font-size: 1.5rem;
  margin: 0.4rem 0;
  text-align: center;
}
.main-greeting-title p span {
  font-size: 1.2rem;
}
.main-greeting-text p {
  font-size: 1.25rem;
  margin-top: 0.5rem;
  padding: 0.2rem 0;
  letter-spacing: -0.025rem;
  text-align: center;
}
.main-greeting-text {
  margin-bottom: 3rem;
}
@media (min-width: 350px) {
  .main-info-location p {
    font-size: 1.7rem;
  }
  .main-greeting-title {
    padding-bottom: 4rem;
  }
  .main-greeting-title p span {
    font-size: 1.4rem;
  }
  .main-greeting-title p {
    font-size: 1.7rem;
  }
  .main-greeting-text p {
    font-size: 1.35rem;
    margin-top: 0.5rem;
    padding: 0.2rem 0;
    letter-spacing: -0.025rem;
  }
  .main-greeting {
    margin: 0 auto;
  }
  .divide-line {
    margin: 3rem 2rem;
  }
}
@media (min-width: 380px) {
  .main-greeting {
    padding: 0 2.7rem;
  }
  .divide-line {
    margin: 3rem 2.5rem;
  }
  .main-greeting-text p {
    font-size: 1.5rem;
    margin-top: 0.5rem;
    padding: 0.2rem 0;
    letter-spacing: -0.025rem;
  }
}
@media (min-width: 420px) {
  .main-info-title p {
    font-size:2.4rem;
  }
  .main-info-location p {
    font-size: 1.7rem;
  }
  .main-greeting-title p span {
    font-size: 1.4rem;
  }
  .main-greeting-title p {
    font-size: 1.8rem;
  }
  .main-greeting-text p {
    font-size: 1.6rem;
    margin-top: 0.5rem;
    padding: 0.2rem 0;
    letter-spacing: -0.025rem;
  }
  .main-greeting {
    padding: 0 3rem;
  }
  .divide-line {
    margin: 3rem 3rem;
  }
}
</style>