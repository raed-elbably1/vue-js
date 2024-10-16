<template>
    <div class="page1" :class="{ 'homepage-background': isHomePage }"> 
        <div class="links">
            <ul class="ul"> 
                <img src="../photos/Frame.png" class="img" alt="Logo" />
                <li><router-link to="/" class="router-link">الرئيسه</router-link></li>
                <li><router-link to="/about" class="router-link">الاستشارات</router-link></li>
                <li><router-link to="/services" class="router-link">خدماتنا</router-link></li>
                <li><router-link to="/partners" class="router-link">شركاء النجاح</router-link></li>
                <li><router-link to="/careers" class="router-link">الوظائف</router-link></li>
                <li><router-link to="/articles" class="router-link">المقالات</router-link></li>
                <li><router-link to="/faq" class='router-link'>الاسئله الشائعه</router-link></li>
                <li><router-link to="/contact" class="router-link">تواصل معنا</router-link></li>  
                <img src="../photos/Rectangle.png" alt="logo" class="image">
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppHeader',
    computed: {
        isHomePage() {
            return this.$route.path === '/'; // تحقق ما إذا كانت الصفحة الرئيسية
        }
    }
}
</script>

<style>
.page1 {
    display: flex;
    direction: rtl;
    border: 5px solid #ffffff;
    border-radius: 10px;
    backdrop-filter: blur(10px);      background: url('../photos/Rectangle 67.png') no-repeat center center;
    background-size: cover; /* لتغطية الصورة */
    width: 100%; /* لتغطية كامل المساحة */
    height: 100vh;
    top: 0;
    left: 0;    opacity: 1; /* قيمة الشفافية */
  
}



.ul {
    display: flex;
    margin: 0;
    padding: 20px;
    list-style-type: none;
    justify-content: flex-start; /* محاذاة الروابط إلى اليسار */
    direction: rtl; /* لضبط اتجاه المحتوى إلى اليمين */  
  
}

li {
    margin: 30px; /* مسافة بين العناصر */
    height: 20px;
    font-size: 18px;  
    color: #ffffff;
}

li:hover {
    font-size: 20px;
    border: 5px solid ;
    border-radius: 20px;
    backdrop-filter: blur(10px); /* تقليل التأثير */
}

.router-link {
    text-decoration: none; /* إزالة التسطير من الروابط */
    color: #fff; /* التأكد من أن لون النص أسود */
    transition: color 0.3s ease; /* تأثير انتقال سلس عند التغيير */   
}

.router-link:hover {
    color: #ffffff; /* تغيير لون النص عند التمرير */
}

.img {
    width: 135px;
    height: 52px;
}

.image {
    width: 101px;
    height: 66px;
    margin-left: 40px;
}
</style>

