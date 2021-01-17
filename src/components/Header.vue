<template>
    <div class="menu">
        <a href="/">
            <img class="logo" src="~@/assets/miiesha-logo-01.png" alt="Miiesha">
        </a>
        <ul>
            <a href="/">
                <li>Bio</li>
            </a>
            <a href="/">
                <li>Watch</li>
            </a>
            <a href="/">
                <li>Contact</li>
            </a>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    .logo {
        display: block;
        margin: 0 auto;
        padding: 20px;
        width: 240px;
        height: auto;
    }

    ul {
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0;
        padding: 0;
    }
    
    li {
        padding: 20px 30px;
        font-size: 24px;
        font-weight: 400;
        text-align: center;
        color: #ffffff;
        transition: ease-in-out;
        transition-duration: .2s;
    }

    li:hover {
        opacity: 0.75;
    }

    a {
        text-decoration: none!important;
    }
</style>