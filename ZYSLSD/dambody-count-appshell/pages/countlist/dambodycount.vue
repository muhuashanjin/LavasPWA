<template>
    <div class="detail-wrapper">
        <v-layout row wrap>
            <v-flex xs10 offset-xs1>
                <article class="detail-content text-xs-center">
                    <header class="detail-title text-xs-center">
                        重力坝计算
                    </header>
                </article>
            </v-flex>
        </v-layout>
    </div>
</template>

<script>
let state = {
    appHeaderState: {
        show: true,
        title: 'ZyslsdProgram',
        showMenu: false,
        showBack: true,
        showLogo: false,
        actions: [
            {
                icon: 'home',
                route: {
                    name: 'index'
                }
            }
        ]
    }
};

function setState(store) {
    store.dispatch('appShell/appHeader/setAppHeader', state.appHeaderState);
}

export default {
    name: 'detailId',
    metaInfo() {
        return {
            title: `ZyslsdProgram`,
            titleTemplate: '%s - ZyslsdProgram',
            meta: [
                {name: 'keywords', content: 'Zyslsd Program'},
                {name: 'description', content: 'Zyslsd Program'}
            ]
        }
    },
    async asyncData({store, route}) {
        setState(store);
        await new Promise((resolve, reject) => {
            setTimeout(resolve, 500);
        });
    },
    activated() {
        setState(this.$store);
    }
};
</script>

<style lang="stylus" scoped>

.detail-content
    font-size 16px
    line-height 30px
    margin-top 30px

    .detail-title
        margin-bottom 20px
        padding 10px 0
        font-size 36px
        font-weight bold

</style>
