<template>
    <v-card class="comic-view" color="background">
    <div class="comic-grid" background-color="background">
        <TitlePanel name="A Christmas Story" date="25 December 2020"/>
        <div class="comic-panel" v-for="m in 7" :key="m">
        <v-img class="comic-panel" height="256" width="256" src="../assets/comic_panel2.jpg"/>
        </div>
    </div>
    <v-card flat color="background">
        <v-btn plain>
            <v-icon size="48px">mdi-chevron-left</v-icon>
            Prev
        </v-btn>
        <v-btn plain>
            Next
            <v-icon size="48px">mdi-chevron-right</v-icon>
        </v-btn>
    </v-card>
    </v-card>
    
</template>

<script>
import TitlePanel from './TitlePanel.vue';
export default {
    name: 'ComicView',
    components: {
        TitlePanel,
    },
    data: () => ({
        
    })
    
}
</script>

<style scoped>
.comic-view {
    padding: 64px 64px;
}
.comic-grid {
    /* padding: 64px 64px; */
    /* flex-direction: row; */
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
    width: 100%;
    background-color: #fdfcdc;
}

.comic-panel {
    margin: 8px 8px;
    background-image: '../assets/comic_panel2.jpg';
    background-size: cover;
}

</style>