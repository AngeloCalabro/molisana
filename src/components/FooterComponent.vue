<template>
    <footer>
        <div class="cols container">
            <a href="#" class="logo">
                <img src="../assets/img/la-molisana-logo.png" alt="logo">
            </a>

                <div class="footer-links">
                <h4></h4>
                <nav>
                <ul>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                </ul>
                </nav>
                </div>

        </div>
    </footer>
</template>

<script>
    export default {
        name: 'FooterComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

footer{
    padding-top: 3rem;
    .cols{
        display: flex;
        margin-bottom: 3rem;
        .footer-links{
            flex-basis: calc(100%/3);
        }
        h4{
            color: $bluetext;
        }
        ul{
            list-style: none;
            li a{
                display: inline-block;

                &:hover{
                    color: $primary;
                }
            }
        }
    }
}
</style>