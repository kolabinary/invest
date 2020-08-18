<template>
    <div class="container">
    <div class="main">
        <div>
            <h1>Invest securely now.</h1>
            <a class="acc gen-hover2" href="">Create a free Account</a>
            <div class="download-btn">
                <a href="" class="hero-btn2 gen-hover"><img src="../../assets/playstore1.svg" alt="" height="35"></a>
                <a href="" class="hero-btn3 gen-hover"><img src="../../assets/appstore1.svg" alt="" height="35"></a>
            </div>

        </div>
        <div class="text-cup">
            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore</p>
        </div>
    </div>

    </div>

</template>

<script>
export default {
  name: 'footer1'

}
</script>


<style lang="scss" scoped>

    @import '../../css/main.css';

    .container {
        padding: 3% 5%;
        background-color: #FCFAFD;

        .main > div {
            width: 50%;
        }

        .main {
            display: flex;
            background: url('../../assets/footer1-bg.svg');
            background-repeat: no-repeat;
            background-position: right center;
            background-size: 54%;
            background-color: #833FAB;
            padding: 2rem 4rem;



            h1 {
                color: #fff;
                font-size: 50px;
                max-width: 15ch;
                line-height: 1.2;
                letter-spacing: 0.5px;
                margin-top: 0;
            }

            p {
                text-align: right;
                color: #fff;
                font-size: 18px;
                /*margin: 0 auto;*/

              }

            .text-cup {
                margin:2rem 10rem 2rem 3rem ;
            }
           .acc {
                padding: 1.4rem 6rem;
                border: 1px solid #F2C45A;
               text-decoration: none;
               color: #F2C45A;
               font-weight: 700;
               display: inline-block;
               margin: 0.5rem 0 0 0;
               letter-spacing: 1px;
               font-size: 18px;
               border-radius: 5px;
               transition: all 0.3s ease-in-out;
            }

            .hero-btn2 {
                display: inline-block;
                margin-top: 1rem;
                background-color: #fff;
                padding: 0.7rem 2rem 0.6rem 2rem;
                border-radius: 7px;
                margin-right: 1rem;
                transition: all 0.3s ease-in-out;
            }
            .hero-btn3 {
                display: inline-block;
                margin-top: 1rem;
                background-color: #fff;
                padding: 0.7rem 2rem 0.6rem 2rem;
                border-radius: 7px;
                transition: all 0.3s ease-in-out;
            }

            .download-btn {
                width: 100%;
                margin-top: 2rem;
            }
        }
    }


</style>
