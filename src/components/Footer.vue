<template>
  <footer>
      <div class="background">
        <div class="top-footer">
          
            <div class="left-box">
                <div v-for="(link, index) in links" :key="index">
                    <h2>{{link.title}}</h2>
                    <ul>
                        <li v-for="(subtitle, index) in link.text" :key="index">
                            <a href="">{{ subtitle }}</a>
                        </li>
                    </ul>
                    <!-- <h2>DC COMICS</h2>
                        <ul>
                            <li>
                                <a href="">2</a>
                            </li>
                        </ul> -->
                </div>
                <!-- <div class="col-2">
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>
                            <a href="">3</a>
                        </li>
                    </ul>
                </div>
                <div class="col-3">
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>
                            <a href="">4</a>
                        </li>
                    </ul>
                </div> -->

            </div>

            <div class="right-box">
                
            </div>
        </div>
      </div>

      <div class="bottom-footer">
          <div class="bottom-box">
              <button class="btn">sign-up now!</button>
              <div class="social">
                  <h2>follow us</h2>
                  <ul> 
                    <li v-for="(icon, index) in icons" :key="index">
                        <a href=""><img :src="icon.icon" alt=""></a>
                    </li>
                  </ul>
              </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            links : [
                {
                    title: 'DC COMICS',
                    text: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                },
                                {
                    title: 'SHOP',
                    text: ['Shop DC', 'Shop DC Collectibles']
                },
                                {
                    title: 'DC',
                    text: ['Terms Of Use', 'Privacy policy(NEW)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },                {
                    title: 'SITES',
                    text: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                }
            ],
            icons : [
                { icon : '../assets/footer-facebook.png' },
                { icon : '../assets/footer-twitter.png' },
                { icon : '../assets/footer-youtube.png' },
                { icon : '../assets/footer-pinterest.png' },
                { icon : '../assets/footer-periscope.png' },
            ],
        }
    }
}
</script>

<style scoped>

    .background {
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;

    }    

    .top-footer {
        display: flex;
        width: 1270px;
        margin: 0 auto;
        padding: 65px;
        background-image: url('../assets/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position-x: right;
        background-position-y: -100px;
    }

    .left-box {
        flex-basis: 30%;
    }

    .right-box {
        flex-basis: 60%;

    }

    .left-box {
        display: flex;
        flex-direction: column;
        max-height: 300px;
        justify-content: space-between;
        flex-wrap: wrap;
    }

    .left-box h2 {
        margin: 10px 0px;
        color: #fff;
    }

    .left-box ul {
        list-style: none;
    }

    .left-box ul li a {
        color: #808080;
        text-decoration: none;
        font-size: 13px;
    }

    .bottom-footer {
        background-color: #303030;
        height: 150px;
    }

    .bottom-box {
        width: 1270px;
        margin: 0 auto;
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 40px;
    }

    .bottom-box .btn {
        padding: 15px 20px;
        background: none;
        outline: none;
        border: 2px solid #0282f9;
        color: #fff;
        text-transform: uppercase;
        font-size: 1rem;
        font-weight: bold;
        cursor: pointer;
    }

    .bottom-box .social {
        display: flex;
        
    }

    .bottom-box .social h2 {
        text-transform: uppercase;
        letter-spacing: 3px;
        color: #0282f9;
        margin-right: 20px;
    }

    .bottom-box .social ul li {
        display: inline-block;
        margin: 0 10px;
        cursor: pointer;
    }

</style>