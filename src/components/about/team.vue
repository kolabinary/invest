<template>
    <div class="container">

        <h1>Meet our team</h1>
        <div class="team-holder">
            <div class="teams">
                <img src="../../assets/team1.jpg" alt="" height="200">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>

            </div>
            <div class="teams">
                <img src="../../assets/team1.jpg" alt="" height="200">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>

            </div>
            <div class="teams">
                <img src="../../assets/team2.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>

            </div>
            <div class="teams">
                <img src="../../assets/team1.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>

            </div>
            <div class="teams">
                <img src="../../assets/team1.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>
            </div>
            <div class="teams">
                <img src="../../assets/team3.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>
            </div>
            <div class="teams">
                <img src="../../assets/team1.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>
            </div>
            <div class="teams">
                <img src="../../assets/team2.jpg" alt="" height="150">
                <h4>Jane Doe</h4>
                <span style="color:#833FAB">Operations</span>
                <div class="links">
                    <a href=""><img src="../../assets/insta1.svg" alt=""></a>
                    <a href=""><img src="../../assets/twitter1.svg" alt=""></a>
                    <a href=""><img src="../../assets/facebook1.svg" alt=""></a>
                </div>
            </div>

        </div>

        <hr>
        <section>
            <h2>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
                invidunt ut labore et dolore magna
            </h2>
            <p>
                Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
                aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea
                takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur
            </p>
        </section>
    </div>

</template>



<script>
export default {
  name: 'team'

}
</script>



<style lang="scss" scoped>
    @import '../../css/main.css';

    .container {

        hr {
            width: 60%;
            opacity: 0.4;
        }

        padding: 5% 5%;
        h1 {
            text-align: center;
            font-size: 35px;
            margin: 5rem 0;
            color: #311342;
        }

        section {
            color: #311342;
           h2 {
               padding-top: 4rem;
               max-width: 55ch;
               margin: 0 auto;
               text-align: center;

           }
            p {
                max-width: 100ch;
                padding-top: 2rem;
                margin: 0 auto;
                text-align: center;
                opacity: 0.7;
            }
        }
        .team-holder {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 0 3%;
        }
        .team-holder > div {
         width: 20%;

        }
        .teams:nth-child(4),.teams:last-child {
            margin-right: 0;
        }

        .teams {
            text-align: center;
            margin-right: 4rem;
            margin-bottom: 6rem;

            span {
                font-weight: 300;
            }

            .links {
                margin-top: .7rem;
                a {
                    margin-right: 1rem;
                    img {
                        height: 20px;
                    }
                }
            }

            h4 {
                font-size: 25px;
                margin: 0;
                color: #311342;
            }

        }
        .teams > img {
            border-radius: 50%;
            height: 180px;
        }

    }

    @media screen and (max-width: 500px){
        .team-holder > div {
            width: 50% !important;

        }
        .teams {
            margin-right: 0 !important;
        }

        .teams > img {
            height: 130px!important;
        }
    }

</style>
