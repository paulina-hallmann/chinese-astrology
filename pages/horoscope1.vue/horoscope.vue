<template>
    <PageHeader></PageHeader>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />
    <main>
        <div class="Check">
            <p>Check out horoscope for your sign!!</p>
        </div>
        <div class="h">
        <div class="ho">
        <p>Rat</p>
        <div class="horoscop">
        <div class="horosc">
            <NuxtLink to="/horoscope/rat/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/rat/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
        </div>
        <p>Dragon</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/dragon/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/dragon/yearly">
                yearly horoscope
            </NuxtLink>
        </div>                                            
           </div>                                                                                                                                                                                                                                                                                     
        <p>Monkey</p>                     
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/monkey/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/monkey/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
            </div>
        <div class="hor">
        <p>Ox</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/ox/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/ox/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        <p>Snake</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/snake/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/snake/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        <p>Rooster</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/rooster/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/rooster/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        </div>
        <div class="horo">
        <p>Tiger</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/tiger/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/tiger/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        <p>Horse</p> 
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/horse/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/horse/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>   
        <p>Dog</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/dog/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/dog/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        </div>
        <div class="horos">
        <p>Rabbit</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/rabbit/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/rabbit/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>
        <p>Goat</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/goat/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/goat/yearly">
                yearly horoscope
            </NuxtLink>
        </div>
            </div>    
        <p>Pig</p>
        <div class="horoscop">
            <div class="horosc">
                <NuxtLink to="/horoscope/pig/daily">
                daily horoscope
            </NuxtLink>
        </div>
        <div class="horosco">
            <NuxtLink to="/horoscope/pig/yearly">
                yearly horoscope
            </NuxtLink>
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
    flex-direction: column;
    align-items: center;
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

<script>

</script>