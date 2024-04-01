<template>
    <PageHeader></PageHeader>
    <ZodiacHeader></ZodiacHeader>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />
    <h1>{{ zodiacSign }}</h1>

    <main>    
        <div class="r">
        <svg class="rp" url="https://danmarshall.github.io/google-font-to-svg-path/?font-select=ABeeZee&font-variant=regular&input-union=false&input-filled=true&input-kerning=true&input-separate=false&input-text=%E9%BC%A0&input-bezier-accuracy=&dxf-units=cm&input-size=200&input-fill=rgb%28238%2C+228%2C+169%29&input-stroke=rgb%28238%2C+228%2C+169%29&input-strokeWidth=0.25mm&input-fill-rule=evenodd">
        
        </svg>
        <div class="rs"> <p> {{ data[zodiacSign]?.summary }} </p>  
        </div>
        </div>
        <div class="per">
        <div class="pers"> <h1>Personality</h1>
        <p>
            {{ data[zodiacSign]?.personality_1 }}
        </p>
        <div class="person">
            <div class="perso"><h2>Strengths</h2>
                <ul style="list-style-type:circle">
                <li> {{ data[zodiacSign]?.strengths }} </li>
                <li> {{ data[zodiacSign]?.strengths_2}} </li>
                <li> {{ data[zodiacSign]?.strengths_3}} </li>
                <li> {{ data[zodiacSign]?.strengths_4}} </li>
                <li> {{ data[zodiacSign]?.strengths_5}} </li>
              </ul></div>
            <div class="perso"><h2>Weaknesses</h2> 
                <ul style="list-style-type:circle">
                <li>{{ data[zodiacSign]?.weaknesses}}</li>
                <li>{{ data[zodiacSign]?.weaknesses_2}}</li>
                <li>{{ data[zodiacSign]?.weaknesses_3}}</li>
                <li>{{ data[zodiacSign]?.weaknesses_4}}</li>
                <li>{{ data[zodiacSign]?.weaknesses_5}}</li>
              </ul>
            </div>
            <div class="persona"> 
            <p>
                {{ data[zodiacSign]?.personality_2 }}
            </p>
              </div>
        </div>
        </div>
        <div class="perr">
            <p>{{ data[zodiacSign]?.years}}</p>
            <table>
            <tr>
              <th>Year</th>
              <th>Lunar year start date</th>
              <th>Lunar year end date</th>
            </tr>
            <tr>
              <td> {{ data[zodiacSign]?.years_1 }}</td>
              <td>{{ data[zodiacSign]?.years_2 }}</td>
              <td>{{ data[zodiacSign]?.years_3 }}</td>
            </tr>
            <tr>
              <td>{{ data[zodiacSign]?.years_4 }}</td>
              <td>{{ data[zodiacSign]?.years_5 }}</td>
              <td>{{ data[zodiacSign]?.years_6 }}</td>
            </tr>
            <tr>
              <td>{{ data[zodiacSign]?.years_7 }}</td>
              <td>{{ data[zodiacSign]?.years_8 }}</td>
              <td>{{ data[zodiacSign]?.years_9 }}</td>
            </tr>
            <tr>
                <td>{{ data[zodiacSign]?.years_10 }}</td>
                <td>{{ data[zodiacSign]?.years_11 }}</td>
                <td>{{ data[zodiacSign]?.years_12 }}</td>
              </tr>
              <tr>
                <td>{{ data[zodiacSign]?.years_13 }}</td>
                <td>{{ data[zodiacSign]?.years_14 }}</td>
                <td>{{ data[zodiacSign]?.years_15 }}</td>
              </tr>  
              <tr>
                <td>{{ data[zodiacSign]?.years_16 }}</td>
                <td> {{ data[zodiacSign]?.years_17 }}</td>
                <td> {{ data[zodiacSign]?.years_18 }}</td>
              </tr>   
              <tr>
                <td>{{ data[zodiacSign]?.years_19 }}</td>
                <td> {{ data[zodiacSign]?.years_20 }}</td>
                <td>{{ data[zodiacSign]?.years_21 }}</td>
              </tr> 
              <tr>
                <td>{{ data[zodiacSign]?.years_22 }}</td>
                <td> {{ data[zodiacSign]?.years_23 }}</td>
                <td>{{ data[zodiacSign]?.years_24 }}</td>
              </tr>
              <tr>
                <td>{{ data[zodiacSign]?.years_25 }}</td>
                <td>{{ data[zodiacSign]?.years_26 }}</td>
                <td> {{ data[zodiacSign]?.years_27 }}</td>
              </tr> 
              <tr>
                <td>{{ data[zodiacSign]?.years_28 }}</td>
                <td>{{ data[zodiacSign]?.years_29 }}</td>
                <td>{{ data[zodiacSign]?.years_30}}</td>
              </tr>
            </table>
            </div>
            </div>
            <div class="sum">
            <p>
                {{ data[zodiacSign]?.overall}}
            </p>
            </div> 
            <div class="five">Five elements theory</div>
            <div class="elements">
            <div class="earth">
                <h2>Metal</h2>  
            <div class="dropdown">
            <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(238, 228, 169);"> 
              expand_circle_down
            </span>
            <div class="dropdown-content">
              <p>
                {{ data[zodiacSign]?.metal}}
              </p>
            </div>
            </div>
            </div>
              <div class="earth">
                <h2>Water</h2>    
              <div class="dropdown">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(238, 228, 169);">
                  expand_circle_down
                  </span>
                <div class="dropdown-content">
                  <p>
                    {{ data[zodiacSign]?.water}}
                </p>
                  </div>
                </div>
              </div>
              <div class="earth">
                  <h2>Wood</h2>   
              <div class="dropdown">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(238, 228, 169);">
                  expand_circle_down
                  </span>
                <div class="dropdown-content">
                    <p>
                        {{ data[zodiacSign]?.wood}}
                    </p>
                </div>
                </div>
                </div>
              <div class="earth">
                  <h2>Fire</h2>
              <div class="dropdown">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(238, 228, 169);">
                  expand_circle_down
                  </span>
                  <div class="dropdown-content">
                  <p> 
                    {{ data[zodiacSign]?.fire}}
                </p>
                </div>
              </div>
              </div>
              <div class="earth">
              <h2>Earth</h2>
              <div class="dropdown">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(238, 228, 169);">
                  expand_circle_down
                  </span>
                <div class="dropdown-content">
                  <p>
                    {{ data[zodiacSign]?.earth}}
                  </p>
                </div>
                </div>  
                </div>
            </div>
            <div class="compatibility">
              <div class="comp">
              <h1>Compatibility</h1>
              <p>
                {{ data[zodiacSign]?.compatibility }}
            </p>
                <h2>Best matches</h2>
                <div class="heart">
                  <span class="material-symbols-outlined">
                  favorite
                </span>
                </div>
              </div>
                <div class="co">
                <div class="com">
                <h3>
                    {{ data[zodiacSign]?.best }}
                </h3>
                </div>
                <div class="compa">
                <p>
                    {{ data[zodiacSign]?.best_more }}
                </p>
                <div class="gender">
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_more }}
                  </p>
                  </div>
                  </div>
                  </div>
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender_reverse }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_reverse_more }}
                  </p>
                </div>
                </div>
                </div>
                </div>
                </div>
                </div>
          </div>      
            <div class="ove">
            <div class="lucky">
              <h2>Unlucky and lucky things</h2>
              </div>
              <div class="u">
              <div class="things"><h2>Lucky things</h2>
                <ul style="list-style-type:circle">
                <li><div class="l"><h4>numbers - </h4><p>{{ data[zodiacSign]?.lucky_1 }} </p></div></li>
                <li><div class="l"><h4>colors - </h4><p> {{ data[zodiacSign]?.lucky_2 }}</p></div></li>
                <li><div class="l"><h4>directions - </h4><p> {{ data[zodiacSign]?.lucky_3 }}</p></div></li>
                <li><div class="l"><h4>flowers - </h4><p>{{ data[zodiacSign]?.lucky_4 }} </p></div></li>
                <li><div class="l"><h4>months - </h4><p> {{ data[zodiacSign]?.lucky_5 }}</p></div></li>
                <li><div class="l"><h4>gemstones - </h4><p> {{ data[zodiacSign]?.lucky_6 }}</p></div></li>
                <li><div class="l"><h4>charms - </h4><p>{{ data[zodiacSign]?.lucky_7 }}</p></div></li>
              </ul></div>
            <div class="things"><h2>Unlucky things</h2> 
                <ul style="list-style-type:circle">
                  <li><div class="l"><h4>numbers - </h4><p>{{ data[zodiacSign]?.unlucky_1 }}</p></div></li>
                  <li><div class="l"><h4>colors - </h4><p>{{ data[zodiacSign]?.unlucky_2 }}</p></div></li>
                  <li><div class="l"><h4>directions - </h4><p>{{ data[zodiacSign]?.unlucky_3 }}</p></div></li>
                  <li><div class="l"><h4>months - </h4><p>{{ data[zodiacSign]?.unlucky_4 }}</p></div></li>
                  <li><div class="l"><h4>gemstones - </h4><p>{{ data[zodiacSign]?.unlucky_5 }}</p></div></li>
              </ul>
            </div>    
            </div>
            </div>
        </main>
        <footer>
            <div class="out">
                <p>Check out the <NuxtLink to="/zodiacs/rat/daily_horoscope">
               daily
            </NuxtLink>/<a href="rat_yearlyhoroscope.html">yearly</a>
                horoscope for {{ data[zodiacSign]?.out }}</p>
            
            </div>
        </footer>
