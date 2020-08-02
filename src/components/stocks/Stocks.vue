<template>
    <div>
        <app-stock v-for="stock in stocks" :stock='stock' :key="$index">
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
                { id: 2, name: 'Google', price: 100},
                { id: 3, name: 'Facebook', price: 20},
                { id: 4, name: 'Apple', price: 200},
                { id: 5, name: 'Tesla', price: 150}
            ]
        }
    },
    components: {
        appStock: Stock
    }
}
</script>