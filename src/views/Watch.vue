<template>
    <div class="watch">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/1LrXv9hOAHo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</template>

<script>
export default {
    name: 'Watch'
}
</script>

<style>
.watch {
    padding: 30px;
    display: flex;
    justify-self: center;
    align-items: center;
}
#app {
    background-image: url('~@/assets/miiesha-03.jpg');
    background-position: center;
    background-size: cover;
}
</style>