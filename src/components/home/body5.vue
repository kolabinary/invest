<template>
    <div class="container">
        <h1>Amazing Stories</h1>
            <section class="main">
                <div class="story-holder">
                    <p>
                        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
                        labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
                        Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet,
                        consetetur sadipscing
                    </p>
                    <h3 style="">-Olofin Aderonke</h3>
                    <a href="">More Amazing Stories</a>
                    <img class="story-img" src="../../assets/story-img.png" alt="">

                </div>

            </section>

    </div>

</template>

<script>
export default {
  name: 'body5'

}
</script>


<style lang="scss" scoped>

    .container {
        /*background-color: #FCFAFD;*/
        padding: 2% 0;
        background: url('../../assets/stories-bg.svg');
        background-repeat: no-repeat;
        background-position: -15% -20%;
        background-size: 35%;
        
        h1 {
            text-align: center;
            font-size: 42px;
            margin-bottom: 0;
        }

        .main {
            padding: 3% 5% 3% 25%;

            /*background: url('../../assets/stories-bg.svg');*/
            /*background-repeat: no-repeat;*/
        }
        
        .story-holder {
            position: relative;
            background: url('../../assets/story-text-bg.svg');
            background-repeat: no-repeat;
            background-color: #EFE4F5;
            background-size: 40%;
            width: 60%;
            padding: 3rem 6rem 5rem 12rem;
            border-radius: 10px;

            .story-img {
                position: absolute;
                width: 350px;
                top: 50px;
                left: -250px;
                filter: drop-shadow(0 10px 13px rgba(0,0,0,0.3));
                /*box-shadow: 5px 5px 15px rgba(49,19,66,0.04),*/
                /*5px 25px 50px rgba(49,19,66,0.04),*/
                /*5px 30px 40px rgba(49,19,66,0.2);*/
            }

            h3 {
                font-weight: 700;
                /*display: block; */
                font-size: 18px;
                margin-bottom: 2rem;
            }
            
            a {
                color: #fff;
                background-color: #401857;
                border-radius: 6px;
                padding: 1rem 1rem;
                text-decoration: none;
                font-weight: 700;
                font-size: 14px;

            }

            p {
                font-weight: 500;
                color: #311342;
                max-width:60ch ;
                line-height: 1.6;
                font-size: 22px;
            }
        }

    }
</style>
