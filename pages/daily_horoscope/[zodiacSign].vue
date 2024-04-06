<template>
    <div>
        <PageHeader/>

        <main>
            <div class="d">
                    <div v-html="data[zodiacSign]?.image"></div>
                <div class="dail">
                    <h2>
                        The daily horoscope for
                        <span style="text-transform: capitalize;">{{ zodiacSign }}</span>
                    </h2>
                    <p>
                        {{data[zodiacSign]?.text}}   
                    </p>
                    <h4>Check out the yearly horoscope</h4>
                </div>
                <div class="da">
                    <p>{{ currentDate.toLocaleString('en-US', { month: 'long' }) }} {{ currentDate.getFullYear() }}</p>
                    <h1>{{ currentDate.getDate() }}</h1>
                    <h3>{{ weekdayName }}</h3>
                </div>
            </div>        
        </main>


        {{ data[zodiacSign]?.text }}
    </div>
</template>

<style>
.d {
    display: flex;
    flex-direction: row;
    padding: 30px;
}
.da {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-left: 150px;
    padding-right: 150px;
    background-color: rgb(238, 228, 169);
    height: 500px;
    padding: 50px;
}
.da h4 {
    text-align: center;
}
.da h1{
    font-size: 200px;
    margin: 0px;
}
.dail h2 {
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(238, 228, 169); 
    letter-spacing: 1px;
    justify-content: center;
    padding: 30px;
    padding-bottom: 0px; 
    text-align: center;   
}
.dail p{
color: rgb(238, 228, 169);
font-size: larger;
line-height: 30px;
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
letter-spacing: 1px; 
text-align: justify;
}
.dail {
}
</style>

<script setup lang="ts">

const { params } = useRoute();

const currentDate = new Date();
const weekdays = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
const weekdayName = weekdays[currentDate.getDay()];

const zodiacSign: string = params.zodiacSign as string;

const data: Record<string, Record<string, string>> = {
    rat: {
        image: "<img src='https://th.bing.com/th/id/OIP.m0Tp4DbdH9w_U9NKvm9BBQHaNK?rs=1&pid=ImgDetMain'>",
        text: "text 1",
    },
    ox: {
        image: "",
        text: "text 2",
    },
}

</script>