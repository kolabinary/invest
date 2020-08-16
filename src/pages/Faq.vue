<template>
    <div class="container">
        <div class="faq">
          <h1>Frequently asked questions</h1>
          <input type="text">
          <div class="fq-flex">
            <div class="fq-box">
              <img src="../assets/started icon.svg">
              <p>Getting Started</p>
            </div>
            <div class="fq-box">
              <img src="../assets/invest-icon.svg" style="width: 1rem">
              <p>Investing</p>
            </div>
            <div class="fq-box">
              <img src="../assets/security-icon.svg">
              <p>Safety &amp; Security</p>
            </div>
          </div>
        </div>
        <div class="g-blck">
          <div class="g-bbox bb1">
            <h2>Getting Started</h2>
          </div>
          <article class="message" :class="accordionClasses" >
            <div class="message-header" @click="toggleAccordion">
              <h3>What is i-invest?</h3>
              <p class="i">-</p>
            </div>
            <div class="message-body">
              <div class="message-content">
            <p>I-Invest is a mobile application designed to encourage people to build a savings and 
              investment culture. It provides a secure, fast and convinient way for the average man to 
              access investment products otherwise reserved for the elite.</p>
              </div>
              </div>

              <div class="message-header" @click="toggleAccordion">
              <h3>What do i need to Register?</h3>
              <p class="i">+</p>
            </div>

          </article>
        </div>
        <div>
        </div>
      </div>
</template>

<script>
export default {
  name: 'faq',
  data() {
    return{
        isOpen: true
}
},
methods: {
        toggleAccordion: function() {
          this.isOpen = !this.isOpen;
          if(this.isOpen === true){
            document.querySelector('.i').innerHTML="-"
          }else{
            document.querySelector('.i').innerHTML="+"
          }
          
        }
      },
      computed: {
        accordionClasses: function() {
          return {
            'is-closed': !this.isOpen,
            'is-primary': this.isOpen,
            'is-dark': !this.isOpen
          };
        }
      }
    
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
  color: #311342;
}
    .faq{
      height: 50vh;
      padding-bottom: 5%;
      text-align:center;
      background-image: url('../assets/faq-bg.svg');
      background-color: whitesmoke;
      margin:0;
      margin-top: 0;           
      padding-top: 5%;
      background-repeat: no-repeat;
      background-position-y: 70%;
      background-position-x: 65%;
      background-size: 140%;
}
    .faq h1{

      margin-bottom: .8rem;
      font-size: 1.8rem;
    }
    .faq input{
      width: 40%;
      height:3rem;
      border: none;
      margin-bottom: 3rem;
      border-radius: 5px;
      box-shadow: 4px 5px 20px -14px rgba(0,0,0,0.6);
    }
    /* .faq input:hover{
      border-style:solid;
      border-width:1px;
      border-image: linear-gradient(top, #8F5EAB, #ffffff);;
    } */
    .fq-flex{
      display: flex;
      justify-content: space-between;
      width:45%;
      margin: auto;
    }
    .fq-box{
      background-color: white;
      padding:.5rem;
      padding-top: 1.5rem;
      border-radius: 5px ;
      width: 9rem;
      height:5rem;
      box-shadow: 4px 5px 20px -14px rgba(0,0,0,0.6)
    }
    .fq-box p{
      font-size: .85rem;
      font-weight: bold;
    }
    .fq-box img{
      width:1.5rem;
      padding-bottom: 0;
      margin-bottom: 0;
    }
    .g-blck{
      width:78%;
      margin:auto;
      display: flex;
      padding-top: 9%;
    }
    .bb1{
      font-size: 1.2rem;
      margin-right: 10%;
    }
    .message{
      border-bottom: 1px solid rgba(248, 248, 248, 0.596);
    }
    .message-header h3{
      color:#8F5EAB;
      margin-bottom: 3%;
      font-size: 1.3rem;
      flex-basis: 70%;
    }
    .message p{
      font-size: .95rem;
      font-weight: 600;
      line-height: 22px;
      letter-spacing: 1.5px;
    }

.message-header {
    cursor: pointer;
    display: flex;
    justify-content: space-between;
      color:#8F5EAB;
}
.message-header p{
      color:grey;
      font-size: 1.5rem;
}

.message-body   {
    padding: 0;
    max-height: 10em;
    overflow: hidden;
    transition: 0.5s ease all;
}

.is-closed .message-body {
    max-height: 0;
}

</style>
