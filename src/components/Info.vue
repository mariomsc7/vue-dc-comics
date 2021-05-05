<template>

<div class="background">
      <div class="container">
      
      <ul>
          <li v-for="(info, index) in images" :key="index">
              <span>
                <img :src="info.img" alt="">
              </span>
              <a href="">{{info.text}}</a>
          </li>

          
      </ul>
  </div>
</div>

</template>

<script>
export default {
    name : 'Info',
    data() {
        return {
            images: [

               { img: '../assets/buy-comics-digital-comics.png',
                 text: 'digital comics'
               },
               { img: '../assets/buy-comics-merchandise.png',
                 text: 'dc merchandise'
               },
                { img: '../assets/buy-comics-shop-locator.png',
                 text: 'subscription'
               },
                { img: '../assets/buy-comics-subscriptions.png',
                 text: 'comic shop locator'
               },
                { img: '../assets/buy-dc-power-visa.svg',
                 text: 'dc power visa'
               },
    
            ],
        }
    }
}
</script>

<style scoped>

    .background {
        background: #0282f9;
    }

    .container {
        max-width: 1270px;
        margin: 0 auto;
        padding: 3rem;
        
    }

    ul {
        display: flex;
        list-style: none;
        justify-content: space-between;
    }

    ul li {
        display: flex;
        align-items: center;
    }

    ul li a {
        text-decoration: none;
        color: #fff;
        margin-left: 10px;
        text-transform: uppercase;
    }

    ul li span img {
        
        width: 48px;
    }
</style>