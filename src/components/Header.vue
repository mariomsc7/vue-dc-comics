<template>

    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            
            <nav>
                <ul class="nav-list">
                    <li> <a href="">characters</a> </li>
                    <li><a href="">comics</a></li>
                    <li><a href="">movies</a></li>
                    <li><a href="">tv</a></li>
                    <li><a href="">ganes</a></li>
                    <li><a href="">collectibles</a></li>
                    <li><a href="">videos</a></li>
                    <li><a href="">fans</a></li>
                    <li><a href="">news</a></li>
                    <li><a href="">shop</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
</template>

<script>
export default {
    name : 'Header'
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
        
    }

    .logo img {
        width: 80px;
    }
    
    .nav-list {
        display: flex;
        list-style: none;
    }

    .nav-list li a {
        padding: 32px 16px;
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