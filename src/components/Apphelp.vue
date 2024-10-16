<template>
    <div class="page3">
        <div class="hello">
            <h2>المدونه</h2>
            <p>نسعد دائمًا بتقديم خدمات الاستشارات الإدارية والمالية وإدارة الجودة لعملائنا</p>
        </div>
        <div class="cards-contact">
            <div class="card">
                <img src="../photos/Rectangle 2 (1).png" alt="A beautiful landscape" class="logo">
                <div class="essay">
                    <h2>ماهي إدارة نماذج عقود المقاولات وماهي مراحله؟</h2>
                    <p>يفترض كثير من الناس المدراء من جميع المستويات على دراية جيدة بتقنيات إدارة العقود الفعالة، لكن إدارة نماذج عقود المقاولات يمكن أن تكون في الواقع...</p>  
                </div>
                <div class="button">
                    <p>19 أكتوبر 2022</p>
                    <button>قراءة المزيد</button>    
                </div>
            </div>

            <div class="card">
                <img src="../photos/Rectangle 2 (1).png" alt="A beautiful landscape" class="logo">
                <div class="essay">
                    <h2>ماهي إدارة نماذج عقود المقاولات وماهي مراحله؟</h2>
                    <p>يفترض كثير من الناس المدراء من جميع المستويات على دراية جيدة بتقنيات إدارة العقود الفعالة، لكن إدارة نماذج عقود المقاولات يمكن أن تكون في الواقع...</p>    
                </div>
                <div class="button">
                    <p>19 أكتوبر 2022</p>
                    <button>قراءة المزيد</button>     
                </div>
            </div>

            <div class="card">
                <img src="../photos/Rectangle 2 (1).png" alt="A beautiful landscape" class="logo">
                <div class="essay">
                    <h2>ماهي إدارة نماذج عقود المقاولات وماهي مراحله؟</h2>
                    <p>يفترض كثير من الناس المدراء من جميع المستويات على دراية جيدة بتقنيات إدارة العقود الفعالة، لكن إدارة نماذج عقود المقاولات يمكن أن تكون في الواقع...</p>
                </div>
                <div class="button">
                    <p>19 أكتوبر 2022</p>
                    <button>قراءة المزيد</button>  
                </div>
            </div>
        </div>
        <button class="button2">رؤية المزيد</button>
    </div>
</template>

<script>
export default {
    name: 'AppHelp'
}
</script>

<style>
.page3 {
    display: flex;
    flex-direction: column;
    align-items: center;
    direction: rtl;
}

.hello {
    text-align: center;
    font-size: 25px;
    margin-bottom: 10px;
}

.cards-contact {
    display: flex;
    justify-content: center; /* لتوسيع العناصر بشكل متوازن */
    flex-wrap: wrap; /* للسماح للعناصر بالالتفاف إلى الصفوف التالية عند الحاجة */
    width: 100%;
}

.card {
    margin: 10px;
    width: 300px; /* تحديد عرض ثابت لكل بطاقة */
    border: 2px solid #fff;
    border-radius: 20px;
    backdrop-filter: blur(20px);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    padding: 10px 20px;
    background-color: rgba(255, 255, 255, 0.8);
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.essay {
    text-align: center; /* محاذاة النص إلى الوسط */
}

.button {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    background-color: #f0f0f0;
}

.button button {
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    background-color: #007bff;
    color: white;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.button button:hover {
    background-color: #0056b3;
}

.button2 {
    padding: 15px;
    background: rgb(0, 0, 142);
    color: #fff;
    border-radius: 40px;
    backdrop-filter: blur(10px);
    cursor: pointer;
    transition: background 0.3s, transform 0.3s, box-shadow 0.3s;
    width: 130px;
}

.button2:hover {
    transform: scale(1.1);
    box-shadow: 0 0 15px blue, 0 0 30px blue;
}

.logo {
    width: 100%; /* ليكون العرض متجاوبًا */
    height: auto; /* الحفاظ على النسبة */
}

p {
    font-family: 'Readex Pro', sans-serif;
    font-size: 23px;
    font-weight: 300;
    line-height: 24px;
    text-align: center;
}
</style>
