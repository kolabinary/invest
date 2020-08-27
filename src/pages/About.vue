<template>
    <div class="container">

        <section class="jumbo">
            <nav class="nav">
                <div class="logo"><router-link to="/"><img src="../assets/logo.svg" alt="" height="40"></router-link></div>
                <div class="link-up">
                    <router-link to="/about" >About</router-link>
                    <router-link to="/faq" href="">FAQs</router-link>
                    <a href="">Stories</a>
                    <a href="">Blog</a>
                    <a href="" style="color: #622586">Sign In</a>
                    <a href="" class="nav-button">Create Free Account</a>
                </div>
            </nav>
            
            <div class="hero">
                <div><h1>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor</h1></div>
                <div>
                   <p>
                       Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
                       sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem
                       ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore
                       magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea
                       takimata sanctus est Lorem ipsum dolor sit amet.
                   </p>
                </div>
            </div>
        </section>
            
            <div class="image-holder">
                <img src="../assets/play-cover.svg" alt="" height="350">
            </div>

        <team></team>
        <footer1></footer1>
        <footer2></footer2>



    </div>

</template>

<script>

 import team from '../components/about/team'
 import footer1 from '../components/home/footer1.vue'
 import footer2 from '../components/home/footer2.vue'


export default {
  name: 'about',
    components: {
      team,
        footer1,
        footer2
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
    @import "../css/main.css";

    .container {

        /*.link-up {*/
                /*a:hover {*/
                    /*color: #622586 !important;*/
                /*}*/

        /*}*/

        .jumbo {
            height: 70vh;
            padding: 2% 5%;
            background: url('../assets/about-bg.svg');
            background-repeat: no-repeat;
            background-size: 160%;
            /*background-size: cover;*/
            background-position: 55% 50%;

            .hero {
                color:#311342;
                margin-top: 120px;
                display: flex;
                flex-wrap: wrap;
                h1 {
                    font-size: 48px;
                    max-width: 20ch;
                    margin-top: 0;
                }

                p {
                    line-height: 2;
                    font-size: 1.05rem;
                    margin-top: 0;
                }
                div {
                    width: 50%;
                }
            }
        }

        .nav {
            display: flex;
            justify-content: space-between;

            .link-up {
                width: 70%;
                text-align: right;
                a {
                    text-decoration: none;
                    padding: 0 3%;
                    color: #000;
                    font-weight: 600;
                }
                .nav-button {
                    border: 1px solid #622586;
                    padding: 1rem 2rem;
                    border-radius: 3px;
                    color: #622586;
                    font-weight: 600;
                    background-color: #fff;
                    transition: all 0.5s ease-in-out;

                }

                .nav-button:hover {
                    background-color: #622586;
                    color: #fff;
                }


            }
        }

        .image-holder {
            background: url('../assets/play.jpg');
            background-size: cover;
            height: 420px;
            background-repeat: no-repeat;
            position: relative;

            img {
                position: absolute;
                left: -100px;
                top: 50px;
            }
        }

    }

    @media screen and (max-width: 500px) {
        .hero div {
            width: 100vw !important;
            h1 {
                font-size: 30px !important;
            }

            p {
                font-size: 0.9rem !important;
            }
        }

        .hero {

        }
        .jumbo {
            height: 100vh!important;
        }

        .image-holder {
            img {
                height: 100px !important;
            }

        }

        .image-holder {
            height: 220px !important;
            background-position: center;
        }
    }

</style>
