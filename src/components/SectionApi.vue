<template>
    <div>

    </div>
</template>

<script>
export default {
    name: 'SectionApi',
    data(){
        return {
            news: null
        }
    },
    mounted(){
        fetch("https://api-football-v1.p.rapidapi.com/v2/countries", {
            "method": "GET", "headers": {
                "x-rapidapi-key": "24c5dd9bbamshf3f8ce442013e00p1187a2jsnd442d6f65bda",
                "x-rapidapi-host": "api-football-v1.p.rapidapi.com"
            }
        })
        .then(response => {
            (this.news = response.json())
            console.log(this.news);
        })
        .catch(err => {
            console.error(err);
        });
    }
}
</script>