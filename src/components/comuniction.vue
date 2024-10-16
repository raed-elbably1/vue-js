<template>
    <div class="contact-container">
        <div class="call">
            <h2>تواصل معنا</h2>
            <h4>نحن سعداء دائمًا بتواصلك</h4>
        </div>
        <div class="form-info-container">            
            <form @submit.prevent="handleSubmit" class="input">
                <input type="text" placeholder="اسمك*" required aria-label="اسمك" />
                <input type="tel" placeholder="رقم الجوال*" required aria-label="رقم الجوال" />
                <input type="email" placeholder="البريد الإلكتروني*" required aria-label="البريد الإلكتروني" />
                <textarea placeholder="رسالتك*" rows="4" required aria-label="رسالتك"></textarea>
                <button type="submit" class="submit">إرسال</button>
            </form>       
            <div class="info-card">
                <div class="app-call">        
                    <h4>معلومات الاتصال</h4>
                    <h2>نحن سعداء دائمًا بمساعدتك</h2>     
                </div>
                <div class="calls"> 
                    <div class="address">
                        <img src="../photos/mdi_location.png" alt="Location Logo" class="icon" />             
                        <h2>العنوان</h2>
                    </div>
                    <h3>الرياض-حي النزهة-شارع حائل</h3> 
                    <div class="phone">
                        <img src="../photos/clarity_mobile-solid.png" alt="Phone Logo" class="icon" />
                        <h2>رقم موحد</h2>
                        <h4>920004541</h4>
                    </div>
                    <div class="calls1">
                        <div class="phone">
                            <img src="../photos/clarity_mobile-solid.png" alt="Phone Logo" class="icon" />
                            <h2>أرقام الهواتف</h2>
                        </div>
                        <h4>0501176820 - 0504430515 - 0557589833</h4>
                        <div class="email-info">
                            <img src="../photos/iconoir_mail-solid.png" alt="Email Logo" class="icon" />
                            <h2>البريد الإلكتروني</h2>
                            <h4>ar@Kam.sa</h4>
                        </div>
                    </div>
                </div>
            </div>
        </div>  
    </div>
</template>

<script>
export default {
    name: "CommunicationApp",
    methods: {
        handleSubmit() {
            alert("تم إرسال رسالتك!");
        }
    }
}
</script>

<style>
.contact-container {
    max-width: 1800px;
    margin: 20px auto;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    direction: rtl;
    position: relative;
    height: 100vh;
}

.call {
    display: flex;
    flex-direction: column;
    text-align: center;
    margin-bottom: 20px;
}

.form-info-container {
    display: flex;
    justify-content: space-between;
}

.input {
    display: flex;
    flex-direction: column;
    width: 60%;
}

.input input,
.input textarea {
    margin-bottom: 15px;
    padding: 10px;
    border: 1px solid #cccccc;
    border-radius: 5px;
    direction: rtl;
}

.info-card {
    background-color: #e0f7fa;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    width: 30%;
    position: relative;
}

.submit {
    width: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    border: 5px solid #FFF;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    box-shadow: 0 24px 24px rgba(0, 0, 0, 0.2);
    padding: 10px;
    font-size: 20px;
    cursor: pointer;
    transition: background-color 0.3s, transform 0.3s;
}

.submit:hover {
    background-color: rgb(0, 0, 255);
    transform: scale(1.05);
}

/* إضافة الخلفية الزرقاء */
.contact-container::before {
    content: '';
    position: absolute;
    background-color: rgb(1, 48, 136);
    z-index: 0;
    width: 300px;
    height: 100%;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
}

/* تنسيق الأيقونات */
.icon {
    width: 20px; /* عرض الأيقونات */
    height: auto; /* الحفاظ على النسبة */
    margin-left: 5px; /* مسافة بين الأيقونة والنص */
}

/* تنسيق عنوان البريد الإلكتروني */
.email-info {
    display: flex;
    align-items: center;
}

/* تنسيق العناوين بحيث تكون محاذاة مع الأيقونات */
.address, .phone, .email-info {
    display: flex;
    align-items: center;
    margin-bottom: 10px; /* مسافة بين العناصر */
}
</style>
