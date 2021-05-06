<template>
<div>
    <v-col lg="12" md="12" sm="12" cols="12">
        <h2 class="myTitle">پروانه‌ها مجوزها و گواهینامه ها</h2>
    </v-col>

<div class="myMembers">
       <v-col lg="4" md="4" sm="12" cols="12" class="text-center"  v-for="item in  Gavahi"
        :key="item.name"
         style="margin-bottom:20px">
        <img v-bind:src="item.src" height="300px"/>
            <p>
                {{item.name}}
            </p>
            <p >
               {{item.year}}
            </p> 
       </v-col>
</div>  

<div class="myMembers">
       <v-col  lg="4" md="4" sm="12" cols="12" class="text-center"  v-for="item in  Parvaneh"
        :key="item.name"
         style="margin-bottom:20px">
        <img v-bind:src="item.src" height="300px"/>
            <p>
                {{item.name}}
            </p>
            <p >
               {{item.year}}
            </p> 
       </v-col>
</div>  

<div class="myMembers">
       <v-col lg="4" md="4" sm="12" cols="12" class="text-center"  v-for="item in  Permission"
        :key="item.name"
         style="margin-bottom:20px">
        <img v-bind:src="item.src" height="300px"/>
            <p>
                {{item.name}}
            </p>
            <p >
               {{item.year}}
            </p> 
       </v-col>
</div>

</div>


</template>

<script>
export default {

    data() {
        return {
          Gavahi: [
                {
                    name: 'وزارت فناوری و اطلاعات',
                    year: '1399',
                    src: require("../assets/1613541928.jpg"),
                },
                {
                  name: 'وزارت صنایع و معادن',
                    year: '1385',
                    src: require("../assets/1613541978.jpg"),
                },
                {
                    name: 'سازمان نظام صنفی',
                    year: '1398',
                    src: require("../assets/1613542199.jpg"),
                },
                ],
         Parvaneh:[
                {
                    name: 'سازمان برنامه و بودجه',
                    year: '1397',
                    src: require("../assets/1613542368.jpg"),
                },
                {
                    name: 'سازمان صنعت و معدن',
                    year: '1396',
                    src: require("../assets/1613542161.jpg"),
                },
                {
                    name: 'سازمان صنعت و معدن',
                    year: '1396',
                    src: require("../assets/1613542265.jpg"),
                }
                ],
         Permission:[
                {
                    name: 'سازمان صنعت و معدن',
                    year: '1396',
                    src: require("../assets/1613542318.jpg"),
                },
                {
                    name: 'سازمان صنعت و معدن',
                    year: '1396',
                    src: require("../assets/1613542105.jpg"),
                },
                 {
                    name: 'سازمان صنعت و معدن',
                    year: '1396',
                    src: require("../assets/1613542038.jpg"),
                },
                ]   
        }
    },
}
</script>

<style scoped>
.myMembers{
    display:flex;
    margin: 5% 10%;
}
.myTitle{
    text-align:center;
     padding:30px 0;
}
.myGavahi{
    width: 50%;
}
</style>
