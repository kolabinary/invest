<template>
    <div class="container">
        <div class="jumbo">
            <nav class="nav">
                <div class="logo"><img src="../assets/logo.svg" alt="" height="40"></div>
                <div class="link-up">
                    <a href="">About</a>
                    <a href="">FAQs</a>
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


    </div>
</template>

<script>
    export default {
        name: 'home'
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
        }
        .hero {
            display: flex;
            margin-top: 30px;



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
                color: #fff;
            }
        }
    }


</style>