<template>

    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            
            <nav>
                <ul class="nav-list">
                    <li v-for="(link, index) in links" :key="index"> 
                        <a href="">{{ link.text }}</a> 
                    </li>

                </ul>
            </nav>
        </div>
    </header>
    
</template>

<script>
export default {
    name : 'Header',
    data() {
        return {
            links : [
                {text : 'characters'},
                {text : 'comics'},
                {text : 'movies'},
                {text : 'tv'},
                {text : 'games'},
                {text : 'collectibles'},
                {text : 'videos'},
                {text : 'fans'},
                {text : 'news'},
                {text : 'shop'},
            ]
        }
    }
}
</script>

<style scoped>

    header {
        margin-top: 30px;
    }

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 1270px;
        margin: 0 auto;
        height: 100px;
        padding-bottom: 25px;
        
    }

    .logo img {
        width: 80px;
    }
    
    .nav-list {
        display: flex;
        list-style: none;
    }

    .nav-list li a {
        padding: 37px 16px;
        text-decoration: none;
        text-transform: uppercase;
        font-size: 1rem;
        font-weight: bold;
        transition: color .2s;
        color: #000;
    }

    .nav-list li a:hover {
        color: dodgerblue;
        border-bottom: 3px solid dodgerblue;
    }
    
    
</style>