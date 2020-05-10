<template>
    <div>
        <h3>
            New Quote
            <button @click="counter++">Increase</button>
            <p>{{ counter }}</p>
        </h3>
    </div>   
</template>
<script>
export default {
    data: function(){
        return{
            counter: 0
        };
    },
    destroyed: function(){
        console.log("Destroyed !!");
    },
    deactivated(){
        console.log("Deactived !!");
    },
    activated(){
        console.log("Activated !!");
    }
}
</script>
<style>
</style>