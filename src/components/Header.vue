<template>
    <div>
        <div class="m-h-10 d-flex flex-column justify-content-between my-5 font-big-1-2">
            <div class="d-flex flex-row justify-content-between">
                <ul class="list-unstyled font-weight-bold">
                    <li><g-link to="/">HOME</g-link></li>
                    <li><g-link to="/about">ABOUT</g-link></li>
                    <li><g-link to="/games">GAMES</g-link></li>
                    <li><g-link to="/blog">BLOG</g-link></li>
                    <li><g-link to="/contact">CONTACT</g-link></li>
                </ul>
                <div class="d-flex flex-column justify-content-end">
                    <img class="logo" src="../assets/tointerLogo.png" width="200" />
                </div>
            </div>
            <div>
                <div class="w-3 border-bottom"></div>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>

    .m-h-10 {
        min-height: 10rem;
    }

    .logo {
        width: 134px;
        background: linear-gradient(45deg, #ff4d82, #74a8f0);
        border-radius: 16px;
    }


</style>