<template>
    <div class="signs">
        <NuxtLink to="/zodiacs/rat">
            <img src="https://i.pinimg.com/564x/40/44/32/404432d203d03570e148c0905f64cb2e.jpg">
            Rat
        </NuxtLink>
        <NuxtLink to="/zodiacs/ox">
            <img src="https://i.pinimg.com/564x/01/07/b1/0107b19de8000055982bbbae03dc4662.jpg">
            Ox
        </NuxtLink>
        <NuxtLink to="/zodiacs/tiger">
            <img src="https://i.pinimg.com/564x/ed/5d/3e/ed5d3eb98c99440fd092d6e1cf887ecf.jpg">
            Tiger
        </NuxtLink>
        <NuxtLink to="/zodiacs/rabbit">
            <img src="https://i.pinimg.com/564x/a0/f8/3d/a0f83d3cd0121709ef2e30f90c33e3d3.jpg">
            Rabbit
        </NuxtLink>
        <NuxtLink to="/zodiacs/dragon">
            <img src="https://i.pinimg.com/564x/ea/25/5d/ea255d93c5086a86628586d604fdd9dd.jpg">
            Dragon
        </NuxtLink>
        <NuxtLink to="/zodiacs/snake">
            <img src="https://i.pinimg.com/736x/c6/ff/bf/c6ffbf9a2153ec6dde07cc722e80823f.jpg">
            Snake
        </NuxtLink>
        <NuxtLink to="/zodiacs/horse">
            <img src="https://i.pinimg.com/564x/0c/54/0a/0c540a78f9d01a84f32f09de656352ac.jpg">
            Horse
        </NuxtLink>
        <NuxtLink to="/zodiacs/goat">
            <img src="https://i.pinimg.com/564x/12/8e/54/128e5453d538f5dcc8332cd22db45eda.jpg">
            Goat
        </NuxtLink>
        <NuxtLink to="/zodiacs/monkey">
            <img src="https://i.pinimg.com/564x/73/34/2c/73342c9b05c026476b64a4ff566f8e4e.jpg">
            Monkey
        </NuxtLink>
        <NuxtLink to="/zodiacs/rooster">
            <img src="https://i.pinimg.com/564x/5f/51/01/5f510126e327f47aea08d7e0a62bdb16.jpg">
            Rooster
        </NuxtLink>
        <NuxtLink to="/zodiacs/dog">
            <img src="https://i.pinimg.com/564x/c0/b0/50/c0b050422bf6c9837001b20db60cbecc.jpg">
            Dog
        </NuxtLink>
        <NuxtLink to="/zodiacs/pig">
            <img src="https://i.pinimg.com/564x/e8/88/8d/e8888da22e4a2c9eb5fb79fd3badef14.jpg">
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
.signs img{
    width: 100%;
    height: 70px;
    background:rgb(26, 15, 32);
    border-radius: 50%;
}
</style>