</template>

<script setup lang="ts">

const { params } = useRoute();
const zodiacSign: string = params.zodiacSign as string;

const data: Record<string, Record<string, string>> = {
    rat: {
        summary: "In Chinese astrology, the Rat is the first sign of the Chinese zodiac cycle, representing the beginning of a new cycle. People born in the Year of the Rat are believed to possess certain personality traits and characteristics based on the attributes associated with this animal symbol.",
        personality_1: "Rats are known for their resourcefulness and ability to find solutions to problems. They are intelligent, clever and charming. Thanks to their wit and charism they can easily win people over. These creatures are often flexible and able to adjust to changing circumstances. People born under this sign are ambitious and driven individuals. They are not afraid to work hard to achieve their goals and are often determined to succeed. Despite their inteligence they are still outgoing and enjoy the company of others. While Rats are ambitious, they are also cautious by nature. They tend to weigh their options carefully before making decisions and are not prone to taking unnecessary risks. They are good at managing their finances and are often careful with their money.",
        strengths: "clever",
        strengths_2: "adaptable",
        strengths_3: "ambitious",
        strengths_4: "outgoing",
        strengths_5: "prudent",
        weaknesses: "restless",
        weaknesses_2: "manipulative",
        weaknesses_3: "sensitive to criticism",
        weaknesses_4: "overly competitive",
        weaknesses_5: "stubborn",
        personality_2: "Lorem Ipsum jest tekstem stosowanym jako przykładowy wypełniacz w przemyśle poligraficznym. Został po raz pierwszy użyty w XV w. przez nieznanego drukarza do wypełnienia tekstem próbnej Lorem Ipsum Lorem Ipsum jest tekstem stosowanym jako przykładowy wypełniacz w przemyśle jest tekstem stosowanym jako przykładowy wypełniacz w przemyśle",
        years: "Years of the Rat",
        years_1: "1924",
        years_2: "February 5, 1924 ",
        years_3:"January 23, 1925",
        years_4:"1936",
        years_5:"January 24, 1936",
        years_6:"February 10, 1937",
        years_7:"1948",
        years_8:"February 10, 1948",
        years_9:"January 28, 1949",
        years_10:"1960",
        years_11:"January 28, 1960",
        years_12:"February 14, 1961",
        years_13:"1972",
        years_14:"February 15, 1972",
        years_15:"February 2, 1973",
        years_16:"1984",
        years_17:"February 2, 1984",
        years_18:"February 19, 1985",
        years_19:"1996",
        years_20:"February 19, 1996",
        years_21: "February 6, 1997",
        years_22: "2008 ",
        years_23: "February 6, 2008",
        years_24: "January 25, 2009",
        years_25: "2020",
        years_26: "January 25, 2020",
        years_27: "February 11, 2021",
        years_28: "2032",
        years_29: "February 11, 2032",
        years_30: "January 30, 2033",
        overall: "Rats are clever, quick thinkers; successful, but content with living a quiet and peaceful life.",
        metal: "Metal Rats have a thirst for knowledge and will voraciously learn everything that interests them. In contrast, they tend to focus on the subjective in their thinking and may experience occasional, albeit well-hidden, emotional turbulence. They may exhibit greed like all Rat personalities, preferring flashy objects and living in a more opulent way. If they manage to control these tendencies, Metal Rats will likely build a great future for themselves.",
        water: "Water Rats are agile-minded, authoritative, and strategic, with success coming later in life in the form of a prosperous blooming closer to retirement. Think of a trickle of water that’s capable of wearing away a mountain! This group is intelligent but, like other Rat natives, tends to be conservative and cautious. They prefer sailing with the current rather than against it, which seems to be the origin of their additional wealth.",
        wood: "The typical Wood Rat is dependable and principled to a fault. This means either Wood Rats will find it difficult to climb the corporate ladder or else enjoy professional respect and a solid reputation. Outside work, they’re able to maintain a harmonious family life with traditional values. They like to have security in their lives above all, which may be why Wood Rats work so hard on their careers.",
        fire: "Fire Rats are intelligent and capable, making them valuable team players when striving for social harmony or material success. They often appear chivalrous at heart, with a generosity not usually found in other Rat natives. Fire Rats can be emotional and often lack discipline. They’ll do well in careers involving communication or the arts, although their fiery nature may cause great ups and downs no matter what career they choose.",
        earth: "Earth Rats are blessed with a stable character, affording them a lively and happy life without much anguish. They’re also more adaptable than other zodiacs with the Earth element, making them well-liked in any group. They dislike taking risks and will never gamble, preferring instead to accumulate wealth over time. Earth Rats are dependable, but at times selfish and stingy with money—giving to the undeserving is risky, after all!",
        compatibility: "In matters of the heart, Rats are soft-spoken, frank, and intuitive. They are eager and capable partners, although they can be very vain at times—thankfully, a rare occurrence that doesn’t spoil the total package. They’re attentive to the object of their desire and will show intense interest in getting to know the other person. Being in a relationship with them is never boring and will likely involve mutual affection, even for less traditionally compatible animals like the Rooster or Snake.",
        best: "Rat and Dragon",
        best_more: "Rat and Dragon may appear diametrically opposed to some, with the Rat being a careful workhorse and the Dragon, a magnanimous leader. But, in fact, those are the very traits that make them complement each other, leading to a surprisingly good relationship. This love compatibility is at its best when the Dragon leads at a high level, making the bigger decisions the Rat struggles with, while the Rat takes care of the details that the Dragon will likely overlook.",
        gender: "Female Rat and Male Dragon",
        gender_more: "This pairing will find their income on the up-and-up, while spending will naturally be curbed. Having their livelihood thus assured, the Rat can truly blossom in security. The Dragon will be energetic and bold, while the Rat is shrewd, dexterous, and sociable. This pairing will enjoy mutual trust in marriage—with the Rat almost worshiping her Dragon mate as a hero.",
        gender_reverse: "Female Dragon and Male Rat",
        gender_reverse_more: "Both partners are straightforward and courageous. They instill trust and mutual respect in their mate while leaving ample personal space for the other’s need for independence. Both Rat and Dragon share a positive and upbeat view on life. You will discover plenty of joy in married life that may not be apparent to outside observers.",
        lucky_1: "2, 3",
        lucky_2: "Blue, Gold",
        lucky_3: "East",
        lucky_4: "Lily, African Violet, Orchid",
        lucky_5: "March, June, September, December",
        lucky_6: "Garnet, Amethyst, Sapphire",
        lucky_7: "Rat-shaped figurines ",
        unlucky_1: "5, 9",
        unlucky_2: "Yellow, Brown",
        unlucky_3: "West, Southwest",
        unlucky_4: "February, May, August, November",
        unlucky_5: "Ruby",
        out: "Rat",
    },
    ox: {
        summary: "lorem ipsum"
    }
}

