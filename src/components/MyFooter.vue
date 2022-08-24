<template>

<div>
    <div class="footer_menu">
        <div class="header_footer">

            <div class="footer_menu_list">
                <ul>
                    <h3>DC COMICS</h3>
                    <li> <a href="#">CHARACTERS</a></li>
                    <li> <a href="#">COMICS</a></li>
                    <li> <a href="#">MOVIES</a></li>
                    <li> <a href="#">TV</a></li>
                    <li> <a href="#">GAMES</a></li>
                    <li> <a href="#">COLLECTIBLES</a></li>
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
    name: 'MyFooter'

    }


</script>


<style scoped lang="scss">

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

    h3{
        color: white;
    }

    ul li a{
        color: white;
        font-size: xx-small;
    }
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