<template>
    <div>
        <app-stock v-for="stock in stocks" :key="$index">
        </app-stock>
    </div>
</template>
<script>
import Stock from './Stock.vue'
export default {
    data() {
        return {
            stocks: [
                { id: 1, name: 'BMW', price: 10},
                { id: 2, name: 'Google', price: 10},
                { id: 1, name: 'Facebook', price: 10},
                { id: 1, name: 'Apple', price: 10},
                { id: 1, name: 'Tesla', price: 10}
            ]
        }
    },
    components: {
        appStock: Stock
    }
}
</script>