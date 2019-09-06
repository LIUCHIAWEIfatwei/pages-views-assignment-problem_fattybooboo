<template>
    <div>
        <h1>products page</h1>
            <input type="text" v-model="pid1">
            <button @click="goPage1">goPage1</button>
            <br>
            <input type="text" v-model="pid2">
            <button @click="goPage2">goPage2</button>

        

    </div>
</template>

<script>
export default {
    data:() =>({
        pid1:'1',
        pid2:'2'
    }),
    methods:{
        goPage1(){
            this.$router.push('/products/' + this.pid1)
        },
        goPage2(){
            this.$router.push('/products/' + this.pid2)
        },
    }
}
</script>