<template>
<div>
<v-row>
    <v-col  lg="12" md="12" sm="12" cols="12" class="px-0 py-0">
      <div class="AboutUs">
        <h1 class="myInnerTitle">درباره ی ما</h1>
      </div>
    </v-col>
</v-row>   

<v-container>
  <v-row>
        <v-col lg="12" md="12" sm="12" cols="12"> 
          <h2 class="myTitle">تاریخچه افرانت</h2> 
          <p class="myText">شرکت افرانت در سال ١٣٧٦ با هدف توسعه اینترنت و تجارت الکترونیک در کشور تاسیس گردیده و در سال 
          ١٣٩٠ وارد فرابورس ایران شده است. طی این سال‌ها، افرانت توانسته است در ارائه خدمات پهنای باند اینترنت اختصاصی، خدمات دیتاسنتر، رایانش ابری و تجارت الکترونیکی خود را به 
          عنوان پیشگام در خدمت‌رسانی به وزارتخانه‌ها، سازمان‌ها و موسسات متعدد دولتی، نیمه دولتی و خصوصی معرفی و تثبیت نماید
          </p>
          <v-col lg="12" md="12" sm="12" cols="12" align="center">
           <img  class="myImage"
            src="../assets/afranet-color.png"/>
          </v-col>
           
      </v-col>
  </v-row>
 
  <v-row>
     <v-col lg="12" md="12" sm="12" cols="12">
        <h2 class="mySecondTitle">مسئولیت اجتماعی</h2> 
        <p class="myText">شرکت افرانت بعنوان پیشتاز صنعت اینترنت و تجارت الکترونیکی در کشور از طریق برگزاری سمینارها،
         مصاحبه ها، کنفرانس های مطبوعاتی، تشکیل جلسات با مدیران و تصمیم گیرندگان اصلی کشور در حوزه فضای مجازی بویژه مدیران و مسئولان ارشد وزارت 
         ICT و شورایعالی فضای مجازی و غیره نقش تعیین کننده ای در ایجاد فرهنگ IT و آشنایی با صنعت دیتاسنتر بویژه دیتاسنترهای
         Cloud در میان مسئولان ارشد، مدیران میانی کشور و عموم مردم داشته است. همچنین شرکت افرانت همواره تلاش کرده است تا 
        افزون بر ارایه این خدمات، فعالیت‌هایی را فراسوی کسب و کار و براساس رسالت اجتماعی خویش انجام دهد. افرانت علاوه برتمایل به توسعه پایدار و حرکت در جهت توسعه 
        اقتصادی با هدف حمایت از اقشار آسیب پذیر جامعه اقدام به شناسایی مراکز خیریه و عام المنفعه نموده و در این راستا قدم برمی دارد.
        </p>
    </v-col>
  </v-row>


    <v-row >
    <v-col lg="4" md="12" cols="12">
    
        <img  class="mySamplePic" src="../assets/sample1.jpg"/>
      
      </v-col>
      <v-col lg="4" md="12" cols="12">
  
        <img class="mySamplePic" src="../assets/sample2.jpg"/> 
   
      </v-col>
      <v-col lg="4" md="12" cols="12">
  
          <img class="mySamplePic" src="../assets/sample3.jpg"/>
    
      </v-col>
    </v-row>

 
   
</v-container>   
    </div>
</template>

<script>

export default {

data() {
    return {
        
    }
},
}
</script>

<style scoped>


.container{
   position: relative;
}
.myInnerTitle{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
  color:white;
}
.mySection{
  justify-content:center;
  text-align:center;
  margin: 0 10%;
}
.AboutUs{
  position:relative;
  background-image: url("../assets/about.jpg");
  width: 100%;
  height: 50vh;
  background-repeat: no-repeat;
  background-size: cover;
}
.myPicture{
  max-width:100%;
  height:auto;
}
.mySamplePic{
  width: 100%;
}
.mySecondTitle{
  padding-bottom: 30px;
   text-align:center;
}
.myText{
  text-align: right;
}
</style>