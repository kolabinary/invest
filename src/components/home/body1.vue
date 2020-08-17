<template>
    <div class="container">
        <div class="text">
            <h1><Span style="color: #8F5EAB">Investment</Span> anywhere, anytime.</h1>
            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
                invidunt ut labore et dolore magna aliquyam
            </p>
        </div>

        <div class="cards">
            <div class="card1">
                <div style="display: flex; justify-content: space-between;">
                    <h3>We are
                        Risk Free</h3>
                    <img src="../../assets/risk-free.svg" alt="Risk free icon" height="65">
                </div>
                <p>Be rest assured that not only is your money safe but it will yield returns. Treasury bills are issued by the CBN,
                    making them an assurement investment option while Eurobonds are commonly issued
                    by the government, companies, and international organizations.</p>
            </div>
            <div class="card2">
                <div style="display: flex; justify-content: space-between;">
                    <h3>Invest
                        Anywhere</h3>
                    <img src="../../assets/anywhere.svg" alt="invest anywhere icon" height="65">
                </div>
                <p>With the I-invest App you can save and invest in Treasury Bills and Eurobonds from anywhere in the world
                    right from your mobile device. This makes it the easiest and fastest way to invest in these instruments.
                </p>

            </div>
            <div class="card3">
                <div style="display: flex; justify-content: space-between;">
                    <h3>Invest
                        anytime</h3>
                    <img src="../../assets/anytime.svg" alt="invest anytime icon" height="65">
                </div>
                <p>I-invest app is available to you 24/7. Open up your app at any time of the day and
                    invest in Treasury Bills and Eurobonds.
                </p>
            </div>
        </div>
    </div>

</template>



<script>
export default {
  name: 'body1'

}
</script>



<style lang="scss" scoped>

    .container {
        background-color: #FCFAFD;
        padding: 2% 5%;
       .text {
           h1 {
               text-align: center;
               font-size: 40px;
               margin-bottom: 0.5rem;
           }
           p {
               text-align: center;
               max-width: 58ch;
               margin: 0 auto;
               color: #8D8194;
               font-size: 16px;
               margin-bottom: 2rem;
           }
       }
        .cards {
            display: flex;
            justify-content: space-between;
            margin: 3rem 0;

            h3 {
                font-size: 35px;
                max-width: 8ch;
                color: #311342;
            }
            p {
                max-width: 40ch;
                font-size: 16px;
                letter-spacing: 1px;
                color: #61516A;
                /*font-weight: 400;*/
                /*text-align: justify;*/
            }

            img {
                margin-top: 3rem;
            }
            .card1 {
                /*margin-right: 1rem;*/
                background-color: #fff;
                background-image: url('../../assets/risk-free-bg.svg');
                background-repeat: no-repeat;
                background-size: 33%;
                background-position: bottom right;
            }
            .card2 {
                background-color: #fff;
                background-image: url('../../assets/anywhere-bg.svg');
                background-repeat: no-repeat;
                background-size: 100%;
            }

            .card3 {
                background-color: #fff;
                background-image: url('../../assets/anytime-bg.svg');
                background-repeat: no-repeat;
                background-size: 100%;
            }
        }

        .cards > div {
            width: 25%;
            background-color: #fff;
            padding: 1.5rem 2rem 3.5em 2em;
            border-radius: 8px;
            box-shadow: 5px 5px 15px rgba(49,19,66,0.04),
                        5px 25px 50px rgba(49,19,66,0.04),
                        5px 30px 40px rgba(49,19,66,0.06);
        }

    }

</style>
