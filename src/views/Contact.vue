<template>
    <div class="contact">
        <p>
            Bookings<br>
            <a href="mailto:katie@villagesounds.com">katie@villagesounds.com</a>
            <br><br><br>
            Management<br>
            <a href="mailto:info@miiesha.com">info@miiesha.com</a>
        </p>
    </div>
</template>

<script>
export default {
    name: 'Contact'
}
</script>

<style>
    a {
        color:#ffffff;
    }

    .contact {
        padding: 30px;
        display: flex;
        justify-self: center;
        align-items: center;
        color: #ffffff;
    }

    .contact p {
        font-size: 24px;
    }

    #app {
        background-position: center;
        background-size: cover;
    }
</style>