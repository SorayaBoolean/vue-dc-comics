<template>

<div>
    <div class="footer_menu">
        <div class="header_footer">

            <div class="footer_menu_list">
                <ul v-for="(comic, index) in dCcomics" :key="index">
                    <h5>DC COMICS</h5>
                    <li> 
                      <a :href="comic.url">{{comic.text}}</a>
                    </li>
                </ul>

                <ul>
                    <h5>DC COMICS</h5>
                    <li> <a href="#">CHARACTERS</a></li>
                </ul>
                <ul>
                    <h5>DC COMICS</h5>
                    <li> <a href="#">CHARACTERS</a></li>
                </ul>

                 <ul class="position">
                    <h5>DC COMICS</h5>
                    <li> <a href="#">CHARACTERS</a></li>
                </ul>
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
                <h4>Follow Us!</h4>
                <div id="social_links">
                    <img src="" alt="facebook">
                    <img src="" alt="twitter">
                    <img src="" alt="youtube">
                    <img src="" alt="Pintrest">
                    <img src="" alt="Maps">
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

    ul {
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
        top: -90px;
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
    
}

</style>