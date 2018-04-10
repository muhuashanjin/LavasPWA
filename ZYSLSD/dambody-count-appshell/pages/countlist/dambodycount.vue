<template>
    <div class="detail-wrapper">
        <v-layout row wrap>
            <v-flex xs10 offset-xs1>
                <article class="detail-content text-xs-center">
                    <header class="detail-title text-xs-center">
                        重力坝抗滑稳定计算
                    </header>
                    <p>
                        下游水位(m)：
                        <input style="border:1px solid" placeholder=" 必填">
                    </p>
                    <p>
                        上游面放坡高程(m)：
                        <input style="border:1px solid" placeholder=" 必填">
                    </p>
                    <p>
                        下游面放坡高程(m)：
                        <input style="border:1px solid" placeholder=" 必填">
                    </p>
                    <p>
                        上游坝坡坡度（1：m）：
                        <input style="border:1px solid" placeholder=" 必填">
                    </p>
                    <p>
                        下游坝坡坡度（1：m）：
                        <input style="border:1px solid" placeholder=" 必填">
                    </p>
                </article>
            </v-flex>
        </v-layout>
    </div>
</template>

<script>
let state = {
  appHeaderState: {
    show: true,
    title: "ZyslsdProgram",
    showMenu: false,
    showBack: true,
    showLogo: false,
    actions: [
      {
        icon: "home",
        route: {
          name: "index"
        }
      }
    ]
  }
};

function setState(store) {
  store.dispatch("appShell/appHeader/setAppHeader", state.appHeaderState);
}

export default {
  name: "detailId",
  metaInfo() {
    return {
      title: `ZyslsdProgram`,
      titleTemplate: "%s - 遵义水利水电勘测设计研究院的计算程序",
      meta: [
        { name: "keywords", content: "Zyslsd Program" },
        { name: "description", content: "Zyslsd Program" }
      ]
    };
  },
  async asyncData({ store, route }) {
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
.detail-content {
  font-size: 16px;
  line-height: 30px;
  margin-top: 30px;

  .detail-title {
    margin-bottom: 20px;
    padding: 10px 0;
    font-size: 36px;
    font-weight: bold;
  }
}
</style>
