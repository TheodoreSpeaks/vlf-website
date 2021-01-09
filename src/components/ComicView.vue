<template>
    <div class="comic-grid">
        <div class="comic-panel" v-for="m in 8" :key="m">
            <v-img class="comic-panel" height="256" width="256" src="../assets/comic_panel2.jpg"/>

        </div>
    </div>
    
</template>

<script>
export default {
    name: 'ComicView',
    data: () => ({
        
    })
    
}
</script>

<style scoped>
.comic-grid {
    padding: 64px 64px;
    /* flex-direction: row; */
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
    width: 100%
}

.comic-panel {
    margin: 8px 8px;
    background-image: '../assets/comic_panel2.jpg';
    background-size: cover;
}

</style>