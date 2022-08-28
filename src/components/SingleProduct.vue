<template>

    <div class="product_card">
        <div class="img_box">
            <img :src="details.thumb" alt="">
        </div>
        <div class="title_box">
            <h4>{{details.series}}</h4>
        </div>
    </div>  
   
</template>

<script>
export default {
    name: 'SingleProduct',
    props: {
        details: Object
    }

}
</script>

<style scoped lang="scss">

.product_card{
            margin: 20px 10px;
            height: 200px;
            width: calc(100% / 7);

            .title_box {
                h4{
                    font-weight: 100;
                    margin: 10px 0px;
                }
            }

            .img_box{
                height: 70% ;

                img{
                    width: 100%;
                    height: 100%;
                    object-fit:cover;
                    object-position: 0px 5px;
                   
                }
            }
         }
    

</style>