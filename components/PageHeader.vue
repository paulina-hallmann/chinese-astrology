<template>
    <header>
        <div class="navigation">
            <NuxtLink to="/">
                Home
            </NuxtLink>  
            <NuxtLink to="/zodiacs">
                Zodiac signs
            </NuxtLink>
            <NuxtLink to="/horoscope">
                Horoscope
            </NuxtLink>
        </div>  
    </header>
</template>

<style>
    header {
        position: sticky;
        top: 0;
    }
    
    .navigation {
        display: flex;
        justify-content: center;
        border-bottom: 20px double rgb(161, 41, 41);
        background-color: rgb(75, 12, 12);
    }

    .navigation a {
        flex: 1;
        text-align: center;
        color: rgb(26, 15, 32);
        background-color: rgb(161, 41, 41);
        padding: 10px 20px;
        transition-duration: 300ms;
        text-decoration: none;
        font-size: 25px;
    }
    .navigation a::selection{
        color: rgb(143, 143, 143);
        background: rgb(75, 12, 12);    
    }

    .navigation a:hover {
        color: rgb(238, 228, 169);
        background-color: rgb(75, 12, 12);
    }
</style>