<template>
    <PageHeader></PageHeader>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />
    <main>
        <div class="Check">
            <p>Check out horoscope for your sign!!</p>
        </div>
        <div class="h">
            <div class="ho">
                <div v-for="zodiacSign in zodiacSigns">
                    <p style="text-transform: capitalize;">{{ zodiacSign }}</p>
                    <div class="horoscop">
                        <div class="horosc">
                            <NuxtLink :to="'/daily_horoscope/' + zodiacSign">
                                daily horoscope
                            </NuxtLink>
                        </div>
                        <div class="horosco">
                            <NuxtLink to="#">
                                yearly horoscope
                            </NuxtLink>
                        </div>
                    </div>
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
    color: rgb(143, 143, 143); 
    letter-spacing: 1px;
    justify-content: center;
    padding: 30px;
    padding-bottom: 0px;
}
.h {
    padding-left: 100px;
    padding-right: 100px;
    padding-bottom: 100px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    gap: 50px;
}
.h p{
    color: rgb(238, 228, 169);
    font-size: xx-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    padding: 30px;
    font-variant: small-caps;
}
.ho {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-evenly;
    gap: 10px;
}
.hor {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.horo {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.horos {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.horosco {
    background-color: rgb(161, 41, 41);
    border-radius: 10px;
    border: 3px solid rgb(238, 228, 169);
}
.horosc {
    background-color: rgb(161, 41, 41); 
    border-radius: 10px;
    border: 3px solid rgb(238, 228, 169);
}
.horoscop {
    display: flex;
    flex-direction: row;
    gap: 20px;
    background-color: rgb(26, 15, 32);
}
.horoscop a{
    padding-top: 10px;
    padding-bottom: 15px;
    display: flex;
    text-align: center;
    color: rgb(238, 228, 169);
    text-decoration: none;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
}
.horoscop a:hover {
    color: rgb(75, 12, 12);
}

</style>

<script setup lang="ts">
    const zodiacSigns: string[] = [
        'rat',
        'ox',
        'goat',
        'dragon',
        'snake',
        'pig',
        'dog',
        'rooster',
        'tiger',
        'rabbit',
    ]
</script>