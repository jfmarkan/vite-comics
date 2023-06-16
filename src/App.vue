<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppBlueRow from './components/AppBlueRow.vue';

export default {
    name: 'App',
    components:{
    AppHeader,
    AppMain,
    AppFooter,
    AppBlueRow,
  }
}
</script>

<template>
    <AppHeader />
    <AppMain />
    <AppBlueRow />
    <AppFooter />
</template>

<style lang="scss">
  @import './styles/general.scss';
</style>
