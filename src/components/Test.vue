<template>
   <div>
        <p> Message : {{ msg }} </p>
        <p> Only first word : {{ onlyFirstWord }} </p>
   </div>
</template>

<script>
export default {
    data() {
        return {
            msg: "hello world"
        }
    },
    computed: {
        onlyFirstWord() {
            return this.msg.split(' ')[0].toUpperCase();
        }
    }
}
</script>