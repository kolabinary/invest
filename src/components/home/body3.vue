<template>
    <div class="container">
        <div class="holder">
            <div class="left" >
                <h1>Some of our investment options for you.</h1>
                <div>
                    <div style="display: flex;">
                        <img src="../../assets/body3-bullet.svg" alt="">
                        <h2>Treasury Bills</h2>
                    </div>

                    <p>Treasury Bills are short-term debt instruments issued by the Federal Government through the Central Bank to
                        provide short term funding for the government. They are by nature, the most liquid money market
                        securities and are backed by the guarantee of the Federal Government.</p>
                </div>
                <div>
                    <div style="display: flex;">
                        <img src="../../assets/body3-bullet.svg" alt="">
                        <h2>Eurobonds</h2>
                    </div>

                    <p>Eurobonds are investments issued in a currency not native to the issuer’s home country.
                        Eurobonds are commonly issued by governments, companies, and international organizations..</p>
                </div>
                <div>
                    <div style="display: flex;">
                        <img src="../../assets/body3-bullet.svg" alt="">
                        <h2>Equities</h2>
                    </div>

                    <p>Equities are stocks and shares issued by a company that carries no fixed interest.
                        The i-invest equities service is provided by PSL Capital Limited - a registered member of
                        the Nigerian Stock Exchange.</p>
                </div>
            </div>
            <div class="right">
                <img src="../../assets/body3-img.svg" alt="">
            </div>
        </div>

    </div>

</template>

<script>
export default {
  name: 'body3'

}
</script>


<style lang="scss" scoped>

    .container {
        background-color: #8F5EAB;
        padding: 2% 5%;

        .holder {
            display: flex;
            padding: 1rem 0;
        }
        /*.holder > div {*/
            /*width: 50%;*/
        /*}*/

        .right{
            width: 60%;
            img {
                width: 700px;
                text-align: center;
                margin: 0 auto;
                display: block;
                margin-top: 4rem;
            }

        }

        .left {
            width: 40%;
            color: #fff;

            p {
                font-size: 18px;
                letter-spacing: 0.5px;
                margin-top: 0;
            }
            h1 {
                font-size: 45px;
                font-weight: bolder;
            }
            h2 {
                font-weight: 800;
            }
            img {
                margin-right: 1rem;
                width: 25px;
            }
        }
    }

    @media screen and ( max-width: 500px){
        .left {
            width: 100% !important;
            h1 {
                font-size: 30px!important;
            }
            p {
                font-size: 16px !important;
                line-height: 1.5;
                opacity: 0.8;
                font-weight: 300;
            }
        }
        .right {
            display: none;
            /*img {*/
                /*display: none !important;*/
            /*}*/
        }
    }
</style>
