<template>
    <main>
        <AppJumbo />
        <div class="indicator">
            <h4>CURRENT SERIES</h4>
        </div>
        <AppProducts />
        <AppBlueRow />
    </main>
</template>

<script>
import AppBlueRow from './AppBlueRow.vue';
import AppJumbo from './AppJumbo.vue';
import AppProducts from './AppProducts.vue';

export default {
    name: 'AppMain',
    components:{
    AppBlueRow,
    AppProducts,
    AppJumbo
},
    
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    main{
        background-color: $dark-bg;
        position: relative;

        .indicator{
            background-color: $blue-bg;
            position: absolute;
            color: #FFF;
            padding: .5rem 1rem;
            transform: translate(-50%, -50%);
            top: 0;
            left: 20%;
        }
    }
</style>