<template>
    <div class="container">
        <div class="jumbo">
            <nav class="nav">
                <div class="logo"><img src="../assets/logo.svg" alt="" height="40"></div>
                <div class="link-up">
                   <router-link to="/about" >About</router-link>
                    <router-link to="/faq" href="">FAQs</router-link>
                    <a href="">Stories</a>
                    <a href="">Blog</a>
                    <a href="" style="color: #622586">Sign In</a>
                    <a href="" class="nav-button">Create Free Account</a>
                </div>
            </nav>

            <section class="hero">
                <div class="hero-text">
                    <h1>Risk-free <span>secure investment</span>  anywhere, anytime.</h1>
                    <p>The first-ever app that enables you to securely purchase and manage
                        Treasury Bills and Eurobonds from your mobile device.</p>
                    <a href="" class="hero-btn1">Create a Free Account</a> <br>
                    <div class="download-btn">
                        <a href="" class="hero-btn2"><img src="../assets/playstore.svg" alt="" height="30"></a>
                        <a href="" class="hero-btn3"><img src="../assets/appstore.svg" alt="" height="30"></a>
                    </div>

                </div>
                <div class="hero-image">

                    <img src="../assets/hero.png" alt="" height="600">
                </div>
            </section>
        </div>

        <body1></body1>
        <body2></body2>
        <body3></body3>
        <body4></body4>
        <body5></body5>
        <footer1></footer1>
        <footer2></footer2>

    </div>
</template>

<script>
    import body1 from '../components/home/body1.vue'
    import body2 from '../components/home/body2.vue'
    import body3 from '../components/home/body3.vue'
    import body4 from '../components/home/body4.vue'
    import body5 from '../components/home/body5.vue'
    import footer1 from '../components/home/footer1.vue'
    import footer2 from '../components/home/footer2.vue'


    export default {
        name: 'home',
        components: {
            body1,
            body2,
            body3,
            body4,
            body5,
            footer1,
            footer2
        }
    }
</script>

<style lang="scss" scoped>
    .container {


        .jumbo {
            height: 90vh;
            background: url('../assets/hero-bg.svg');
            background-repeat: no-repeat;
            padding: 2% 5%;
            background-position: 120% 50%;
            background-size: 25%;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .hero {
            display: flex;
            margin-top: 30px;
            flex-wrap: wrap;



            div {
                width: 50%;
            }
            .hero-image {
                text-align: right;
                img {
                    margin-top: -25px;
                }
            }
            .hero-text {
                p {
                    max-width: 60ch;
                    color: #8D8194;
                    margin-bottom: 1rem;
                    line-height: 1.5;
                }
                h1 {
                    line-height: 1.3;
                    font-size: 55px;
                    margin-bottom: 0;
                    span {
                        color: #8F5EAB;
                    }

                }
            }
            .hero-btn1 {
                padding: 1.5rem 5rem;
                background-color: #FADE9D;
                color: #622586;
                text-decoration: none;
                font-weight: 600;
                border-radius: 3px;
                margin-top: 1rem;
                display: inline-block;
                font-size: 20px;
                transition: all 0.5s ease-in-out;

            }
            .hero-btn1:hover {
               outline: 1px solid #622586;
            }

            .hero-btn2 {
                display: inline-block;
                margin-top: 1rem;
                background-color: #311342;
                padding: 0.7rem 2rem 0.6rem 2rem;
                border-radius: 7px;
                margin-right: 1rem;
            }

            .hero-btn3 {
                display: inline-block;
                margin-top: 1rem;
                background-color: #311342;
                padding: 0.7rem 2rem 0.6rem 2rem;
                border-radius: 7px;
            }

            .download-btn {
                width: 100%;
                margin-top: 2rem;
            }
        }



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
                color: #fff !important;
            }


        }
    }

    /* Mobile responsive */

    @media screen and (max-width: 500px) {
        .hero div {
            width: 100% !important;

            h1 {
                font-size: 40px!important;
            }
        }

        .hero-image {
            display: none;
        }
        .jumbo {
            /*height: 100vh !important;*/
        }

    }

</style>