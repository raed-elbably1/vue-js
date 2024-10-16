<template>
  <div class="card">
    <img src="../photos/Group 9.png" alt="logo" >
    <h2>{{ name }}</h2>
    <p>{{ dateInfo }}</p> <!-- استخدام اسم آخر هنا -->
    <button>معرفه المزيد</button>
  </div>
</template>

<script>
export default {
  name: 'CardsList',
  props: {
    name: String,
    dateInfo: String // تغيير الاسم هنا
  }
}
</script>

<style scoped>
.card {
  padding: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  margin: 10px;
  text-align: center;
  width: 300px;
}

.card:hover {
  transform: translateY(-5px); /* رفع الكارت عند التمرير */
}
button{
  background-color:rgba(0, 0, 253, 0.707);
  color: #fff;
  border:2px solid #fff ;
  border-radius: 20px ;
  backdrop-filter: blur(20px);
  padding: 15px;
  transition: background 0.3s, color 0.3s; /* تأثير سلس على الخلفية واللون */
  cursor: pointer;
  font-size: 20px;
}
button:hover {
  background: #fff;
  color: black;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* ظل خفيف */
}
img{
  height: 100px;
  transform: translateY(-5px);
  width: 65px;
height: 65px;
top: 976px;
left: 215px;
gap: 0px;
opacity: 0px;

}
p{
  width: 270px;
height: 120px;
top: 1097px;
left: 743px;
gap: 0px;
opacity: 0px;


color: rgba(164, 163, 178, 1);
width: 100%;

}
</style>
