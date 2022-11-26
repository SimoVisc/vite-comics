<script>
    export default {
    name: "AppMain",
   }
</script>

<template>
    <main>
      <div class="container-top">
            <div class="container ">
                <h1> --Content goes here--></h1>
            </div>
      </div> 
      <div class="container-bottom">
            <div class="container ">
                <ul>
                    <li>
                        <img class="img-big" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </li>
                    <li>
                        <img class="img-big" src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>
          </div>
      </div> 
   </main>
</template>

<style lang="scss">
main{
    padding: 30px;
    .container-top{
        background-color: var(--secondary-color);
       .container{
        padding: 40px 0;
           h1{
                color: #fff;
            }
        }
    }
    .container-bottom{
        background-color: var(--primary-color);
        .container{
            ul {
                display: flex;
                list-style: none;
                
                li{
                    display: flex;
                    align-items: center;
                    padding: 40px 10px;
                    color:#fff;
                    img{
                        width:40px;
                        padding-right: 5px;
                    }
                    .img-big{
                        width:30px;
                    }
                }
            }   
        }
    }
}
</style>