</script>

<style>
.r {
display:flex;
flex-direction: row; 
padding: 30px; 
align-items: center; 
}
.r p{
padding-left: 30px;
padding-right: 10px;
color: rgb(238, 228, 169);
}
.rs p{
    padding: 1px 30px;
    color: rgb(238, 228, 169);
    text-align: justify;
    font-size: larger;
    Line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;   
}
.rs p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.rs {
background-color: rgb(161, 41, 41);
outline: 10px double rgb(238, 228, 169);
}
.rp{
font-size: 100px;
float: left;
}
.rp svg::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.per{
display: flex;    
flex-direction: row;
align-items: center;
padding: 30px;
}
.pers {
border-right: 10px double rgb(161, 41, 41);    
}
.pers h1{
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(161, 41, 41);
    padding-left: 30px;
    padding-top: 30px;  
    letter-spacing: 1px;     
}
.pers h1::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.pers p {
    padding: 1px 30px;
    color: rgb(238, 228, 169);
    text-align: justify;
    font-size: larger;
    Line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
}
.pers p::first-letter{
font-size: xx-large;   
color: rgb(161, 41, 41); 
font-family: fantasy;
}
.pers p::selection {
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.perr{
padding-left: 30px;   
}
.perr p{
    font-size: x-large;  
    font-family: fantasy;
    color: rgb(161, 41, 41);
    padding-right: 30px;  
    letter-spacing: 1px;   
}
.perr p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.perr table {
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;    
    border: 2px solid rgb(238, 228, 169);
    border-collapse: collapse;
}
.perr th, td {
    border: 1px solid rgb(238, 228, 169);
    text-align: left;
    padding: 8px;    
    color: rgb(238, 228, 169);
    }
.perr tr:hover{
        background-color:rgb(75, 12, 12);    
}    

.perr td::selection{
        color: rgb(143, 143, 143);
        background: rgb(75, 12, 12);    
    }
.perr th::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.person {
    display: flex; 
    justify-content: space-between;
    gap: 20px; 
    padding: 20px; 
    background-color: rgb(26, 15, 32); 
    }
.perso h2{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    height: 50px;
    color: rgb(26, 15, 32);
    }
.perso h2::selection{
        color: rgb(143, 143, 143);
        background: rgb(75, 12, 12);    
    }    
.person p{
    padding: 1px 30px;
    color: rgb(238, 228, 169);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;   
    text-align: center;
    flex-direction: row-reverse;
    }
.person p::selection{
        color: rgb(143, 143, 143);
        background: rgb(75, 12, 12);    
    }    
.perso li {
    padding: 1px 30px;
    color: rgb(26, 15, 32);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;   
    text-align: left;
} 
.perso li::marker{
    color: rgb(161, 41, 41);
    font-size: 23px;   
}
.perso li::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.perso p {
    align-items: flex-start;  
   }
.perso p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}   
.perso{
    display: flex;
    flex-direction: column;  
    width: 300px;
    text-align: center;
    background-color: rgb(143, 143, 143);     
    }
