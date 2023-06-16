<template>
    <main>
        <div class="container">
        <pre>--> Content Goes Here </pre>
        </div>
        <AppBlueRow />
    </main>
</template>

<script>
import AppBlueRow from './AppBlueRow.vue';

export default {
    name: 'AppMain',
    components:{
    AppBlueRow,
    AppBlueRow
}
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