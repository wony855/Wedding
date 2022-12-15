<template>
  <div class="contact">
    <div class="contactH">
      <div class="contact-1">
        <p>신랑에게 연락하기</p>
        <div class="buttons btn-center">
          <div class="contact-1-call">
            <a href="tel:010-5161-5044">
              <div class="icon"><img :src="require('@/assets/images/phone.svg')" /></div>
            </a>
          </div>
          <div class="contact-1-msg">
            <a href="sms:010-5161-5044">
              <div class="icon"><img :src="require('@/assets/images/envelope.svg')" /></div>
            </a>
          </div>
        </div>
      </div>
      <!-- 신랑에게 연락하기 -->

      <div class="contact-2">
        <div>
          <p>신부에게 연락하기</p>
          <div class="buttons btn-center">
            <div class="contact-2-call">
              <a href="tel:010-8405-2322">
                <div class="icon"><img :src="require('@/assets/images/phone.svg')" /></div>
              </a>
            </div>
            <div class="contact-2-msg">
              <a href="sms:010-8405-2322"><div class="icon">
                <img :src="require('@/assets/images/envelope.svg')" /></div>
              </a>
            </div>
          </div>
        </div>
      </div>
      <!-- 신부에게 연락하기 -->
    </div>

    <!-- 토글 -->
    <div v-if="!toggle" >
      <button @click="handleToggleButton">
        더보기 <i class="fa-solid fa-circle-chevron-down"></i>
      </button>
    </div>
    <div v-else class="toggle-button">
      <button @click="handleToggleButton">
        접 기 <i class="fa-solid fa-circle-chevron-up"></i>
      </button>
    </div>

    <!-- 토글버튼 -->
    <div class="toggle-box" v-if="toggle">
      <div class="grooms">
        <p>신랑측 혼주</p>
        <div class="grooms-contact">
          <div>
            <p>아버지 왕대환</p>
            <div class="buttons parents-btn-center">
              <div class="contact-1-call">
                <a href="tel:010-8592-5339">
                  <div class="icon">
                    <img :src="require('@/assets/images/phone.svg')" /></div
                ></a>
              </div>
              <div class="contact-1-msg">
                <a href="sms:010-8592-5339"
                  ><div class="icon">
                    <img :src="require('@/assets/images/envelope.svg')" /></div
                ></a>
              </div>
            </div>
          </div>
          <p>어머니 김정국</p>
          <div class="buttons parents-btn-center">
            <div class="contact-1-call">
              <a href="tel:010-3634-5339">
                <div class="icon">
                  <img :src="require('@/assets/images/phone.svg')" /></div
              ></a>
            </div>
            <div class="contact-1-msg">
              <a href="sms:010-3634-5339">
                <div class="icon">
                  <img :src="require('@/assets/images/envelope.svg')" /></div
              ></a>
            </div>
          </div>
        </div>
      </div>
      <!-- 신랑측 혼주 -->
      
      <div class="brides">
        <p>신부측 혼주</p>
        <div class="grooms-contact">
          <p>어머니 송미숙</p>
          <div class="buttons parents-btn-center">
            <div class="contact-1-call">
              <a href="tel:010-9795-2322"
                ><div class="icon">
                  <img :src="require('@/assets/images/phone.svg')" /></div
              ></a>
            </div>
            <div class="contact-1-msg">
              <a href="sms:010-9795-2322">
                <div class="icon">
                  <img :src="require('@/assets/images/envelope.svg')" /></div
              ></a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- 신부측 혼주 -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggle: false,
    };
  },
  methods: {
    handleToggleButton() {
      this.toggle = !this.toggle;
    },
  },
};
</script>

<style scoped>
.toggle-button {
  animation: rotateX 300ms ease-in-out forwards;
}
.contact {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 47rem;
}
.contactH {
  display: flex;
  flex-direction: row;
}
.contact-1,
.contact-2 {
  margin: 0 3rem;
}
.contact-1 p,
.contact-2 p {
  font-size: 1.6rem;
  text-align: center;
}
.contact button {
  border: none;
  background: none;
  font-size: 1.6rem;
  color: #d6ac8a;
}
.contact-1-call img,
.contact-2-call img,
.contact-1-msg img,
.contact-2-msg img {
  margin-right: 1rem;
  width: 1.5rem;
}
.buttons {
  display: flex;
  padding-top: 3.4rem;
  justify-content: space-around;
  width: 8rem;
  opacity: 0.6;
}
.parents-btn-center {
  padding: 1rem 1rem 1rem 2.25rem;
}
.btn-center {
  padding: 1rem 1rem 1rem 3.25rem;
}
.toggle-box {
  display: flex;
  font-size: 1.5rem;
  text-align: center;
  animation: fadein 300ms ease-in-out forwards;
}
.grooms,
.brides {
  margin: 0 4.6rem;
}

#rotate-btn {
  transform: rotate(180deg);
}
@media (min-width: 350px) {
  .contact-1 p,
  .contact-2 p {
    font-size: 1.7rem;
    text-align: center;
  }
  .contact-1-call img,
  .contact-2-call img,
  .contact-1-msg img,
  .contact-2-msg img {
    margin-right: 1rem;
    width: 1.6rem;
  }
  
  .grooms p,
  .brides p {
    font-size: 1.6rem;
  }
}
@media (min-width: 420px) {
  .contact-1 p,
  .contact-2 p {
    font-size: 1.8rem;
    text-align: center;
  }
  .contact-1-call img,
  .contact-2-call img,
  .contact-1-msg img,
  .contact-2-msg img {
    margin-right: 1rem;
    width: 1.8rem;
  }
  .grooms p,
  .brides p {
    font-size: 1.8rem;
  }
}
@keyframes fadein{
  0% {
    transform: scale(0, 0);
    opacity: 0;
  }
  100% {
    transform: scale(1, 1);
    opacity: 1;
  }
}
@keyframes rotateX {
  0% {
    transform: rotateX(-90deg);
  }
  100% {
    transform: rotateX(0deg);
  }
}
</style>