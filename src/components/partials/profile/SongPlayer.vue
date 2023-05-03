<template>
    <di class="bg-green-500 rounded">
        <div id="aPlayer">

        </div>        
    </di>
</template>

<script setup>
import APlayer from 'aplayer';

const thePlayer = ()=> {
    new APlayer({
    container: document.getElementById('aplayer'),
    audio: [{
        name: 'name',
        artist: 'artist',
        url: 'url.mp3',
        cover: 'cover.jpg'
    }]
});
}

</script>

<style lang="stylus" scoped>

</style>
