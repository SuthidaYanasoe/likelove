<template>
<div id="app">

    <HelloWorld msg="We want everyone to join the press and express their feelings as show in the picture." />
    <hr>
    <div class="row">
        <div class="col-6">
            <img src="https://img.kapook.com/u/2018/Jarosphan/Pet/Cat/166/01.jpg" width="630" height="430">
            <br />
            <br />
            <h3>Persian cat</h3>
            <h7>อ่อนโยน เข้ากับคนอื่นง่าย ช่างประจบ มีไหวพริบมาก</h7>
            <h1>{{total1}}</h1>
            <CsButton @cc="sum" />
        </div>
        <div class="col-6">
            <img src="https://img.kapook.com/u/pirawan/Pet/shutterstock_119848222.jpg" width="630" height="430">
            <br />
            <br />
            <h3>Main Coon cat</h3>
            <h7>นิสัยขี้อ่อน ผิดกับหน้าตา ขี้เล่น ร่าเริง</h7>
            <h1>{{total2}}</h1>
            <CsButton @cc="sum1" />
        </div>
        <div class="col-6">
            <img src="https://img.kapook.com/u/pirawan/Pet/bangol1.jpg" width="630" height="430">
            <br />
            <br />
            <h3>Bengal cat</h3>
            <h7>เป็นมิตรกับทุกคน ซุกซน ชอบปีนป่าย ชอบเล่นน้ำ</h7>
            <h1>{{total3}}</h1>
        </div>

        <div class="col-6">
            <img src="https://static.trueplookpanya.com/tppy/member/m_545000_547500/545994/cms/images/2018-08-Sep/%E0%B8%A7%E0%B8%B4%E0%B9%80%E0%B8%8A%E0%B8%B5%E0%B8%A2%E0%B8%A3%E0%B8%A1%E0%B8%B2%E0%B8%A8_02.jpg" width="630" height="430">
            <br />
            <br />
            <h3>Siamese cat</h3>
            <h7>ฉลาด ปราดเปรียว เป็นตัวของตัวเองสูง</h7>
            <h1>{{total4}}</h1>
        </div>
        <div class="col-6">
            <CsButton @cc="sum2" />
        </div>
        <div class="col-6">
            <CsButton @cc="sum3" />
        </div>

    </div>

</div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CSButton.vue";
export default {
    name: "App",
    components: {
        HelloWorld,
        CsButton,

    },
    data: function () {
        return {
            total1: 0,
            total2: 0,
            total3: 0,
            total4: 0,

        }
    },
    methods: {
        sum(counterValue) {
            this.total1 = counterValue
        },

        sum1(counterValue) {
            this.total2 = counterValue

        },

        sum2(counterValue) {
            this.total3 = counterValue
        },

        sum3(counterValue) {
            this.total4 = counterValue
        },

    },

};
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #000000;
    margin-top: 60px;
}
</style>
