<template>
  <div>
    
    <nav class="container">
        <a href="#">
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </a>

        <ul>
            <li v-for="(link,index) in links" :key="index"> 
              <a :href="link.url">{{link.text}}</a>
            </li>
            
        </ul>

    </nav>


  </div>
</template>

<script>

    export default {
    name: 'MyHeader',
    data () {
      return {
        links: [
          {text: 'Characters',
            url: '#',
            active: false
          },
            {text: 'Comics',
            url: '#',
            active: false
          },
            {text: 'Movies',
            url: '#',
            active: true
          },
           {text: 'Tv',
            url: '#',
            active: false
          },
            {text: 'Games',
            url: '#',
            active: false
          },
            {text: 'Collectibles',
            url: '#',
            active: true
          },
           {text: 'Videos',
            url: '#',
            active: false
          },
          {text: 'Fans',
            url: '#',
            active: false
          },
          {text: 'News',
            url: '#',
            active: false
          }


        ]

      }

        }

    }

</script>


<style scoped lang="scss">

  ul {
    display: flex;
    justify-content: space-around;

    li {
      margin: 10px;
      display: flex;
      align-items: center;
      font-size: smaller;
        a {
            color: rgb(27, 27, 27);
        }
     
    }
  }
  nav {
    padding: 10px 0px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: auto;
    max-width: 1000px;

    img {
      height: 70px;
      widows: 70px;
    }
  }



</style>
