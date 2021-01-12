<template>
    <div class="title-panel">
        <h1>{{name}}</h1>
        <h3>{{date}}</h3>
    </div>
  
</template>

<script>
export default {
    name: "TitlePanel",
    props: ['name', 'date']

}
</script>

<style>
.title-panel {
    background-color: #00afb9;
    width: 256px;
    height: 256px;
    padding: 32px 16px;
    margin: 8px; 
}

</style>