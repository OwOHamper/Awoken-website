<template>
  <main>
    <div class="text-div">
      <p>Watch trailer</p>
    </div>

    <div class="video">
        <iframe class="responsive-iframe" src="https://www.youtube.com/embed/bD5X31YCS6w?si=M4vJzPmvHgKKxuzJ"
        title="YouTube video player" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen></iframe>
    </div>
  </main>
</template>


<style scoped>

iframe {
  width: 960px;
  height: 540px;
}

@media screen and (max-width: 1000px) {
  iframe {
    width: 640px;
    height: 360px;
  }
}

@media screen and (max-width: 700px) {
  iframe {
    width: 480px;
    height: 270px;
  }
}

@media screen and (max-width: 500px) {
  iframe {
    width: 320px;
    height: 180px;
  }
}

.video {
    margin-top: 0px;
    text-align: center;
}

.text-div {
    margin-top: 100px;
    text-align: center;
}

p {

    display: inline-block;
    font-size: 3rem;
    font-weight: 800;
    color: var(--red)
    
}


</style>