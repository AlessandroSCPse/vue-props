<template>
    <div>
        <h2>{{ titleText }}</h2>
    </div>
</template>

<script>
export default {
    name: "TitleComponent",
    // props: ['titleText'],
    props: {
        titleText: String
    },
    data() {
        return {
            miaVar: 'Dichiarata nel componente'
        };
    },
    methods: {}
}
</script>

<style lang="scss" scoped>
h2 {
    margin: 30px 0;
}
</style>