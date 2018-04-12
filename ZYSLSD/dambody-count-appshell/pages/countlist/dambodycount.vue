<template>
    <div class="detail-wrapper">
        <!-- <v-layout row wrap>
            <v-flex xs10 offset-xs1> -->
                <article class="detail-content text-xs-center">
                    <header class="detail-title text-xs-center">
                        重力坝抗滑稳定计算
                    </header>
                    <table class="table">
                        <tr>
                            <th>{{rowTitles[0]}}{{B3}}</th>
                            <td>
                                <input v-model="B3" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[1]}}{{B4}}</th>
                            <td>
                                <input v-model="B4" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[2]}}{{B5}}</th>
                            <td>
                                <input v-model="B5" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[3]}}{{B6}}</th>
                            <td>
                                <input v-model="B6" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[4]}}{{B7}}</th>
                            <td>
                                <input v-model="B7" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[5]}}{{B8}}</th>
                            <td>
                                <input v-model="B8" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[6]}}{{B9}}</th>
                            <td>
                                <input v-model="B9" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[7]}}{{B10}}</th>
                            <td>
                                <input v-model="B10" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[8]}}{{B11}}</th>
                            <td>
                                <input v-model="B11" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[9]}}{{B12}}</th>
                            <td>
                                <input v-model="B12" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[10]}}{{B13}}</th>
                            <td>
                                <input v-model="B13" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[11]}}{{D3}}</th>
                            <td>
                                <input v-model="D3" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[12]}}{{D4}}</th>
                            <td>
                                <input v-model="D4" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[13]}}{{D5}}</th>
                            <td>
                                <input v-model="D5" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[14]}}{{D6}}</th>
                            <td>
                                <input v-model="D6" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[15]}}{{D7}}</th>
                            <td>
                                <input v-model="D7" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[16]}}{{D8}}</th>
                            <td>
                                <input v-model="D8" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[17]}}{{D9}}</th>
                            <td>
                                <input v-model="D9" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[18]}}{{D10}}</th>
                            <td>
                                <input v-model="D10" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[19]}}{{D11}}</th>
                            <td>
                                <input v-model="D11" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[20]}}{{D12}}</th>
                            <td>
                                <input v-model="D12" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[21]}}{{D13}}</th>
                            <td>
                                <input v-model="D13" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[22]}}{{K5}}</th>
                            <td>
                                <input v-model="K5" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[23]}}{{K6}}</th>
                            <td>
                                <input v-model="K6" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[24]}}{{K7}}</th>
                            <td>
                                <input v-model="K7" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[25]}}{{K8}}</th>
                            <td>
                                <input v-model="K8" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[26]}}{{K9}}</th>
                            <td>
                                <input v-model="K9" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[27]}}{{K10}}</th>
                            <td>
                                <input v-model="K10" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>                        
                        <tr>
                            <th>{{rowTitles[28]}}{{K11}}</th>
                            <td>
                                <input v-model="K11" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[29]}}{{K12}}</th>
                            <td>
                                <input v-model="K12" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[30]}}{{K13}}</th>
                            <td>
                                <input v-model="K13" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[31]}}{{M3}}</th>
                            <td>
                                <input v-model="M3" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                        <tr>
                            <th>{{rowTitles[32]}}{{M11}}</th>
                            <td>
                                <input v-model="M11" style="border: 2px solid #1976d2" placeholder=" 必填">
                            </td>
                        </tr>
                    </table>
                    <button v-on:click="incrementCounter" style="width:150px;margin-top:20px;text-align:center;background-color:#1976d2;color:#fff;line-height:200%;">
                        点击生成计算结果
                    </button>
                    <table class="table" style="margin-top:20px;margin-bottom:20px;">
                        <tr>
                            <th>{{resultTitles[0]}}{{resultH13}}</th>
                        </tr>
                        <tr>
                            <th>{{resultTitles[1]}}{{resultM12}}</th>
                        </tr>
                        <tr>
                            <th>{{resultTitles[2]}}{{resultM13}}</th>
                        </tr>
                    </table>
                </article>
            <!-- </v-flex>
        </v-layout> -->
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
                    "第一滑裂面与水平面夹角α（角度）: ",
                    "第二滑裂面与水平面夹角β（角度）（先试算使K2´最小）:",
                    "第一滑裂面与水平面夹角α（弧度）:",
                    "第二滑裂面与水平面夹角β（弧度）: ",
                    "两滑面上岩体间作用面上作用力与水平面的夹角φ: ",
                    "第一滑裂面抗剪断摩擦系数f1´：",
                    "第二滑裂面抗剪断摩擦系数f2´：",
                    "第一滑裂面抗剪断粘结力C1´(t): ",
                    "第二滑裂面抗剪断粘结力C2´(t): ",
                    "岩体溶重r(t/m3)：",
                    "两滑面上岩体间作用面上作用力Q(试算使K1´=K2´)："
                ],
                resultTitles: [
                    "沿建基面滑动（单滑面）- 下游水深矩形浮托力U1(t)：",
                    "深层滑动（双滑面）- 第一滑裂面的抗滑稳定安全系数K1´:",
                    "深层滑动（双滑面）- 第二滑裂面的抗滑稳定安全系数K2´:"
                ],

                // rowTitles[0]-B3，rowTitles[11]-D3，rowTitles[22]-K5
                // 以此类推往下一一对应
                B3: 796,
                B4: 758,
                B5: 797.38,
                B6: 761.74,
                B7: 771.2,
                B8: 793,
                B9: 5,
                B10: 1.333333,
                B11: 0.981,
                B12: 2.467,
                B13: 776.5,
                D3: 0.8,
                D4: 14,
                D5: 0.25,
                D6: 0,
                D7: 0,
                D8: 6,
                D9: 4,
                D10: 0.78,
                D11: 68,
                D12: 0.68,
                D13: 0.200843,
                K5:3,
                K6:38,
                K7:0.05236,
                K8:0.66323,
                K9:0,
                K10:0.58,
                K11:0.68,
                K12:18,
                K13:48,
                M3:2.7,
                M11:225,

                //最终结果
                resultH13:0,
                resultM12:0,
                resultM13:0,

            }
        },
        methods: {
        incrementCounter: function () {
            console.log('server started at localhost:============' );

            //==================沿建基面滑动（单滑面）===================

            //最大坝高(m)：
            let F3 = this.B3-this.B4;
            console.log("最大坝高(m)： " + F3);

            //坝底宽度(m)：
            let F4 = ((this.B7>this.B4?this.B7:this.B4)-this.B4)/(this.B9>0?this.B9:1) + this.D8+(this.B8-this.B4)/this.B10;
            console.log("坝底宽度(m)： " + F4);

            //矩形体自重G1(t)：
            let F5 = this.D8 * this.B12 * F3;
            console.log("矩形体自重G1(t)： " + F5);

            //下游楔形体自重G2(t)：
            let F6 = 0.5*Math.pow((this.B8-this.B4),2)*this.B12/this.B10;
            console.log("下游楔形体自重G2(t)： " + F6);

            //上游楔形体自重G2(t)：
            let F7 = 0.5*this.B12*Math.pow((this.B7-this.B4),2)*(this.B9>0?1:0)/(this.B9>0?this.B9:1);
            console.log("上游楔形体自重G2(t)： " + F7);
            
            //上游矩形体水重G2(t)：
            let F8 = this.B11*(this.B5-this.B7)*((this.B7>this.B4?this.B7:this.B4)-this.B4)/(this.B9>0?this.B9:1);
            console.log("上游矩形体水重G2(t)：" + F8);


            //上游楔形体水重G2(t)：
            let F9 = 0.5*this.B11*Math.pow(((this.B7>this.B4?this.B7:this.B4)-this.B4),2)*(this.B9>0?1:0)/(this.B9>0?this.B9:1);
            console.log("上游楔形体水重G2(t)：" + F9);

            //下游楔形体水重G2(t)：
            let F10 = 0.5*this.B11*Math.pow((this.B6-this.B4),2)/this.B10;
            console.log("下游楔形体水重G2(t)：" + F10);

            //垂直淤沙压力PsV(t)：
            let F11 = 0.5*this.D3*Math.pow((this.B13-this.B4),2)*(this.B9>0?1:0)/(this.B9>0?this.B9:1);
            console.log("垂直淤沙压力PsV(t)：" + F11);

            //竖直向下合力ΣG(t):
            let F12 = F5 + F6 + F7 + F8 + F9 + F10 + F11;
            console.log("竖直向下合力ΣG(t):" + F12);

            //下游水深矩形浮托力U1(t)：
            let F13 = this.B11*F4*(this.B6-this.B4)*(this.B4>this.B6?0:1);
            console.log("下游水深矩形浮托力U1(t)：" + F13);

            //排水孔折减处扬压力U2(t)：
            let H3 = 0.5*this.B11*(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D6*(F4-this.D9-this.D7);
            console.log("排水孔折减处扬压力U2(t)：" + H3);

            //灌浆折减处扬压力U3(t)：
            let H4 = (this.D6>0,
            0.5*this.B11*((this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5+((this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D6))*this.D7,
            0.5*this.B11*(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5*(F4-this.D9));
            console.log("灌浆折减处扬压力U3(t)：" + H4);
            
            //坝踵处扬压力U4(t)：
            let H5 = 0.5*this.B11*((this.B5-(this.B4>this.B6?this.B4:this.B6))+(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5)*this.D9;
            console.log("坝踵处扬压力U4(t)：" + H5);

            //总扬压力ΣU(t):
            let H6 = F13 + H3 + H4 + H5;
            console.log("总扬压力ΣU(t):" + H6);

            //总铅直力ΣW(t):↓
            let H7 = F12 - H6;
            console.log("总铅直力ΣW(t):↓" + H7);

            //上游水平水压力P1(t)：
            let H8 = 0.5*this.B11*Math.pow((this.B5-this.B4),2);
            console.log("上游水平水压力P1(t)：" + H8);

            //下游水平水压力P2(t)：
            let H9 = 0.5*this.B11*Math.pow((this.B6-this.B4),2)*(this.B4>this.B6?0:1);
            console.log("下游水平水压力P2(t)：" + H9);

            //上游水平淤沙压力PsH(t)：
            let H10 = 0.5*this.D3*Math.pow((this.B13-this.B4),2)*Math.pow((Math.tan((45-this.D4/2)*3.1415926/180)),2);
            console.log("上游水平淤沙压力PsH(t)：" + H10);

            //浪压力(t)：
            let H11 = this.B11*5*this.D13*(5*this.D13+this.D13+0.3*this.D13)/2-this.B11*Math.pow((5*this.D13),2)/2;
            console.log("浪压力(t)：" + H11);

            //总水平力ΣP(t):→
            let H12 = H8-H9+H10+H11;
            console.log("总水平力ΣP(t):→" + H12);
            
            //抗剪断安全系数K´:
            let H13 = (this.D10*H7+this.D11*F4*1)/H12;
            console.log("抗剪断安全系数K´:" + H13);
            
            this.resultH13 = H13;

            //==================深层滑动（双滑面）===================
           
            //坝体竖直向下的合力W(t)↓:
            let K3 = F12;
            console.log("坝体竖直向下的合力W(t)↓：" + K3);

            //坝体水平向合力H(t)→:
            let K4 = H12;
            console.log("坝体水平向合力H(t)→：" + K4);    
 
            //第一滑裂面面积A1:
            let M4 = F4/Math.cos(this.K7)*1;
            console.log("第一滑裂面面积A1：" + M4);   

            //第二滑裂面面积A2:
            let M5 = (F4*Math.tan(this.K7)+3)/Math.sin(this.K8)*1;
            console.log("第二滑裂面面积A2：" + M5);  
            
            //第一滑裂面上岩体自重G1(t):
            let M6 = this.M3*0.5*F4*F4+Math.tan(this.K7)*1;
            console.log("第一滑裂面上岩体自重G1(t)：" + M6);

            //第二滑裂面上岩体自重G2(t):
            let M7 = this.M3*0.5*(F4*Math.tan(this.K7)+3)*(F4*Math.tan(this.K7)+3)/Math.tan(this.K8);
            console.log("第二滑裂面上岩体自重G2(t)：" + M7);

            //第一滑裂面上扬压力U1:
            let M8 = (this.B11*(this.B6-this.B4+F4*Math.tan(this.K7))*F4/Math.cos(this.K7))+0.5*(this.B11*(this.B5-this.B4-(this.B6-this.B4+F4*Math.tan(this.K7)))+this.D5*this.B11*(this.B5-this.B4-(this.B6-this.B4+F4*Math.tan(this.K7))))*this.D9/Math.cos(this.K7)+0.5*this.D5*this.B11*(this.B5-this.B4-(this.B6-this.B4+F4*Math.tan(this.K7)))*(F4/Math.cos(this.K7)-this.D9/Math.cos(this.K7));
            console.log("第一滑裂面上扬压力U1：" + M8);
            
            //第二滑裂面上扬压力U2:
            let M9 = 0.5*(this.B11*(this.B6-this.B4)+this.B11*(this.B6-this.B4+F4*Math.tan(this.K7)))*F4*Math.tan(this.K7)/Math.sin(this.K8);
            console.log("第二滑裂面上扬压力U2：" + M9);

            //两滑面上岩体间作用面上扬压力U3:
            let M10 = 0.5*(this.B11*(this.B6-this.B4)+this.B11*(this.B6-this.B4+F4*Math.tan(this.K7)))*F4*Math.tan(this.K7);
            console.log("两滑面上岩体间作用面上扬压力U3：" + M10);
            
            //第一滑裂面的抗滑稳定安全系数K1´:
            let M12 = (this.K10*((K3+M6)*Math.cos(this.K7)-K4*Math.sin(this.K7)-this.M11*Math.sin(this.K9-this.K7)-M8+M10*Math.sin(this.K7))+this.K12*M4)/((K3+M6)*Math.sin(this.K7)+K4*Math.cos(this.K7)-M10*Math.cos(this.K7)-this.M11*Math.cos(this.K9-this.K7));
            console.log("第一滑裂面的抗滑稳定安全系数K1´：" + M12);

            //第二滑裂面的抗滑稳定安全系数K2´:
            let M13 = (this.K11*(M7*Math.cos(this.K8)+this.M11*Math.sin(this.K9+this.K8)-M9+M10*Math.sin(this.K8))+this.K13*M5)/(this.M11*Math.cos(this.K9+this.K8)-M7*Math.sin(this.K8)+M10*Math.cos(this.K8));
            console.log("第二滑裂面的抗滑稳定安全系数K2´：" + M13);         
            
            this.resultM12 = M12;
            this.resultM13 = M13;

            //==================重力坝上、下游边缘正应力计算（沿建基面）==================

            let C17 = F5;
            let C18 = F6;
            let C19 = F7;
            let C22 = F8;
            let C23 = F9;
            let C24 = F10;
            let C30 = F11;

            let D25 = F13;
            let D26 = H3;
            let D27 = H4;
            let D28 = H5;

            let E20 = H8;
            let E29 = H11;
            let E31 = H10;

            let F21 = H9;

            //垂直力合计:
            let C33 = (C17+C18+C19+C22+C23+C24+C30) - (D25+D26+D27+D28)
            console.log("垂直力合计：" + C33);  

            //水平力合计:
            let E33 = (E20+E29+E31) - F21
            console.log("水平力合计:" + E33);

            //---对基础中心的力臂---

            //矩形体自重
            let G17 = F4/2-(this.D8/2)-((this.B7>0?this.B7:this.B4)-this.B4)/(this.B9>0?this.B9:1)
            console.log("矩形体自重:" + G17);

            //下游楔形体自重
            let G18 = ((F4/2-((this.B8-this.B4)/this.B10)*2/3)>0?(-(F4/2-((this.B8-this.B4)/this.B10)*2/3)):((((this.B8-this.B4)/this.B10)*2/3)-F4/2));
            console.log("下游楔形体自重:" + G18);

            //上游楔形体自重
            let G19 = F4/2-((this.B7-this.B4)/this.B9)*2/3;
            console.log("上游楔形体自重:" + G19);

            //上游水平水压力
            let G20 = -(this.B5-this.B4)/3;
            console.log("上游水平水压力:" + G20);

            //下游水平水压力
            let G21 = (this.B6-this.B4)/3;
            console.log("下游水平水压力:" + G21);

            //上游矩形体水重
            let G22 = F4/2-(this.B7-this.B4)*(this.B9>0?1:0)/((this.B9>0?this.B9:1)*2);
            console.log("上游矩形体水重:" + G22);

            //上游楔形体水重
            let G23 = F4/2-(this.B7-this.B4)*(this.B9>0?1:0)/((this.B9>0?this.B9:1)*3);
            console.log("上游楔形体水重:" + G23);   

            //下游楔形体水重
            let G24 = -(F4/2-((this.B6-this.B4)/this.B10)/3);
            console.log("下游楔形体水重:" + G24);
            
            //下游水深矩形浮托力
            // let G25 = 0;
            // console.log("下游水深矩形浮托力:" + G25);

            //排水孔折减处扬压力
            let G26 = (F4/2-(F4-this.D9-this.D7)*2/3)>0?(F4/2-(F4-this.D9-this.D7)*2/3):-((F4-this.D9-this.D7)*2/3-F4/2);
            console.log("排水孔折减处扬压力:" + G26);

            //灌浆折减处扬压力
            let G27 =  this.D6>0?
            -(F4/2-this.D9-(((this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5+2*(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D6)*this.D7/3*(((this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5+(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D6)))):
            ((F4/2-(F4-this.D9)*2/3)>0?(F4/2-(F4-this.D9)*2/3):-((F4-this.D9)*2/3-F4/2));
            console.log("灌浆折减处扬压力:" + G27);

            //坝踵处扬压力
            let G28 = -(F4/2-((this.B5-(this.B4>this.B6?this.B4:this.B6))+2*(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5)/(3*((this.B5-(this.B4>this.B6?this.B4:this.B6))+(this.B5-(this.B4>this.B6?this.B4:this.B6))*this.D5)));
            console.log("坝踵处扬压力:" + G28);

            //浪压力
            let G29 = -(this.B5-this.B4+this.D13/2);
            console.log("浪压力:" + G29);
           
            //垂直淤沙压力
            let G30 = (F4/2-(this.B13-this.B4)*(this.B9>0?1:0)/((this.B9>0?this.B9:1)*3));
            console.log("垂直淤沙压力:" + G30);

            //水平淤沙压力
            let G31 = -(this.B13-this.B4)/3;
            console.log("水平淤沙压力:" + G31);
            

            

            



        }
  },
    };
</script>

<style lang="stylus" scoped>
    .detail-content {
        font-size: 16px;
        line-height: 30px;
        margin-top: 30px;

        .detail-title {
            margin-bottom: 20px;
            font-size: 30px;
            font-weight: bold;
        }
    }

    table {
        border: 2px solid #1976d2;
        border-radius: 3px;
        background-color: #fff;
        padding: 30px;
    }

    th {
        border: 2px solid white;
        background-color: #1976d2;
        color: white;
        cursor: pointer;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
    }

    td {
        border: 2px solid #1976d2;
        background-color: #f9f9f9;
    }

    th,
    td {
        min-width: 80px;
        padding: 10px;
    }
</style>