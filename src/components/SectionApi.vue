<template>
    <div>
        
    </div>
</template>

<script>

import axios from 'axios';


export default {
    name: 'SectionApi',
    data() {
        return {
            news: null,
        }
    },
    mounted() {
        fetch('https://newsapi.org/v2/top-headlines?country=co&category=sports&apiKey=8982d839d7174ed0959e518d808770ea', {method: 'GET'})
        .then(response => {
            (this.news = response)
            console.log(this.news)
        })
    }
}

</script>