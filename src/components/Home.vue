<template>
    <div>
        <h1>Home component.</h1>
    <p>Your Funds: {{ funds }}</p>
    </div>
</template>
<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds;
        }
    }
}
</script>