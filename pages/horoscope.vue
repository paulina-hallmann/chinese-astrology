<template>
    <PageHeader></PageHeader>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />
    <main>
        <div class="Check">
            <p>Check out horoscope for your sign</p>
        </div>
        <div class="ho">
                <div v-for="zodiacSign in zodiacSigns">
                    <p style="text-transform: capitalize;">{{ zodiacSign }}</p>
                        <div class="horosc">
                            <NuxtLink :to="'/daily_horoscope/' + zodiacSign">
                                daily horoscope
                            </NuxtLink>
                </div>
            </div>
        </div>        
    </main>
</template>

<style>
.Check P {
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(26, 15, 33); 
    letter-spacing: 1px;
    justify-content: center;
    padding: 30px;
    padding-bottom: 0px;
}
.Check p::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.ho {
    padding-left: 100px;
    padding-right: 100px;
    padding-bottom: 100px;
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.ho p{
    color: rgb(75, 12, 12);
    font-size: xx-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    padding: 30px;
    font-variant: small-caps;
    text-align: center;
}
.ho p::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.ho {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-evenly;
    gap: 10px;
}
.horosc {
    background-color: rgb(161, 41, 41); 
    border-radius: 10px;
    border: 3px solid rgb(26, 15, 33);
    gap: 30px;
    width: 200px;
    height: 50px;
    align-items: center;
    display: flex;
    justify-content: center;
}
.horosc a{
    display: flex;
    text-align: center;
    padding-top: 10px;
    padding-bottom: 15px;
    padding: 5px;
    color: rgb(238, 228, 169);
    text-decoration: none;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
}
.horosc a::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.horosc a:hover {
    color: rgb(75, 12, 12);
}

</style>

<script setup lang="ts">
    const zodiacSigns: string[] = [
        'rat',
        'ox',
        'tiger',
        'rabbit',
        'dragon',
        'snake',
        'horse',
        'goat',
        'monkey',
        'rooster',
        'dog',
        'pig',
    ]
</script>