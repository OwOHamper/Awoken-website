<template>
    <div class="person">
        <div class="person-image">
            <img class="person-img" :src="image" alt="person image">
        </div>
        <div class="person-info">
            <h2>{{name}}</h2>
            <p>{{description}}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        name: String,
        description: String,
        image: String
    }

}
</script>

<style scoped>
    .person {
        width: 800px;
        height: 300px;
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
        /* border: 1px solid black; */
    }

    .person-info {
        color: rgb(226, 226, 226);
        width: 200px;
        text-shadow: rgba(0, 0, 0, 0.25) 2px 2px 3px;
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
</style>