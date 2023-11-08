<template>
    <main>
        <p style="display:block">You can download the windows build here (Submitted version):</p>
        <a href="https://drive.google.com/drive/u/0/folders/1U1AOMdeBNcZOVHVIAYzxHdaxIGA9i1iu">
            <button class="red-button blue">Download (Google Drive)</button>
        </a>
        <ul>
            <li>
                <p><strong>•</strong> Download <strong>Build.zip</strong></p>
            </li>
            <li>
                <p><strong>•</strong> Unzip and run <strong>Awoken.exe</strong></p>
            </li>
        </ul>
        <br>

        <p style="display:block">Or you can play the latest version directly in your browser:</p>
        <a href="https://play.awoken.sk/">
            <button class="red-button blue" type="button">Play Online</button>
        </a>

        <br>
        <!-- <iframe src="https://spongia.hamper.dev" style="border:2px dotted #000000;" name="Awoken" scrolling="no" frameborder="1" marginheight="px" marginwidth="320px" height="720px" width="1280px"></iframe> -->
        <br>
        <br>
        <br>
    </main>
</template>

<script>
export default {

}
</script>

<style scoped>
    main {
        margin-top: 20px;
        text-align: center;
        /* display: flex; */
        /* justify-content: center; */
        /* align-items: center; */
        /* height: 100vh; */
    }

    p {
        display: inline-block;
        font-size: 1.5rem;
        font-weight: 500;
        color: var(--red);
        margin: 10px;
        
    }

    .blue {
        background-color: var(--blue);
    }

    .blue:active {
      box-shadow: var(--blue) 0 5px 20px -10px;
    }

    ul {
        list-style-type: none;
    }


</style>