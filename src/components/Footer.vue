<template>
<div class="myFooter">
    <v-row class="py-5" id="MainRow">
        <v-col lg="2" class="text-right">
            <h3>تماس</h3>
            <p>www.afranet.ir</p>
            <p>021-81181-5</p>
            <p>pr[AT]afranet.ir</p>
        </v-col>
        <v-col lg="2" class="text-right">
            <h3>دسترسی سریع</h3>
            <p>فرم استخدام</p>
            <p>همکاری در فروش</p>
            <p>امور سهام</p>
        </v-col>
        <v-col lg="2" class="text-right">
            <h3>خدمات افرانت</h3>
            <p>پهنای باند اختصاصی</p>
            <p>پهنای باند سازمانی</p>
            <p>فضای دیتا سنتر</p>
            <p>سرور اختصاصی</p>
            <p>سرور ابری</p>
            <p>ایمیل سازمانی</p>
        </v-col>
        <v-col  lg="2" class="text-right">
            <h3>افرانت</h3>
            <p>اخبار</p>
            <p>امور سهام</p>
            <p>همکاری با ما</p>
            <p>درباره ما</p>
            <p>تماس با ما</p>
        </v-col>
        <v-col lg="2" class="text-right">
             <h3>ابزارها</h3>
             <p>سوالات متداول</p>
             <p>تست سرعت</p> 
              <p>آموزش</p>
        </v-col>
        <v-col lg="2" class="text-center">
            <img src="../assets/afranet.png"/>
            <img src="../assets/cra.png"/>
        </v-col>
    </v-row>
</div>
   
</template>

<script>
export default {
    data(){
        return{

        }
    }
}
</script>
<style scoped>
.myFooter{
    background-color:#223144;
}
h3{
    color:white
}
p{
    color:white
}
#MainRow{
margin: 0 10%;
}
</style>