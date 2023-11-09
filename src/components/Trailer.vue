<template>
  <main>
    <div class="text-div">
      <p>Watch trailer</p>
    </div>

    <div class="video">
        <iframe width="960" height="540" src="https://www.youtube.com/embed/bD5X31YCS6w?si=M4vJzPmvHgKKxuzJ"
        title="YouTube video player" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen></iframe>
    </div>
  </main>
</template>


<style scoped>

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