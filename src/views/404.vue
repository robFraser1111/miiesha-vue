<template>
    <div class="not-found">
        <p>
            Sorry, that page can't be found.
            <br /><br />
            <router-link to="/">
                Return home
            </router-link>
        </p>
    </div>
</template>

<script>
export default {
    name: '404'
}
</script>

<style>

    .not-found {
        max-width: 900px;
        text-align: center;
        color: #ffffff;
        padding: 30px;
        display: flex;
        justify-self: center;
        align-items: center;
    }

    .not-found p {
        font-size: 24px;
    }
    
</style>

<style scoped>

    a {
        color: #ffffff;
    }
    
</style>