<template>
    <div class="signs">
        <NuxtLink to="/zodiacs/rat">
            Rat
        </NuxtLink>
        <NuxtLink to="/zodiacs/ox">
            Ox
        </NuxtLink>
        <NuxtLink to="/zodiacs/tiger">
            Tiger
        </NuxtLink>
        <NuxtLink to="/zodiacs/rabbit">
            Rabbit
        </NuxtLink>
        <NuxtLink to="/zodiacs/dragon">
            Dragon
        </NuxtLink>
        <NuxtLink to="/zodiacs/snake">
            Snake
        </NuxtLink>
        <NuxtLink to="/zodiacs/horse">
            Horse
        </NuxtLink>
        <NuxtLink to="/zodiacs/goat">
            Goat
        </NuxtLink>
        <NuxtLink to="/zodiacs/monkey">
            Monkey
        </NuxtLink>
        <NuxtLink to="/zodiacs/rooster">
            Rooster
        </NuxtLink>
        <NuxtLink to="/zodiacs/dog">
            Dog
        </NuxtLink>
        <NuxtLink to="/zodiacs/pig">
            Pig
        </NuxtLink>
    </div>  
</template>

<style>
.signs {
    display: flex;
    justify-content: space-between;
    border-bottom: 2px solid rgb(26, 15, 32);
}
.signs a {
    flex: 1;
    text-align: center;
    color: rgb(238, 228, 169);
    background-color: rgb(75, 12, 12);
    padding: 10px 20px;
    transition-duration: 300ms;
    text-decoration: none;
    font-size: 16px;
}
.signs a::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.signs a:hover {
-webkit-text-fill-color: rgb(161, 41, 41);
background-color: rgb(26, 15, 32);
}
</style>