<template>
  <div class="hero">
        <div class="hero-left">
            <p class="title-text">Awoken</p>
            <p class="subtitle-text">A click and point video game that was created as a submission to <a href="https://smnd.sk/mikey/PHP/spongia/spongia_2023/index.php">Špongia 2023</a>.</p>
            <div class="button-div">
                <RouterLink to="/play" custom v-slot="{ navigate }">
                    <button class="red-button" @click="navigate" role="link">Play Now</button>
                </RouterLink>
            </div>
        </div>

        <div class="right">
            <div class="image-div">
                <img id="anchor" class="hero-image" src="/hero.png">
                <!-- <img id="eye" class="eye" src="Assets/hero-icon-eye.png" style="top: 120px;left: 120px;"> -->
            </div>
        </div>

    </div>
</template>

<style scoped>

.hero {
    margin-top: 50px;
    display: flex;
    justify-content: space-around;
    /* align-items: center; */
    /* height: 100vh; */

    /* color: white; */
    /* border: solid 1px black; */
}

@media screen and (max-width: 950px) {
    .hero {
        flex-direction: column;
        align-items: center;
    }
    /* align center */
    .red-button {
        margin-left: 0;
        margin-top: 0; 
    }

    .button-div {
        display: flex;
        justify-content: center;
        align-items: center;
       
    }
    .title-text {
        text-align: center;
    }
    .subtitle-text {
        text-align: center;
    }

    .right {
        margin-top: 100px;
    }
    /* .subtitle-text.letters { */
    /* word-wrap: break-word; */
/* } */
}
@media screen and (max-width: 600px) {
 .subtitle-text {
    height: 50px;
 }
}

a {
    white-space: pre;
}

.hero-left {
    margin-top: 100px;
    width: 650px;
}

@media screen and (max-width: 700px) {
    .hero-left {
        width: 80%;
    }
}

.title-text {
    font-size: 4rem;
    font-weight: 900;
    color: var(--red);
    margin-bottom: 26px;
}

.subtitle-text {
    font-size: 1rem;
    font-weight: 200;
    color: var(--red);
}

.right {
    width: 25%;
    /* height: 600px; */
    /* border: solid 1px black; */
}

@media screen and (max-width: 1100px) {
    .right {
        width: 275px;
    }
}

.image-div {
    display: flex;
    justify-content: center; /* Center horizontally */
    align-items: center; /* Center vertically */
    height: 100%;
    width: 100%;
    /* display: flex; */
    /* justify-content: center; */
    /* align-items: center; */
    /* align-items: center; */
    /* position: relative; */

}

.hero-image {
    /* margin-top: 100px; */
    /* display: block; */
    /* margin-left: auto; */
    margin: 0 auto;
    width: 100%;
    /* position: absolute; */
}



.eye {
    width: 350px;
    /* position: absolute; */
}





/* CSS */


    /* transition */
    .play-now {
        transition: all 0.2s ease-in-out;
    }
</style>