<template>
    <header>
        <a href="#">
            <img src="../assets/img/la-molisana-logo.png" alt="Logo">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in navbar" :key="index">
                    <a :href="link.url" :class="{'active': link.current}">{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
import { links } from '../data/data'
    export default {
        name: 'HeaderComponent',
        data(){
            return{
                navbar: links
            }
        },
        methods :{
            getImagePath: function(imgPath){
                return new URL (imgPath, import.meta.url).href;
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;
header{
    text-align: center;
    a{
        text-decoration: none;
    }
    nav{
        ul{
            list-style: none;
            margin:  2.5rem 1rem 4rem;
            @include dflex;
            li a{
                display: inline-block;
                padding: 1rem;
                text-decoration: none;
                font-weight: 600;
                color: $blacktext;

                &.active, 
                &:hover{
                background-color: $lightblue;
                }
            }
        }
    }
}

</style>