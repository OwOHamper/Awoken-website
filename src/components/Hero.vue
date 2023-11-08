<template>
  <div class="hero">
        <div class="hero-left">
            <p class="title-text">Awoken</p>
            <p class="subtitle-text">A click and point video game that was created as a submission to <a href="https://smnd.sk/mikey/PHP/spongia/spongia_2023/index.php">Špongia 2023</a>.</p>
            <RouterLink to="/play" custom v-slot="{ navigate }">
                <button class="red-button" @click="navigate" role="link">Play Now</button>
            </RouterLink>
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
    margin-top: 100px;
    display: flex;
    justify-content: space-around;
    /* align-items: center; */
    /* height: 100vh; */

    /* color: white; */
    /* border: solid 1px black; */
}

.hero-left {
    margin-top: 100px;
    width: 650px;
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
    width: 400px;
    height: 600px;
    /* border: solid 1px black; */
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
    width: 350px;
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