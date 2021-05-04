<template>
  <div class="container">
      
      <ul>
          <li>
              <span>
                <img src="../assets/buy-comics-digital-comics.png" alt="">
              </span>
              <a href="">digital comics</a>
          </li>
          <li>
              <span>
                <img src="../assets/buy-comics-digital-comics.png" alt="">
              </span>
              <a href="">digital comics</a>
          </li>
          
      </ul>
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
                 text: 'digital comics'
               },
                { img: '../assets/buy-comics-shop-locator.png',
                 text: 'digital comics'
               },
                { img: '../assets/buy-comics-subscriptions.png',
                 text: 'digital comics'
               },
                { img: '../assets/buy-dc-power-visa.svg',
                 text: 'digital comics'
               },
    
            ],
        }
    }
}
</script>

<style scoped>
    .container {
        max-width: 1270px;
        margin: 0 auto;
        padding: 3rem;
        background-color: #888;
    }

    ul {
        display: flex;
        list-style: none;
        justify-content: space-between;
    }

    ul li a {
        text-decoration: none;
        color: #fff;
        margin-left: 10px;
        text-transform: uppercase;
    }

    ul li span img {
        vertical-align: middle;
        width: 48px;
    }
</style>