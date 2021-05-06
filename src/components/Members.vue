<template>
<div>
    <div class="myMebSec">
    <v-col lg="12" md="12" sm="12" cols="12">
        <h2 class="myTitle">اعضای هیئت مدیره</h2>
    </v-col>
    <div class="myMembers">
       <v-card  
       v-for="item in memberships"
       :key="item.name"
        max-width="320"
        id="myCard"
         >
        <v-img v-bind:src="item.src"></v-img>
            <v-card-title id="myCardTitle" class="justify-center">
                {{item.name}}
                <br/>
                 {{item.position}}
            </v-card-title>
             <v-card-title  class="justify-center">
               
            </v-card-title>
       </v-card>
    </div> 
</div>
    <v-col lg="12" md="12" sm="12" cols="12" id="Summery">
    <h2 class="myTitle">افرانت در یک نگاه</h2>
    <v-row id="InnerSummery">
        <v-col lg="4" md="4" sm="12" cols="12" class="text-right">
            <h1>1200</h1>
             <p>مشتری</p>
             <p>شعار ما: مدیریت مخاطرات و فرصت‌های کسب و کار</p>
        </v-col>
        <v-col lg="4" md="4" sm="12" cols="12" class="text-right">
         <h1>22</h1>
         <p>سال سابقه</p>
         <p>این شرکت از با سابقه ترین شرکت های حوزه ی آتی می باشد</p>
         </v-col>
        <v-col lg="4" md="4" sm="12" cols="12" class="text-right">
         <h1>28/200</h1>
          <p>خدمات ارایه شده</p>
          <p> استفاده از فناوری و دانش متناسب در راستای ارائۀ خدمات با کیفیت و امن و توسعه و بهبود مداوم آنها با تاکید براتوماسیون فرآیندها</p>
         </v-col>
    </v-row>
    </v-col>
</div>


</template>

<script>
export default {

    data() {
        return {
          memberships: [
                {
                    name: 'آقای هاشم ربانی',
                    position: 'رئیس هیئت مدیره',
                    src: require("../assets/1613824452518.jpeg"),
                    img: '1613824452518.jpeg'
                },
                {
                    name: 'آقای محمدرضا صادقی',
                    position: 'نائب رئیس هیئت مدیره',
                     src: require("../assets/1613459585.jpeg"),
                    img: '1613459585.jpeg'
                },
                {
                    name: 'آقای فریبرز باذرجانی',
                    position: 'مدیر عامل و عضو هیئت مدیره',
                     src: require("../assets/1613459670.jpeg"),
                    img: '1613459670.jpeg'
                },
                {
                    name: 'سید عباس نوربخش',
                    position: 'عضو هیئت مدیره',
                     src: require("../assets/1613459721.jpeg"),
                    img: '1613459721.jpeg'
                },
                {
                    name: 'احمد فیاض بخش',
                    position: 'عضو هیئت مدیره',
                     src: require("../assets/1613459766.jpeg"),
                    img: '1613459766.jpeg'
                }
            ],
        }
    },
}
</script>

<style>
.myMebSec{
background-color: #f1f6fa;
}
.myMembers{
display:flex;
justify-content: center;
}
.myTitle{
    text-align:center;
    padding:30px 0;
}
#myCard{
margin: 0 10px 100px 10px;
background-color: #164194;
color: white;
}

#Summery{
background-color:#164194;
color:white;
}
#InnerSummery{
margin: 0 12%;
}
</style>