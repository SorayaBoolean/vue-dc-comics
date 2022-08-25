<template>
    <div id="main">
        
        <section class="main container">
            <section class="contents"> 
                <div class="contents_row">
                    <h3> >Contents goes here </h3> 
                </div>
                
            </section>

            <section class="shop_nav">
                <div class="shop_nav_list">
                    <ul>
                    <li v-for="(text,index) in menu" :key="index"> 
                        <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
                        <a :href="text.url">{{text.text}}</a>
                    </li>
                </ul>
                </div>
                
            </section>

        </section>
        

    </div>
</template>

<script>

    export default {
    name: 'MyMain',
    data () {
      return {
        menu: [
          {text: 'DIGITAL COMICS',
            url: '#',
            img: '', 
          },
            {text: 'DC MERCHANDISE',
            url: '#',
            img: '',
          },
            {text: 'SUBSCRIPTION',
             url: '#',
             img: '', 
          },
           {text: 'COMIC SHOP LOCATOR',
            url: '#',
            img: '',
          },
           {text: 'DC POWER VISA',
            url: '#',
            img: '',
          }
      ]
      }}

    }

</script>

<style scoped lang="scss">

.contents {
    background-color: #1C1C1C;
    height: 80px;
    color: white;

    .contents_row{
        margin: auto;
        height: 100%;
        max-width: 1000px;
        display: flex;
        align-items: center;
    }
}

.shop_nav {
    display: flex;
    align-items: center;
    background-color: #0282F9;
    height: 100px;

     .shop_nav_list {
            margin:auto;
            height: 100px;
            width: 1000px;
         }

    ul{
        height: 100%;
        max-width: 1000px;
        display: flex;
        justify-content: space-between;
        align-items:center ;
        margin:auto;
         li{
            display:flex;
            align-items: center;
            margin: 0px;
            font-weight: bold;
            font-size: x-small;

    ;
            a{
                color:white;
            }    
         }
         img {
            height: 70px;
            widows: 70px;
            margin: 10px;
         }

        
    }

}





</style>