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
        <div class="p-div" >
        <p>
        Our game is a simple point-and-click adventure game.
It's based on moving with a robot on a map by right-clicking on the path.
You can interact with various objects on the map using right or left mouse button while hovering over the object.
Some of those objects will send you to a different room, where there are other objects and characters you can interact with.
Other objects will immediatelly turn on a dialogue - dialogue can be controlled by left-clicking over the dialogue panel.
Sometimes you can make a decision in a dialogue - the text will change color when hovering over it with cursor.
In that case the player can choose an option by clicking on the text representing his choice.
</p>
<p>
Robot has a limited level of battery during the game (you can see the remaining level of battery in the upper right corner)
As soon as the robot runs out of battery, the game ends.
You have to use segments of battery to progress in the game.
</p>
<p>
You can quit the game while in main scene (overworld) by pressing Escape.
In this menu you can also change the volume of music and sounds.
</p>
<p>
Achieved endings are being stored in the main menu, those remain saved even after closing and opening the game.
</p>
<p>
You can achieve 8 different endings, list of their names is in the Stats section.
The main ending one should strive to achieve is ending 1 - The Martyr.
</p>
<p>
We hope you'll like our game :)
</p>
</div>
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

    .p-div {
        width: 80%;
        margin: auto;
        margin-top: 20px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
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