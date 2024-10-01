<script>
import { store } from '@/store/store';
import axios from 'axios';

export default { 
    data() {
        return {
            works: [],
        }
    },
    methods: {
        getApi() {
            // missing api

            axios.get(store.apiUrl + 'works').then(response => {
                console.log(response.data);
            })
        }
    },
    mounted() {
        this.getApi();
    },
}
</script>

<template>
    <div>
        <h1> Progetti </h1>
    </div>
</template>

<style lang="scss">
    
</style>