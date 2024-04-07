
 <template>
    <div class="horoscope">
    <PageHeader/>

        <main>
            <div class="d">
                <div class="dail">
                    <div v-html="data[zodiacSign]?.image"></div>
                    <h2>
                        The daily horoscope for
                        <span style="text-transform: capitalize;">{{ zodiacSign }}</span>
                    </h2>
                    <p>
                        {{data[zodiacSign]?.text}}   
                    </p>
                </div>
                <div class="da">
                    <p>{{ currentDate.toLocaleString('en-US', { month: 'long' }) }} {{ currentDate.getFullYear() }}</p>
                    <h1>{{ currentDate.getDate() }}</h1>
                    <h3>{{ weekdayName }}</h3>
                </div>
            </div>       
        </main>
        <footer>
            <div class="footer"></div>
        </footer>
    </div>
</template>

<style>
.horoscope {
    background-color: rgb(26, 15, 33);
}
.d {
    display: flex;
    flex-direction: row;
    padding: 30px;
}
.d img::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.da {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: rgb(238, 228, 169);
    width: 80%;
    padding-top: 0px;
    border-top: 20px double rgb(75, 12, 12);
    border-bottom: 20px double rgb(75, 12, 12);
    font-variant: small-caps;
    height: 510px;
}
.da h3::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.da h3{
    color:rgb(26, 15, 33);
    padding-bottom: 20px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    font-size: x-large;
}
.da h1{
    font-size: 200px;
    margin: 0px;
    color:rgb(75, 12, 12);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
}
.da h1::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.da p{
background-color: rgb(161, 41, 41);
width: 100%;
padding-bottom: 15px;
padding-top: 15px;
text-align: center;
color: rgb(26, 15, 33);
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
letter-spacing: 1px; 
font-size: xx-large;
}
.da p::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.dail h2 {
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(238, 228, 169); 
    letter-spacing: 1px;
    padding-bottom: 0px;    
}
.dail h2::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.dail img{
    display: flex;
    align-items: center;
    border-radius: 50%; 
    height: 200px;
    text-align: center;
}
.dail{
    display: flex;
    justify-content: center;
    flex-direction: column;
    padding-right: 30px;
    padding-left: 30px;
    align-items: center;
    width: 100%;
}
.dail p{
color: rgb(238, 228, 169);
font-size: larger;
line-height: 30px;
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
letter-spacing: 1px; 
text-align: center;
width: 400px;
}
.dail p::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.dail span::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
}
.footer{
    height:100%;
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
        image: "<img src='https://i.pinimg.com/564x/40/44/32/404432d203d03570e148c0905f64cb2e.jpg'>",
        text: "Get moving today. This day will inspire you to make things happen. Exercise, errands, and work ought to keep your mind off something that would ordinarily distract you. Stay busy.",
    },
    ox: {
        image: "<img src='https://i.pinimg.com/564x/01/07/b1/0107b19de8000055982bbbae03dc4662.jpg'>",
        text: "Borrowing money is such a downer, but don't get caught up in the drama of it all. Things happen. Make sure your finances are in order so that you can survive the next blow that may come.",
    },
    tiger: {
        image: "<img src='https://i.pinimg.com/564x/ed/5d/3e/ed5d3eb98c99440fd092d6e1cf887ecf.jpg'>",
        text: "If you have the will but can't find the way, be patient. Your desires will lead you to the place and the moment for action. Just make sure you're prepared for that moment.",
    },
    rabbit: {
        image: "<img src='https://i.pinimg.com/564x/a0/f8/3d/a0f83d3cd0121709ef2e30f90c33e3d3.jpg'>",
        text: "You may not be as sharp as usual, but that's okay. Work on creative pursuits and leave the critical thinking for another time. As long as you're making some sort of progress, you can feel good.",
    },
    dragon: {
        image: "<img src='https://i.pinimg.com/564x/ea/25/5d/ea255d93c5086a86628586d604fdd9dd.jpg'>",
        text: "You want to cut back on sugary treats, but that doesn't mean you have to deny yourself all pleasure. You can pay attention to your intake and still enjoy yourself. Don't go overboard.",
    },
    snake: {
        image: "<img src='https://i.pinimg.com/736x/c6/ff/bf/c6ffbf9a2153ec6dde07cc722e80823f.jpg'>",
        text: "Get your creative juices flowing. An idea of yours might just impress the right person. Don't be afraid to speak up about it to your boss or pitch a client a new project. Have faith in your abilities.",
    },
    horse: {
        image: "<img src='https://i.pinimg.com/564x/0c/54/0a/0c540a78f9d01a84f32f09de656352ac.jpg'>",
        text: "Someone's authoritative attitude might be rubbing you the wrong way. Instead of snapping and trying to take back control, avoid any interaction. It's unlikely either of you will back down.",
    },
    goat: {
        image: "<img src='https://i.pinimg.com/564x/12/8e/54/128e5453d538f5dcc8332cd22db45eda.jpg'>",
        text: "It's time to bury the hatchet. There's no use carrying around resentment, no matter what the original cause. The stress of it all only hurts you. It's time to let it go. Your pride can handle it. ",
    },
    monkey: {
        image: "<img src='https://i.pinimg.com/564x/73/34/2c/73342c9b05c026476b64a4ff566f8e4e.jpg'>",
        text: "Keep your eyes on the prize. Hold tight to the outcome you want. See only success and prosperity in your future. If that's hard, pretend you're an actor playing the part of someone who believes.",
    },
    rooster: {
        image: "<img src='https://i.pinimg.com/564x/5f/51/01/5f510126e327f47aea08d7e0a62bdb16.jpg'>",
        text: "It might be time to cut all of the drama out of your life. This could mean curbing your temper and watching how you treat others. Make an effort to be kind, calm, and mature today.",
    },
    dog: {
        image: "<img src='https://i.pinimg.com/564x/c0/b0/50/c0b050422bf6c9837001b20db60cbecc.jpg'>",
        text: "Are you the one who's always enforcing order and structure at work and home? This could get you far today, so stick to the plan. You'll be recognized for your efforts, and you deserve it.",
    },
    pig: {
        image: "<img src='https://i.pinimg.com/564x/e8/88/8d/e8888da22e4a2c9eb5fb79fd3badef14.jpg'>",
        text: "Don't take someone's criticism to heart. Ignore an irritable coworker or disgruntled store employee. Avoid people who are in a foul mood. You don't need the negativity in your life now.",
    },
}

</script>