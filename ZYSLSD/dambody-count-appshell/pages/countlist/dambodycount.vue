<template>
    <div class="detail-wrapper">
        <v-layout row wrap>
            <v-flex xs10 offset-xs1>
                <article class="detail-content text-xs-center">
                    <header class="detail-title text-xs-center">
                        重力坝抗滑稳定计算
                    </header>
                    <table class="table text-xs-center">
                        <tr>
                            <th>{{rowTitles[0]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[1]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[2]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[3]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[4]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[5]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[6]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[7]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[8]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[9]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[10]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[11]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[12]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[13]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[14]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[15]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[16]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[17]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[18]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>                        
                        <tr>
                            <th>{{rowTitles[19]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>                       
                         <tr>
                            <th>{{rowTitles[20]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>                        
                        <tr>
                            <th>{{rowTitles[21]}}</th>
                            <td>
                                <input style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>                        
                        
                    </table>
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
        },
        data: function () {
            return {
                rowTitles: [
                    "坝顶高程(m)：",
                    "建基面高程（m)：",
                    "上游水位(m)：",
                    "下游水位(m)：",
                    "上游面放坡高程(m)：",
                    "下游面放坡高程(m)：",
                    "上游坝坡坡度（1：m）：",
                    "下游坝坡坡度（1：m）：",
                    "水溶重ro(t/m3)：",
                    "坝体材料溶重r(t/m3)：",
                    "淤沙高程(m)：",
                    "淤沙浮溶重rs(t/m3)：",
                    "淤沙摩擦角（度)：",
                    "灌浆折减系数：",
                    "排水孔处折减系数：",
                    "排水孔宽度(m)：",
                    "坝顶宽度(m)： ",
                    "灌浆距上游坝面平距(m)：",
                    "抗剪断摩擦系数f´： ",
                    " 抗剪断粘结力C´(t)：",
                    "抗剪摩擦系数f： ",
                    "浪高hz（m）: ",
                ]
            }
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

    table {
        border: 2px solid #1976d2;
        border-radius: 3px;
        background-color: #fff;
    }

    th {
        background-color: #1976d2;
        color: white;
        cursor: pointer;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
    }

    td {
        background-color: #f9f9f9;
    }

    th,
    td {
        min-width: 120px;
        padding: 20px 20px;
    }
</style>