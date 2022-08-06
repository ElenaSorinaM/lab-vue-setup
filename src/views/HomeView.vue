<template>
  <div class="home">
    <input type="number" v-model="num1" :class="check" />
    <input type="number" v-model="num2" />
    <p> {{result}} </p>
  </div>
</template>

<script>

export default {
    name: "HomeView",
    data() {
        return {
            num1: 1,
            num2: 2,
        };
    },
    methods: {},
    computed: {
        result () {
            return this.num1 + this.num2;
        },
        check () {
            if (this.num1 <10 ) {
                return 'unvalid';
            } else {
                return 'valid';
            }
        }
    },
};
</script>

<style scoped>
.unvalid {
    border: 1px solid red;
}
.valid {
    border: 1px solid green;
}
</style>