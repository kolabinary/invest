<template>
    <div class="container">
        <h1>Videos that may help.</h1>
        <div class="holder">
            <div class="left" >
                <iframe width="520" height="345" src="https://www.youtube.com/embed/zqnmaV3OD60">
                </iframe>
            </div>
            <div class="right">
                <iframe width="520" height="345" src="https://www.youtube.com/embed/skoXPRQfJD4">
                </iframe>
            </div>
        </div>

    </div>

</template>

<script>
export default {
  name: 'body4'

}
</script>


<style lang="scss" scoped>

    .container {
        background-color: #FCFAFD;
        padding: 3% 5%;
        h1 {
            text-align: center;
            font-size: 45px;
            color: #311342;
        }

        .holder {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 2rem 0;
            .right {
                margin-left: 2rem;
            }
        }

        iframe {
            border-radius: 10px;
            border: none;
        }


    }

    @media screen and (max-width: 500px) {

       .container {
           h1 {
               font-size: 30px;
           }
       }
        iframe {
            width: 320px;
        }

        .right {
            margin-left: 0!important;
        }
    }
</style>
