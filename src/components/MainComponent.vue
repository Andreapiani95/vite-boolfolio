<script>
import axios from 'axios';

export default {
    name: 'MainComponent',
    data() {
        return {
            projects: []
        }
    },
    created() {
        axios
            .get('http://localhost:8000/api/projects')
            .then(res => {
                console.log(res);
            });

    },
    methods: {

    }
};
</script>

<template>
    <h2>MainComponent</h2>
</template>

<style lang="scss"></style>