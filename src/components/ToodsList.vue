<template>
  <div class="toods">
    <h1>خدمات الموقع</h1>
    <h2 class="p5">نسعد دائماً بتقديم خدمات الاستشارات الإدارية والمالية وإدارة الجودة لعملائنا.</h2>
    <div class="page">
      <Card 
        v-for="(item, index) in cards" 
        :key="index" 
        :name="item.name" 
        :date-info="item.dateInfo"
      />
    </div>
  </div>
</template>

<script>
import Card from './Card.vue';

export default {
  name: 'ToodsList',
  components: {
    Card
  },
  data() {
    return {
      cards: [
        { 
          name: 'خدمات تصنيف المقاولين',
          dateInfo: 'إنشاء مختلف أنظمة الإدارة والجودة المتوافقة مع المواصفات العالمية ISO للشركات والمصانع والمدارس والمستشفيات والمعامل والوزارات وغيرها حسب نشاط المنظومة',
        },
        { 
          name: 'استشارات مالية',
          dateInfo: 'تإنشاء مختلف أنظمة الإدارة والجودة المتوافقة مع المواصفات العالمية ISO للشركات والمصانع والمدارس والمستشفيات والمعامل والوزارات وغيرها حسب نشاط المنظومة',
        },
        { 
          name: 'تدريب الموظفين',
          dateInfo: 'تإنشاء مختلف أنظمة الإدارة والجودة المتوافقة مع المواصفات العالمية ISO للشركات والمصانع والمدارس والمستشفيات والمعامل والوزارات وغيرها حسب نشاط المنظومة',
        },
        { 
          name: 'استشارات جودة',
          dateInfo: 'تإنشاء مختلف أنظمة الإدارة والجودة المتوافقة مع المواصفات العالمية ISO للشركات والمصانع والمدارس والمستشفيات والمعامل والوزارات وغيرها حسب نشاط المنظومة',
        },
      ]
    }
  }
}
</script>

<style>
.toods {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.page{
display: flex;
flex-direction: row;
}
.p5{
  width: 729px;
height: 24px;
top: 2586px;
left: 355px;
gap: 0px;
opacity: 0px;
color: rgba(164, 163, 178, 1);

}
</style>
