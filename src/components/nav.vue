<template>
<div>
    <header>
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <nav>
            <ul>
                <li v-for="item in links" :key="item.label">
                  <a>{{item.label}}</a>
                </li>
            </ul>
        </nav>
        <nav>
            <ul>
               <li> <a>ثبت نام</a></li>
                <li><a>ورود</a></li>
               
            </ul>
        </nav>
    </header>
     <div class="col-lg-12" id="mySubHeader">

        <base-button id="myBtn">
        پشتیبانی
          <v-icon color="white" id="myIcon">
          mdi-account-circle-outline
          </v-icon>
        </base-button>

         <nav>
            <ul>
               <li> <a>خدمات پهنای باند</a>
                <v-icon  id="myIcon">
                mdi-access-point-network
                </v-icon></li>
               <li><a>خدمات دیتا سنتر</a>
               <v-icon  id="myIcon">
                  mdi-database
                </v-icon>
               </li>
               <li><a>خدمات ابری</a>
                <v-icon  id="myIcon">
                  mdi-google-cloud
                </v-icon>
               </li>
              <li><a>خدمات پشتیبانی</a>
                <v-icon  id="myIcon">
                  mdi-account-circle-outline
                </v-icon>
              </li>  
            </ul>
        </nav>

          <img 
          class="myImage" 
          src="../assets/afranet-color.png"/>

    </div>
    
 </div>  
</template>

<script>
export default {
    data(){
      return{
        links: [
        {
          label: "EN",
          url: "/",
        },
        {
          label: "تماس با ما",
          url: "/",
        },
        {
          label: "درباره ی ما",
          url: "/",
        },
         {
          label: "همکاری با ما",
           url: "/",
        },
         {
          label: "خانه",
          url: "/",
        },
        
      ],
      }
    }
}
</script>
<style scoped>
header {
  height: 50px;
  background-color: #164194;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

ul {
  list-style: none;
  margin: 0 100px;
  padding: 0;
  display: flex;
  justify-self: center;
  align-items: center;
}

li {
  margin: 0 1rem;
}

a {
  font-size:15px;
  text-decoration: none;
  color: white;
  font-weight: bold;
  border-bottom: 2px solid transparent;
  padding-bottom: 0.25rem;
}

a:hover,
a:active,
a.router-link-active {
  color: white;
}


.v-application a{
    color: white;
}
 .v-application ul {
    padding-left: 0px;
}
#mySubHeader{
display: flex;
align-items: center;
}
.myImage{
  position: absolute;
  right:100px;
  width: 150px;
  height: 50px;
}
#myBtn{
margin-left: 100px;
padding: 10px 20px;
 cursor: pointer;
  border: 1px solid palevioletred;
  background-color: #e63323;
  color: white;
  box-shadow: 5px 5px 5px rgb(253 179 179);
  border-radius: 4px;
}
#myBtn button:hover,
#myBtn button:active {
  background-color: palevioletred;
} 
#myIcon{
  padding-left: 5px;
}
#mySubHeader nav{
  position: absolute;
  right: 200px;
  justify-self: center;

}
#mySubHeader a {
   color: rgb(148, 148, 148);
}
</style>