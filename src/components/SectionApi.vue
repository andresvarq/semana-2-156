<template>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5" style="background-color: rgba(255, 255, 255, 0.3); color: aliceblue;">
        <div class="col-lg-6 col-xs-12" v-for="(item, index) of news" :key="index">
            <div class="d-flex justify-content-center align-items-center">
                <div class="p-3">
                    <img v-bind:src="item.logo" alt="" width="200" height="200" style="border-radius: 15%">
                </div>
    
                <div class="p-2">
                    <h4>{{ item.name }}</h4>
                    <p>Fundación: {{ item.founded }} </p>
                    <p>Estadio: {{ item.venue_name }}</p>
                    <p>Ciudad: {{ item.venue_city }}</p>
                </div>
    
            </div>
            <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                <a :href="'https://dimayor.com.co/?s=' + item.name" target="blank" style="color: #f51720;"> Ver info reciente</a>
            </div>
        </div>
    </div>
</template>

<script>

import axios from 'axios';

export default {
    name: 'SectionApi',
    data(){
        return {
            news: null
        }
    },
    mounted(){
        axios
        .get('https://api-football-v1.p.rapidapi.com/v2/teams/league/138', {
            method: 'GET', headers: {
                'x-rapidapi-key': '24c5dd9bbamshf3f8ce442013e00p1187a2jsnd442d6f65bda',
                'x-rapidapi-host': 'api-football-v1.p.rapidapi.com'
            }
        })
        .then(response => {
            (this.news = response.data.api.teams.slice(7, 11))
            console.log(this.news);
        }).catch(function (error) {
            console.error(error);
        });
    }
}


</script>