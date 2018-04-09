<template>
    <div>
        <div class="content">
            <div>
                <h2>Zyslsd Program</h2>
            </div>
        </div>
    </div>
</template>

<script>
import {mapActions} from 'vuex';
function setState(store) {
    store.dispatch('appShell/appHeader/setAppHeader', {
        show: true,
        title: 'ZyslsdProgram',
        showMenu: true,
        showBack: false,
        showLogo: false,
        actions: [
            {
                icon: 'search',
                route: '/search'
            }
        ]
    });
}

export default {
    name: 'index',
    metaInfo: {
        title: 'Home',
        titleTemplate: '%s - ZyslsdProgram',
        meta: [
            {name: 'keywords', content: 'Zyslsd Program'},
            {name: 'description', content: 'Zyslsd Program'}
        ]
    },
    async asyncData({store, route}) {
        setState(store);
    },
    activated() {
        setState(this.$store);
    }
};
</script>

<style lang="stylus" scoped>
.content
    display flex
    align-items center
    justify-content center
    height 100%
    flex-wrap wrap
    h2
        font-size 46px
        font-weight 500
</style>
