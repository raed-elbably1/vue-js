<template>
    <div class="my-component">
        <img src="../photos/images.png" alt="logo">
    <div class="end">
            <h1 class="title">{{ title }}</h1>
      <p class="description">{{ description }}</p>

        </div>

    </div>
  </template>
  
  <script>
  export default {
    name: 'MyComponent',
    data() {
      return  {
          title: 'مكتب ناصر الكنهل',
        description: 'يقدم الديد من الحلول الاستشاريه والخدمات المتطورة لخدمه القطاعات الاقتصاديه في المملكه العربيه السعوديه', 

    }
  },
}
  </script>
  
  <style scoped>
  .my-component{
    display: flex;
    flex-direction:column ;
    justify-content: center;
    align-items: center;
  }

  </style>