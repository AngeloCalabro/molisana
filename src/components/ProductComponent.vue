<template>
    <div class="col">
        <!-- <img :src="img" :alt="title"> -->
        <img :src="obj.src" :alt="obj.titolo">
        <!-- <h4>{{title}}</h4> -->
        <h4>{{obj.titolo}}</h4>
    </div>
</template>

<script>
    export default {
        name: 'ProductComponent',
        props: [
            // 'img', 'title'
            'obj'
        ]
    }
</script>

<style lang="scss" scoped>

</style>