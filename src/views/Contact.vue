<template>
    <div class="contact">
        <p>
            Bookings<br>
            <a href="mailto:katie@villagesounds.com">katie@villagesounds.com</a>
            <br><br>
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
        font-size: 24px;
    }

    #app {
        background-image: url('~@/assets/miiesha-04.jpg');
        background-position: center;
        background-size: cover;
    }
</style>