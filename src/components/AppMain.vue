<template>
    <main>
        <div class="container">
        <pre>--> Content Goes Here </pre>
        </div>
    </main>
</template>

<script>
export default {
    name: 'AppMain',
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    main{
        background-color: $dark-bg;
        height: 100px;

        pre{
            color: #FFF;
        }
    }
</style>