<template lang="">
    <!-- <div>
        <h1>{{sampleData}}</h1>
        <div>{{sampleData2}}</div>
    </div>

    <br />
    <br />

    <div>
        <h1>{{valueModel}}</h1>
        <input type="text" v-model="valueModel" />
        <input type="number" v-model.number="valueModel2" />
        <textarea v-model="valueModel3"></textarea>
    </div>

    <br />
    <br />

    <div>
        <select v-model="city">
            <option value="02">서울</option>
            <option value="21">부산</option>
            <option value="064">제주</option>
        </select>

        <label><input type="checkbox" value="서울" v-model="checked"/>서울</label>
        <label><input type="checkbox" value="부산" v-model="checked"/>부산</label>
        <label><input type="checkbox" value="제주" v-model="checked"/>제주</label>
        <br />
        <span>체크한 지역: {{checked}}</span>
    </div>-->

    <div>
        <label><input type="radio" v-bind:value="radio[0]" v-model="picked" />서울</label>
        <label><input type="radio" v-bind:value="radio[1]" v-model="picked" />부산</label>
        <label><input type="radio" v-vind:value="radio[2]" v-model="picked" />제주</label>
        <br/>
        <span>선택한 지역: {{picked}}</span>
    </div>
</template>

<script>
export default {
    data() {
        return {
            sampleData: "sample",
            sampleData2: "data",

            valueModel: 'Vue Practice',
            valueModel2: 12,
            valueModel3: "Hello",

            city: "064",
            checked: [],

            radio: ["서울","부산","제주"],
            picked: ""
        };
    },
    mounted() {

    },
    methods: {

    }
}
</script>

<style scoped>
    
</style>