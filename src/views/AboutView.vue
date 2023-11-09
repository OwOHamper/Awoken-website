<script setup>
import Person from '../components/Person.vue'
import PersonBig from '../components/PersonBig.vue'
</script>

<template>
  <main>
    <h2>Team "Chorá Puma"</h2>
    <p>We are a group of <strong class="team-size">six</strong> high school student who are studying at <a href="https://www.galeje.sk/">Gymnázium Alejová 1, Košice.</a></p>
    <br>
    <p>Our team consists of:</p>

    <dir class="vertical-flexbox">
      <div class="horizontal-flexbox">
        <Person name="Teodor Barča" description="Python Programmer" image="hamper.png" instagram="9teodor" website="hamper.dev"
        github="OwOHamper" youtubeUrl="@OwOHamper" youtubeName="OwOHamper"/>
        <Person name="Michal Petričko" description="C enthusiast" image="l33t.png"/>
        <Person name="Michal Katriňák" description="Artist/Designer" image="michaldo.png"/>
      </div>
      <div class="horizontal-flexbox">
        <Person name="Abigail Beblavá" description="Artist" image="abby.png"/>
        <Person name="Oliver Seman" description="Programmer" image="oliver.png"/>
        <Person name="Kristián Ohman" description="Music composer" image="tinky.png" spotifyUrl="2o910s2uauvav9o900rua8t7z"
        spotifyName="Tinkydakiko" soundcloudUrl="getcha_records" soundcloudName="Getcha Records" appleUrl="sk/artist/tinky/1706677480" appleName="Tinky"
        youtubeUrl="@getcha.records" youtubeName="Getcha Records" />
      </div>

    <!-- <div class="persons-div">
      <PersonBig name="Teodor Barča" description="Python enjoyer" image="starosta.png"/>
      <PersonBig name="Michal Petričko" description="C enthusiast" image="starosta.png"/>
      <PersonBig name="Michal Katriňák" description="Artist" image="starosta.png"/>
      <PersonBig name="Abigail Beblavá" description="Artist" image="starosta.png"/>
      <PersonBig name="Oliver Seman" description="Programmer" image="starosta.png"/>
      <PersonBig name="Kristián Ohman" description="Music composer" image="starosta.png"/>
    </div> -->

    </dir>
  </main>

</template>

<style scoped>
    main {
        /* margin-top: 0px; */
        text-align: center;
        /* display: flex; */
        /* justify-content: center; */
        /* align-items: center; */
        /* height: 100vh; */
    }

    h2 {
        /* background: #B48484; */
        font-size: 3rem;
        font-weight: 700;
        background: #B48787;
        background: -webkit-linear-gradient(to right, #B48787 0%, #6B77B5 100%);
        background: -moz-linear-gradient(to right, #B48787 0%, #6B77B5 100%);
        background: linear-gradient(to right, #B48787 0%, #6B77B5 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        
    }
    .team-size {
      color: rgb(193, 168, 168)
    }

    p {
        display: inline-block;
        font-size: 1.5rem;
        font-weight: 500;
        color: var(--red);
        
    }

    .vertical-flexbox {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 50px;
    }

    .horizontal-flexbox {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      gap: 150px;
    }

    /* .persons-div {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: start;
      gap: 50px;
      left: 0px;
    } */

</style>
