<template>
    <div id="Body">
        this is a body. in the trunk. Muahahaha.
        <button id="crazy-btn" v-on:click="createChild">Click Me!</button>
        <One/>
        <Two/>
        <Three/>
    </div>
</template>
<script>
import One from './one.vue';
import Two from './two.vue';
import Three from './three.vue';
export default {
    name: 'Body',
    components: {
        One,
        Two,
        Three
    },
    methods: {
        createChild: function (){
            console.log("this is what happens when you click me!");
            document.getElementById('Body').style.backgroundColor = "blue";
        }
    }
}
</script>
<style scoped>
#Body {
    background-color: bisque;
    min-height: 80vh;
    width: 100vw;
}
</style>