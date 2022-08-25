<template>

<div>
    <div class="footer_menu">
        <div class="header_footer">

            <div class="footer_menu_list">
                <div>
                    <h5>DC COMICS</h5>
                    <ul v-for="(comic, index) in dCcomics" :key="index">
                    <li> 
                      <a :href="comic.url">{{comic.text}}</a>
                    </li>
                    </ul>   
                </div>
                <div>
                    <h5>DC</h5>
                    <ul v-for="(doc, index) in Dc" :key="index">
                    <li> 
                      <a :href="doc.url">{{doc.text}}</a>
                    </li>
                    </ul>   
                </div>
                <div>
                    <h5>SITES</h5>
                    <ul v-for="(site, index) in Sites" :key="index">
                    <li> 
                      <a :href="site.url">{{site.text}}</a>
                    </li>
                    </ul>   
                </div>
                  <div>
                     <h5 class="position">SHOP</h5>
                    <ul class="position" v-for="(shopping, index) in shop" :key="index">
                    <li> 
                      <a :href="shopping.url">{{shopping.text}}</a>
                    </li>
                    </ul>   
                </div>
               
            </div>
        
        <div class="Logo_Container">
            <img src="@/assets/img/dc-logo-bg.png" alt="logo-big">
        </div>
    </div>
        

        <div class="bottom_footer">
            <div id="sign_up">
                <h4><a href="#">SIGN-UP NOW!</a></h4>
            </div>
            <div id="follow_us">
                <h4>FOLLOW US!</h4>
                <div id="social_links">
                    <img src="@/assets/img/footer-facebook.png" alt="logo-fb">
                    <img src="@/assets/img/footer-twitter.png" alt="logo-tw">
                    <img src="@/assets/img/footer-youtube.png" alt="logo-y">
                    <img src="@/assets/img/footer-pinterest.png" alt="logo-p">
                    <img src="@/assets/img/footer-facebook.png" alt=""> 
                </div>
            </div>

        </div>
        
    </div>

    
</div>
  
</template>

<script>

    export default {
    name: 'MyFooter',
    data () {
        return {
            dCcomics: [
          {text: 'Characters',
            url: '#'
          },
            {text: 'Comics',
            url: '#',
          },
            {text: 'Movies',
            url: '#',
          },
           {text: 'Tv',
            url: '#',
          },
            {text: 'News',
            url: '#',
          },
            {text: 'Fans',
            url: '#',
            }
          ],

           Dc: [
          {text: 'Terms of use',
            url: '#'
          },
            {text: 'Privacy Policy (New)',
            url: '#',
          },
            {text: 'Ad Choiches',
            url: '#',
          },
           {text: 'Advertising',
            url: '#',
          },
            {text: 'Jobs',
            url: '#',
          },
            {text: 'Subscriptions',
            url: '#',
            },
            {text: 'Talent Workshops',
            url: '#',
          },
            {text: 'CPSC Certificates',
            url: '#',
          },
           {text: 'Ratings',
            url: '#',
          },
            {text: 'Shop Help',
            url: '#',
          },
            {text: 'Contact us',
            url: '#',
            }
          ],

           Sites: [
          {text: 'DC',
            url: '#'
          },
            {text: 'Mad Magazine',
            url: '#',
          },
            {text: 'DC Kids',
            url: '#',
          },
           {text: 'DC Universe',
            url: '#',
          },
            {text: 'DC Power Visa',
            url: '#',
          }
          ],

           shop: [
          {text: 'Shop DC',
            url: '#'
          },
            {text: 'Shop DC Collectibles ',
            url: '#',
          }
          ]
          
        }
    }

    }


</script>


<style scoped lang="scss">

.footer_menu_list {
    max-width: 300px;
    display:flex;
    flex-wrap: wrap;

    div{

        margin: 10px;
    }
}

.header_footer{
    display: flex;
    justify-content: center;
    justify-content: space-around;
    height: 300px;
    background-image: url(@/assets/img/footer-bg.jpg);

    img{
        height: 280px;

    }

    .footer_menu_list {
        margin: 20px 0px;
    }

    h5{
        color: white;
    }

    ul li a{
        color: grey;
        font-size: xx-small;
    }
}
 .position {
        position: relative;
        bottom:90px;
    }

.bottom_footer {
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    background-color: #303030;
}

#sign_up h4 {
    padding: 0px 10px;
    display: flex;
    align-items: center;
    color: white;
    border: 2px solid #0282F9;
    height: 50px;
    
    a {
        text-decoration: none;
        color: white;
    }  
}

#follow_us{
    display: flex;

    img{
        margin: 0px 10px ;
    }

    h4{
      margin-top: 10px;
      color:#0282F9;
    }
    
}

</style>