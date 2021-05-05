<template>
  <footer>
      <div class="background">
        <div class="top-footer">
          
            <div class="left-box">
                <div class="col-1">
                    <h2>DC COMICS</h2>
                    <ul>
                        <li v-for="(link, index) in links" :key="index">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>
                    <h2>DC COMICS</h2>
                        <ul>
                            <li>
                                <a href="">2</a>
                            </li>
                        </ul>
                </div>
                <div class="col-2">
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
                </div>

            </div>

            <div class="right-box">
                
            </div>
        </div>
      </div>

      <div class="bottom-footer"></div>
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
            ]
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
        height: 400px;
        padding: 40px;
        color: #fff;
    }

    .left-box {
        flex-basis: 30%;
    }

    .right-box {
        flex-basis: 70%;
    }

    .left-box {
        display: flex;
        justify-content: space-between;
    }

    ul {
        list-style: none;
    }


</style>