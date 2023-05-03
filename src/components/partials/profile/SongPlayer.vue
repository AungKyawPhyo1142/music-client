<template>
    <di class="bg-green-500 rounded">
        <div id="aplayer">
        </div>        
    </di>
</template>

<script setup>

import APlayer from 'aplayer';
import 'aplayer/dist/APlayer.min.css';
import { onMounted } from 'vue';

onMounted(()=>{
    thePlayer();
})

const thePlayer = ()=> {
    new APlayer({
    container: document.getElementById('aplayer'),
    audio: [
        {
            name: 'First Song',
            artist: 'artist',
            url: '/music/firstSong.mp3',
            cover: 'cover.jpg'
        },
        {
            name: 'Second Song',
            artist: 'artist',
            url: '/music/secondSong.mp3',
            cover: 'cover.jpg'
        },

    ]
});
}
</script>

<style lang="stylus" scoped>

</style>
