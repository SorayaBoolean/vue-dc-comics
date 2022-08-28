<template>
    <div id="main">
        
        <section class="main container">
            <section class="contents"> 

                <div class="jumbotron"></div>
                   
                <div class="contents_row">
                    <SingleProduct v-for="(product, index) in products" :key="index" :details="product"/>
                </div> 
               
                   
                              
            </section>
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

    </div>
</template>

<script>
    import SingleProduct from './SingleProduct.vue'

    export default {
    name: 'MyMain',
    components: {
        SingleProduct
    },
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
      ],

      products: [
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel"
            }
]

      
      }}

     

    }

</script>

<style scoped lang="scss">

.contents {
    background-color: #1C1C1C;
    color: white;

      .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-repeat: no-repeat;
         background-size: cover;
        width:100vw;
        height: 270px;
            }
        }

    .contents_row{
        width: 1000px;
        height: 500px;
        margin: auto;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
    }
 
    .products-list{
        display: flex;
        width: 1000px;
        margin: auto;
        border: 1px solid red;

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