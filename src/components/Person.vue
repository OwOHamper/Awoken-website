

<template>
    <div class="person">
        <div class="person-image">
            <img class="person-img" :src="'/' + image" alt="person image">
        </div>
        <div class="person-info">
            <div class="name-div">
                <h2>{{name}}</h2>
            </div>
            <div class="description-div">
                <p>{{description}}</p>
            </div>
            <div  class="social-div">
                <a v-if="github != null" :href="'https://github.com/' + github">
                    <i class="fa-brands fa-github" :title="'@' + github"></i>
                </a>
                <a v-if="website != null" :href="'https://' + website">
                    <i class="fa-solid fa-earth-americas" :title="website"></i>
                </a>
                <a v-if="instagram != null" :href="'https://www.instagram.com/' + instagram" >
                    <i class="fa-brands fa-instagram" :title="'@' + instagram"></i>
                </a>
                
                
            </div>
            
            
        </div>
    </div>
</template>

<script>
export default {
    props: {
        name: String,
        description: String,
        image: String,
        instagram: String,
        website: String,
        github: String
    }
}
</script>

<style scoped>
    .person {
        border: 1px solid rgb(0, 0, 0, 0.1);
        display: flex;
        flex-direction: space-between;
        padding-right: 20px;

        background: #535151;
        /* background: radial-gradient(circle at right, #535151 0%, #5a4a49 var(--x, 0)200%); */
        background: linear-gradient(90deg, #535151, #5a4a49 51%, #535151) var(--x, 0)/ 200%;
        /* background: #535151; */
        border-radius: 15px;
        box-shadow: rgba(99, 99, 99, 0.265) 0px 2px 8px 0px;

    }

    .person-image {
        padding: 10px 20px;
        
    }

    .person-img{
        border-radius: 50%;
        width: 100px;
        border: 1px solid rgba(55, 55, 55, 1) 
    }

    .person-info {
        color: rgb(226, 226, 226);
        width: 200px;
        /* height: 100px; */
        text-shadow: rgba(0, 0, 0, 0.25) 2px 2px 3px;

        display: flex;
        flex-direction: column;
        justify-content: space-between;
        gap: 10px;
    }



    /* .person:hover {
        background: #535151;
        background: radial-gradient(circle at right, #535151 50%, #5a4a49 100%);
        box-shadow: rgba(99, 99, 99, 0.265) 0px 2px 8px 0px;
    } */
    .person:hover { --x: 100%; }

    .person {
        transition: all 0.5s ease-in-out;
    }

    .name-div {
        /* border: 1px solid black; */
        margin-top: 10px;
        height: 30px;
        /* width: 60; */
    }

    .description-div {
        /* border: 1px solid black; */
        height: 35px;
    }

    .social-div {
        /* border: 1px solid black; */
        height: 20px;
        display: flex;
        justify-content: flex-end;
        margin-right: 10px;
        margin-bottom: 10px;
        gap: 15px;
        /* align-items: center; */
    }

    h2 {
        margin: 0;
        padding: 0;
    }

    p {
        margin: 0;
        padding: 0;
    }
</style>