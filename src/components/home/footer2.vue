<template>
    <footer class="container">

        <div class="foot-flex">
            <div class="links">
                <div>
                    <h2>Company</h2>
                    <ul>
                        <li>About Us</li>
                        <li>FAQs</li>
                        <li>Stories</li>
                    </ul>
                </div>
                <div>
                    <h2>Products</h2>
                    <ul>
                        <li>EuroBonds</li>
                        <li>Treasury Bills</li>
                        <li>Equities</li>
                        <li>Features</li>
                    </ul>
                </div>
                <div>
                    <h2>Legal</h2>
                    <ul>
                        <li>Privacy Policy</li>
                        <li>Terms of Use</li>
                        <!--<li>Stories</li>-->
                    </ul>
                </div>
            </div>
            <div class="social">
                <h2>The Social Plug</h2>
                <a href=""><img src="../../assets/instagram.svg" alt=""></a>
                <a href=""><img src="../../assets/twitter.svg" alt=""></a>
                <a href=""><img src="../../assets/facebook.svg" alt=""></a>
                <a href=""><img src="../../assets/youtube.svg" alt=""></a>

            </div>

            <hr>
            <div class="address">
                <a href=""><img src="../../assets/logo.svg" alt="" height="50"></a>
                <p class="address-office">22a Udi Street, Osborne Foreshore, Ikoyi, Lagos</p>
                <a href="tel:+23419037095">+ 234 1 903 7095</a>
                <a href="tel:+2348075290008">+ 234 807 529 0008</a>
                <a href="mailto:">info@i-investng.com</a>
                <a href="mailto:">enquiries@i-investng.com</a>

            </div>
        </div>
        <hr>
        <div class="last">
            <p>i-invest is a mobile application which allows current and aspiring investors purchase securities and
                other related instruments without the aid of a broker. In addition, the application provides a UI
                dashboard to track diverse investment portfolios, provides a convenient way for retail investors to
                save money whilst earning attractive interest rates, and allowing retail investors to help fund
                infrastructure projects in Nigeria whilst earning an income.
            </p>
        </div>

    </footer>

</template>

<script>
export default {
  name: 'footer2'

}
</script>


<style lang="scss" scoped>

    @import '../../css/main.css';

    .container {

        padding: 2% 8%;
        background: url('../../assets/footer-bg.svg');
        background-repeat: no-repeat;
        background-size: 120%;
        background-position: 20% -300%;

        h2 {
            font-size: 1px;
        }

        .last {
            margin-top: 5rem;

            p {
                color: #776382;

            }
        }

        .links {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;

            ul {
                list-style: none;
                padding: 0;

                li {
                    margin-bottom: 1rem;
                    font-weight: 500;
                    font-size: 15px;
                    color: #776382;
                }
            }
        }

        .social {

            a {
                margin-right: 1rem;
                img {
                    width: 28px;
                    height: 28px;
                }
            }
        }

        .foot-flex > div {
            width: 30%;
        }



        .foot-flex {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            color: #311342;

            .address {
                text-align: right;
                .address-office {
                    text-align: right;
                    font-size: 18px;
                }
                a {
                    display: block;
                    text-decoration: none;
                    font-size: 15px;
                    font-weight: 500;
                    color: #776382;
                    margin-bottom: 0.5rem;
                    transition: all 0.5s ease-in-out;
                }
                a:hover {
                    color: #311342;
                    font-weight: 700;

                }


                p {
                    font-size: 15px;
                    font-weight: 500;
                }

            }
        }

    }



    @media screen and (max-width: 500px) {
    .foot-flex > div {
        width: 100% !important;
        margin-bottom: 2rem;

    }
        .address {
            margin-bottom: 0!important;
            text-align: left !important;
            p {
                text-align: left !important;
            }

        }

        hr {
            opacity: 0.7;
        }

        .last {
            margin-top: 1rem !important;

            p {
                line-height: 1.5;
                font-size: 16px;
                opacity: 0.7;

            }
        }
    }
</style>
