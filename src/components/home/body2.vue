<template>
    <div class="container">
        <div class="holder">
            <div class="step-img">
                <img src="../../assets/create.png" alt="" height="700">
            </div>
            <div class="details">
                <h3>Investing on i-invest in 4 easy steps</h3>

                <div class="steps">
                    <div class="step-list">
                        <span class="step-num"></span>
                        <div class="step-list-content">
                            <span class="title" style="display: block;">Create a free Account</span>
                            <span class="lines">Register by enter your personal details. </span>

                        </div>
                    </div>

                    <div class="step-list">
                        <span class="step-num"></span>
                        <div class="step-list-content">
                            <span class="title" style="display: block;">Fund your wallet</span>
                            <span class="lines">Log into your account and fund your wallet using a debit
                                card from any bank or online transfer.
                            </span>

                        </div>
                    </div>

                    <div class="step-list">
                        <span class="step-num"></span>
                        <div class="step-list-content">
                            <span class="title" style="display: block;">Fund your wallet</span>
                            <span class="lines">Log into your account and fund your wallet using a debit
                                card from any bank or online transfer.
                            </span>

                        </div>
                    </div>


                </div>
            </div>
        </div>

    </div>

</template>

<script>
export default {
  name: 'body2'

}
</script>


<style lang="scss" scoped>

    body {
        counter-reset: section;
    }

    .container {
        padding: 2% 5%;

        .holder {

            counter-reset: item;
            display: flex;
            justify-content: space-between;


            .details {
                padding: 2% 10%;
            }

            .step-img {
                background: url('../../assets/step-bg.svg');
                /*-webkit-background-size:100%;*/
                background-size:75% ;
                background-repeat: no-repeat;
                background-position: 50% 50%;
            }


            h3 {
                font-size: 35px;
            }
            .step-num::before {

            }
            .step-num::after {
                counter-increment: item;
                content: "0" counter(item);
                font-weight: 700;
                color: #8F5EAB;
                font-size: 20px;
            }

            .step-list {
                display: flex;
                justify-content: flex-start;
                align-items: flex-start;
                position: relative;
                margin-bottom: 50px;
                .title {
                    font-weight: 700;
                    font-size: 25px;
                    color: #8F5EAB;
                }


            }
            .step-list:before {
                content: "";
                width: 1px;
                position: absolute;
                background-color: #8F5EAB;
                top: 50px;
                opacity: 1;
                left: 12px;
                height: 80%;
                transition: height .8s ease-out;
            }
            .step-list:last-child:before{content:none}
            .step-list-content {
                margin-left: 35px;
            }

        }

        .holder > div {
            width: 50%;
        }
    }


    @media screen and (max-width: 500px) {
        .holder > div {
            width: 100% !important;

            img {
                height: 300px;
            }
        }

        .details h3 {
            color: #311342;
        }

        .holder {
            flex-wrap: wrap;
        }
        .step-img {
            img {
                height: 530px !important;
                margin: 0 auto;
                display: block;
            }
        }

        .lines {
            font-size: 16px;
            line-height: 1.5;
            opacity: 0.7;
            letter-spacing: 0.5px;
        }



    }


</style>
