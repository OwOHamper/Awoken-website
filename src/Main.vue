<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './components/Footer.vue'

</script>



<template>
    <main>
        <header>
            <div class="navbar">
                <div class="links">
                    <div class="link">
                        <RouterLink class="router-link" to="/">Home</RouterLink>
                    </div>
                    <div class="link">
                        <RouterLink class="router-link" to ="/play">Play</RouterLink>
                    </div>
                    <div class="link">
                        <RouterLink class="router-link" to="/about">About Us</RouterLink>
                    </div>
                    
                    
                    
                </div>
            </div>
        </header>
        <main>
            <RouterView />


        </main>
            
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>

        <footer>
            <Footer />
        </footer>
            
        <!-- <p1 class="test">Awoken</p1> -->
        

    </main>

</template>


<style scoped>

    .navbar {
        display: flex;
        justify-content: end;
        align-items: center;
        /* border: solid 1px black; */
        padding-top: 35px;
        height: 50px;
    }

    .links {
        width: 500px;
        display: flex;
        justify-content: space-around;
        margin-right: 7%;
        height: 100px;
        align-items: center;
    }
    /* if screen width is small */
    @media screen and (max-width: 600px) {
        .links {
            width: 80%;
            justify-content: space-around;
            margin-right: 5%;
            height: 100px;
            align-items: center;
        }
    }

    .link {
        height: 100px;
        width: 100%;
        align-content: center;
        display: flex;
        justify-content: center;
    }

    .router-link {
        color: #b1a8a3;
        text-decoration: none;
        font-size: 1.5rem;
        font-weight: 200;
        width: 100%;
        margin-top: 18px;
        text-align: center;
    }

    .router-link:hover {
        color: #c7a7a7;
        font-size: 1.8rem;
    }

    .router-link-active {
        font-size: 1.8rem;
        /* font-weight: 700; */
        color: #c7a7a7;
    }


    .router-link {
        transition: all 0.15s ease-in-out;
    }

    /* transition */
    
</style>