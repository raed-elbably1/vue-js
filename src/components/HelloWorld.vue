<template>
  <div class="hello" @click="changeNumber">
    <div class="page2">
      <h2>ناصر الكهنل للاستشارات الادرايه</h2>
      <p>نحن نقدم بشكل مستمر الحلول والخدمات المتطورة</p>
      <span class="number-display">+{{ number }}</span>
      <p class="description">{{ description }}</p>
    </div>
    <button @click="goToabout" class="consult-button">
      <i class="fas fa-arrow-left"></i>  طلب استشارة 
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      number: 320,
      descriptions: {
        320: "استشارات التطوير العقاري",
        240: "استشارات اداريه",
        215: "استشارات الجوده",
        900: 'تصنيف المقاولين'
      },
      description: "وصف الرقم 320"
    };
  },
  methods: {
    goToabout() {
      this.$router.push('/about');
    },
    changeNumber() {
      if (this.number === +320) {
        this.number = +240;
      } else if (this.number === +240) {
        this.number = +215;
      } else if (this.number === +215) {
        this.number = +900;
      } else {
        this.number = +320;
      }
      this.updateDescription();
    },
    updateDescription() {
      this.description = this.descriptions[this.number];
    }
  },
  mounted() {
    this.updateDescription();
  },
}
</script>

<style scoped lang="scss">
.hello {  
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 400px;
  height: 60vh;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.page2 {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 20px;
  color: #fff;
}

.number-display {
  font-size: 100px;
  font-weight: bold;
  margin-top: 20px;
  cursor: pointer;
}

.description {
  font-size: 18px;
  color: #fff;
  margin-top: 10px;
}

.consult-button {
  margin-top: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 2px solid #fff;
  border-radius: 20px;
  backdrop-filter: blur(20px);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  padding: 20px;
  background-color: rgba(255, 255, 255, 0.8);
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.3s ease;
  width: 164px;
height: 24px;
top: 556px;
left: 637px;
gap: 0px;
opacity: 0px;
color: rgb(0, 0, 255);

}

.consult-button:hover {
  background-color: rgba(255, 255, 255, 1);
  transform: scale(1.05);
}
.fas{
  margin-right: 5px;
}
</style>