.persona p{
    padding: 1px 30px;
    color: rgb(238, 228, 169);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
}
.persona p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.sum p {
font-size: 70px;  
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
padding: 30px;
text-align: center;
padding-top: 80px;
padding-bottom: 80px;
font-weight: bolder;
font-variant: small-caps;
}
.sum {
background-image: url(https://i.pinimg.com/564x/29/cc/06/29cc0670039ecfcf49a96ed26e800dde.jpg);    
}
.sum p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.five {
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(238, 228, 169); 
    letter-spacing: 1px;
    justify-content: center;   
}
.elements{
display: flex;    
flex-direction: row;
justify-content: space-around;
}
.dropdown {
padding-left: 70px;
padding-right: 80px;    
}
  
.dropdown-content {
    display: none;
    background-color: rgb(143, 143, 143);
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    padding: 20px;
    z-index: 1;
  }
.dropdown-content p{ 
    color: rgb(26, 15, 32);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    text-align: justify;
    padding-right: 20px;
    padding-left: 20px;
} 
.dropdown:hover .dropdown-content {
    display: block;
    justify-content: baseline;
  }
.dropdown span {
    border-radius: 25px;
    background: rgb(161, 41, 41);
}
.earth {
display: flex;    
flex-direction: column;
padding-bottom: 50px;
}
.earth h2{
padding-left: 60px;   
padding-right: 50px; 
letter-spacing: 1px;
color: rgb(238, 228, 169);
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.compatibility {
padding: 30px;
}
.heart span {
position: absolute;
left: 30px;
top: 2400px;
z-index: -1;
width: 20%;
color: rgb(75, 12, 12);
}
.heart{
    font-size: xxx-large;  
    font-family: fantasy
}
.comp h1{
    display: flex;
    justify-content: center;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(161, 41, 41); 
    letter-spacing: 1px;
    justify-content: center;
}
.comp p{
    color: rgb(238, 228, 169);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    text-align: justify;    
}
.comp h2{
    color: rgb(161, 41, 41);
    font-size: xx-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
    font-variant: small-caps;     
}
.co{
    display: flex;
    flex-direction: row;
    padding-bottom: 30px;
}
.co h3{
flex-wrap: nowrap;
}
.compa {
padding: 30px;    
border-left: 10px double rgb(75, 12, 12);   
}
.compa p{
display: flex;
flex-wrap: wrap;
color: rgb(238, 228, 169);
font-size: larger;
line-height: 30px;
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
letter-spacing: 1px; 
text-align: justify;
}
.com h3{
    color: rgb(161, 41, 41);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
    width: 150px;
}
.g {
padding: 30px; 
padding-top: 5px;
}
.kw {
background-color: rgb(143, 143, 143);
text-align: center;
}
.kw h2 {
    padding: 30px;
    padding-bottom: 0px; 
}
.gender {
    gap: 20px; 
    padding: 20px; 
    background-color: rgb(26, 15, 32);  
}
.gender h2{
    color: rgb(75, 12, 12);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
}
.gender span{
    border-radius: 25px;
    background: rgb(75, 12, 12);
}
.g-content {
        display: none;
        background-color: rgb(161, 41, 41);
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        padding: 20px;
        z-index: 1;
}
.g-content p{ 
        color: rgb(238, 228, 169);
        font-size: larger;
        line-height: 30px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        letter-spacing: 1px; 
    } 
.g:hover .g-content {
        display: block;
        justify-content: baseline;
      }
.ove {
    background-color: rgb(75, 12, 12);  
    padding-bottom: 50px;
}
.lucky{
display: flex;  
justify-content: center; 
padding-bottom: 30px; 
padding-top: 50px;
}
.lucky h2{
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(143, 143, 143); 
    letter-spacing: 1px;
    justify-content: center;
}
.u {
display: flex; 
flex-direction: row;  
justify-content: space-evenly;
}
.things li::marker{
    color: rgb(161, 41, 41);
    font-size: 23px;   
}
.things {
    background-color: rgb(143, 143, 143);
    border-radius: 20px;
    padding: 20px;
    width: 40%;
    color:rgb(26, 15, 32);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
}
.things p{
    display: flex;
    padding-left: 10px;
    align-items: center;
}
.l {
    display: flex;
    flex-direction: row;
}
.out p{
    color: rgb(238, 228, 169);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
}
.out a{
color: rgb(161, 41, 41); 
}
.out a:hover{
    color:rgb(75, 12, 12);
}
</style>
