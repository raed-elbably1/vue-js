<template>
    <div class="faq-container">            
        <h2>الأسئلة الشائعة</h2>
        <div class="faq-item" v-for="(item, index) in faqItems" :key="index">
            <div class="faq-question" @click="toggleAnswer(index)">
                {{ item.question }}
                <div class="toggle-icon">
                    <span>{{ item.showAnswer ? '-' : '+' }}</span>                 
                </div>
            </div>        
            <div class="faq-answer" v-if="item.showAnswer">{{ item.answer }}</div>
        </div>         
    </div>
</template>

<script>
export default {
    name: 'ToodsList',
    data() {
        return {
            faqItems: [
                { question: 'ماهو برنامج فرات؟', answer: 'برنامج "فرات" هو منصة تعليمية مبتكرة تهدف إلى تعزيز تجربة التعلم من خلال تقديم محتوى تعليمي متنوع. يجمع البرنامج بين الدروس والمحاضرات التفاعلية، مما يسهل على المتعلمين استيعاب المعلومات بشكل أفضل. يعتمد "فرات" على تقنيات حديثة، مما يتيح للمتعلمين الوصول إلى الموارد التعليمية في أي وقت ومن أي مكان. بالإضافة إلى ذلك، يوفر أدوات لتقييم الأداء، مما يساعد في تتبع التقدم وتحقيق الأهداف التعليمية. في النهاية، يسعى البرنامج إلى تقديم تجربة تعليمية مخصصة تناسب احتياجات كل متعلم.', showAnswer: false },
                { question: 'ماهي الخدمات التي يقدمها برنامج فرات؟', answer: 'برنامج "فرات" يقدم مجموعة متنوعة من الخدمات التعليمية التي تلبي احتياجات المتعلمين. تشمل هذه الخدمات تقديم محتوى تعليمي متنوع يغطي مواضيع متعددة، بدءًا من العلوم والتكنولوجيا إلى الأدب والفنون. كما يتيح البرنامج للمتعلمين الوصول إلى دورات تدريبية وورش عمل تفاعلية تعزز مهاراتهم العملية والنظرية. بالإضافة إلى ذلك، يوفر "فرات" أدوات تقييم متعددة، تساعد في قياس مستوى الفهم وتقدم المتعلمين. يتميز البرنامج أيضًا بواجهة مستخدم سهلة الاستخدام، مما يسهل التنقل والبحث عن المحتوى المطلوب. في النهاية، يهدف "فرات" إلى خلق بيئة تعليمية متميزة تدعم التعلم المستمر وتساهم في تطوير المهارات الشخصية والمهنية.', showAnswer: false },
                { question: 'ماهي الفئات المستهدفة من برنامج فرات؟', answer: 'برنامج "فرات" يستهدف الطلاب والمعلمين وأي شخص يسعى لتطوير مهاراته التعليمية.', showAnswer: false },
            ]
        }
    },
    methods: {
        toggleAnswer(index) {
            this.faqItems[index].showAnswer = !this.faqItems[index].showAnswer;
        }
    }
}
</script>

<style scoped>
.faq-container {
    background-color: rgba(210, 221, 235, 0.5);
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 20px;
    max-width: 800px;
    margin: 20px auto;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.faq-container h2 {
    text-align: center;
    color: #333;
    font-family: 'Arial', sans-serif;
    font-size: 24px;
    margin-bottom: 20px;
}

.faq-item {
    margin-bottom: 15px;
    border-bottom: 1px solid #ddd;
    padding: 10px 0;
    direction: rtl;
}

.faq-question {
    display: flex; /* جعل السؤال وعلامة التبديل في صف واحد */
    justify-content: space-between; /* توزيع العناصر */
    align-items: center; /* محاذاة العمود بشكل مركزي */
    font-weight: bold;
    cursor: pointer;
    color: black;
    transition: color 0.3s;
}

.faq-question:hover {
    text-decoration: underline;
    color: #0056b3;
}

.toggle-icon {
    margin-right: 10px; /* مسافة بين الرمز والنص */
    font-size: 25px;
}

.faq-answer {
    margin-top: 5px;
    color: #555;
    padding: 10px;
    border-left: 4px solid #007bff;
    background-color: #f1f9ff;
    border-radius: 5px;
    transition: max-height 0.3s ease, padding 0.3s ease;
}
</style>


