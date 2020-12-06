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
            news: null        }
    },
    mounted() {
        fetch('http://www.omdbapi.com/?apikey=c6b2da83&t=brave&type=movie', {method: 'GET'})
        .then(response => {
            (this.news = response)
            console.log(this.news)
        })
    }
}

</script>