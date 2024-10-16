<template>
    <div class="app">
        <div class="pohots">
            <img src="../photos/_Client logo (5).png" alt="logo" class="logo5">
            <img src="../photos/_Client logo (4).png" alt="logo" class="logo5">
            <img src="../photos/_Client logo (3).png" alt="logo" class="logo5">
            <img src="../photos/_Client logo (2).png" alt="logo" class="logo5">
            <img src="../photos/_Client logo (1).png" alt="logo" class="logo5">
            <img src="../photos/_Client logo.png" alt="logo" class="logo5">
        </div> 
        <div class="continer">
 <img src="../photos/Rectangle 82hello.png" alt="logo" class="img"> 
 <div class="our-app">
    <h2>عن المكتب</h2>
    <p class="p1">منذ تأسيس مكتب ناصر الكنهل للاستشارات الإدارية بالعام ٢٠١١ م، ونحن نقدم بشكل مستمر الحلول والخدمات المتطورة التي تحتاجها القطاعات الاقتصادية في المملكة العربية السعودية، ودائماً نأخذ على عاتقنا بالعمل على تميز الاستشارات المقدمة إلى عملائنا، ونسعى جاهدين دائماً لتعزيز الاستدامة في القطاعات الاقتصادية، ويتميز فريق العمل لدينا بالخبرات والمؤهلات اللازمة لتقديم الاستشارات وفق أعلى المعاير المنظمة...</p>
    <button>معرفه المزيد</button>
</div>
            </div>            
            <div class="contect">
    <div class="our">
        <h2>320+</h2> <!-- تم تغيير الرقم -->
        <h3>استشارات تطوير العقاري</h3>
    </div>
    <div class="app-our">
        <h2>215+</h2> <!-- تم تغيير الرقم -->
        <h3>استشارات إدارية</h3>
    </div>
    <div class="number">
        <h2>492+</h2> <!-- تم تغيير الرقم -->
        <h4>استشارات الجودة</h4>
    </div>
    <div class="name">
        <h2>956+</h2> <!-- تم تغيير الرقم -->
        <h3>تصنيف المقاولين</h3>
    </div>
 
</div>
   <div class="advir">
    <div class="logo">
    <img src="../photos/Layer_1.png" alt="logo" class="logo">
    </div>
   
        <h2>طلب استشاره مجانيه</h2>
        <p class="p2">انطلاقاً من المسؤولية الاجتماعية للمكتب، يرحب دائماً مكتب ناصر الكنهل للاستشارات الإدارية بالإجابة عن كافة الاستفسارات الخاصة بأنشطة الاستشارات الإدارية والمالية</p>
 <button class="button"> معرفه المزيد
    <i class="  button1 fas fa-arrow-left"></i>  </button> 
    </div>

    </div>
</template>

<script>
export default {
    name: 'ReactApp'
}
</script>

<style scoped>

.continer {
    background: #ffffff;
    display: flex; /* استخدام flexbox لتوزيع العناصر */
    padding: 20px; /* إضافة مسافة داخلية */
}

.pohots { 
    background: rgb(241, 241, 241);
    display: flex; 
    justify-content: center; 
    padding: 20px; 
    gap: 20px; /* زيادة المسافة بين الصور */
}

@media (max-width: 600px) {
    .pohots {
        display: flex;
        flex-direction: column; 
        margin: 200px;
        gap: 10px; /* أو تعديل المسافة حسب الحاجة */
    }
}

.logo5{
    display: flex;
    margin: 20px;
}
.img {
    display: flex;
    border: 5px solid #fff;
    border-radius: 20px;
    backdrop-filter: blur(20px);
    align-items: center; /* لمركزة المحتوى داخل الصورة */
    justify-content: center; /* لمركزة المحتوى داخل الصورة */
    width: 447px;
height: 444px;
top: 1545px;
left: 168px;
gap: 0px;
border-radius: 10px 0px 0px 0px;
opacity: 0px;

}

.our-app {
    display: flex;
    justify-content: flex-end;
    flex-direction: column;
    direction: rtl; 
    width:100%;
    padding: 20px; /* إضافة padding لجميع الجوانب */
    background-image: url('../photos/24px Gridpng.png'); 
    background-size: cover; /* جعل الصورة تغطي العنصر */
    height: 50vh2;

}
.p1{
    width: 63%;
    font-family: Readex Pro;
font-size: 25px;
font-weight: 400;
line-height: 24px;
text-align: right;
color: rgba(164, 163, 178, 1);

}

h2 {
    font-size: 40px;
}
button{
    background: rgba(163, 112, 112, 0.732);
    border: 2px solid #fff;
    font-size: 20px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    box-shadow: 0 24px 24x #fff;
    padding: 15px;
    width: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 100px ;
    cursor: pointer;
}
button:hover {
    background: #684f4f63; /* تغيير لون الخلفية إلى الأبيض */
    border: 2px solid #fff; /* تغيير لون الحدود إلى الأبيض */
    border-radius: 20px; /* جعل الزوايا مستديرة */
    backdrop-filter: blur(10px); /* إضافة تأثير ضبابي للخلفية */
    box-shadow: 0 24px 24px rgba(255, 255, 255, 0.5); /* ظل للزر */
    transition: all 0.3s ease; /* إضافة انتقال سلس */

}
.button {
    background: #fff;
    border: 2px solid #fff;
    font-size: 20px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    box-shadow: 0 24px 24px rgba(255, 255, 255, 0.5);
    padding: 15px;
    width: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 30px;
    margin-top: -80px ;
    cursor: pointer;
    direction: rtl;
}

.button1 {
    margin-right: 5px;
    direction: rtl;
}

.button:hover {
    background: #f0f0f0; /* تغيير لون الخلفية عند التحويم */
    transition: all 0.3s ease; /* إضافة انتقال سلس */
}

.contect {
    display: flex;
    direction: rtl;
    padding: 20px;
}

.our, .app-our, .number, .name {
    padding: 20px; /* اجعل padding موحدًا */
    background: rgba(1, 48, 136, 0.347);

    color: #000dff;
    border: 5px solid rgb(255, 255, 255);
    border-radius: 20px;
    backdrop-filter: blur(10px);
    margin-left: 20px; /* إضافة مسافة بين البطاقات */    
    padding:10px ;
    width: 100%;
    font-size: 30px;


 
}

.our:first-child {
    margin-left: 50px; /* إزالة المسافة للبطاقة الأولى */
}

.our, .app-our, .number, .name {
    margin-bottom: 20px; /* إضافة مسافة أسفل كل بطاقة */
}
.advir {
    color: white;
    padding: 40px;
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;   
    direction: rtl;
    margin: 20px auto; /* هوامش علوية وسفلية */
    border-radius: 10px; /* زوايا مستديرة */
    text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.5); /* ظل للنص */
    position: relative; /* للسماح بتحديد موضع الشعار */
    background: rgba(1, 48, 136, 1);

}

.logo {
    position: absolute; /* السماح للشعار بالتداخل فوق الخلفية */
    top: 10px; /* ضبط المسافة العلوية حسب الحاجة */
    width: 197px;
    height: 263px;
    opacity:1; /* التحكم في الشفافية */
    direction: rtl;
    right: 10px;
}
.p2{
    width: 517px;
height: 168px;
top: 1671px;
left: 754px;
gap: 0px;
opacity: 0px;

color: rgba(255, 255, 255, 1);

}
p {
    margin-top: -20px; /* Adjust as needed */
}




</style>
