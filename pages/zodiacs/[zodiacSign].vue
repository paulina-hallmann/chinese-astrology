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
                <h4>{{ data[zodiacSign]?.metal_years}}</h4> 
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
                <h4>{{ data[zodiacSign]?.water_years}}</h4>  
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
                  <h4>{{ data[zodiacSign]?.wood_years}}</h4>
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
                  <h4>{{ data[zodiacSign]?.fire_years}}</h4>
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
              <h4>{{ data[zodiacSign]?.earth_years}}</h4>
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
                <div class="co">
                <div class="com">
                <h3>
                    {{ data[zodiacSign]?.best_2 }}
                </h3>
                </div>
                <div class="compa">
                <p>
                    {{ data[zodiacSign]?.best_more_2 }}
                </p>
                <div class="gender">
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender_2 }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_more_2 }}
                  </p>
                  </div>
                  </div>
                  </div>
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender_reverse_2 }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_reverse_more_2 }}
                  </p>
                </div>
                </div>
                </div>
                </div>
                </div>
                </div>
                <div class="co">
                <div class="com">
                <h3>
                    {{ data[zodiacSign]?.best_3 }}
                </h3>
                </div>
                <div class="compa">
                <p>
                    {{ data[zodiacSign]?.best_more_3 }}
                </p>
                <div class="gender">
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender_3 }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_more_3 }}
                  </p>
                  </div>
                  </div>
                  </div>
                <div class="kw">
                <h2>{{ data[zodiacSign]?.gender_reverse_3 }}</h2>
                <div class="g">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(143, 143, 143);">
                    expand_circle_down
                </span>
                <div class="g-content">
                  <p>
                    {{ data[zodiacSign]?.gender_reverse_more_3 }}
                  </p>
                </div>
                </div>
                </div>
                </div>
                </div>
                </div>
                <div class="comp">
                    <h2>Worst matches</h2>
                </div>
                <div class="co">
                <div class="com">
                <h3>
                    {{ data[zodiacSign]?.worst }}
                </h3>
                </div>
                <div class="compa">
                <p>
                    {{ data[zodiacSign]?.worst_more }}
                </p>
            </div>
        </div>
        <div class="co">
                <div class="com">
                <h3>
                    {{ data[zodiacSign]?.worst_2 }}
                </h3>
                </div>
                <div class="compa">
                <p>
                    {{ data[zodiacSign]?.worst_more_2 }}
                </p>
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
        strengths: "resourcefulness",
        strengths_2: "adaptability",
        strengths_3: "ambition",
        strengths_4: "intelligence",
        strengths_5: "charm",
        weaknesses: "restlessness",
        weaknesses_2: "impulsiveness",
        weaknesses_3: "manipulativeness",
        weaknesses_4: "indecisiveness",
        weaknesses_5: "opportunism",
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
        metal_years: "1960, 2020",
        water: "Water Rats are agile-minded, authoritative, and strategic, with success coming later in life in the form of a prosperous blooming closer to retirement. Think of a trickle of water that’s capable of wearing away a mountain! This group is intelligent but, like other Rat natives, tends to be conservative and cautious. They prefer sailing with the current rather than against it, which seems to be the origin of their additional wealth.",
        water_years: "1972, 2032",
        wood: "The typical Wood Rat is dependable and principled to a fault. This means either Wood Rats will find it difficult to climb the corporate ladder or else enjoy professional respect and a solid reputation. Outside work, they’re able to maintain a harmonious family life with traditional values. They like to have security in their lives above all, which may be why Wood Rats work so hard on their careers.",
        wood_years: "1924, 1984",
        fire: "Fire Rats are intelligent and capable, making them valuable team players when striving for social harmony or material success. They often appear chivalrous at heart, with a generosity not usually found in other Rat natives. Fire Rats can be emotional and often lack discipline. They’ll do well in careers involving communication or the arts, although their fiery nature may cause great ups and downs no matter what career they choose.",
        fire_years: "1936, 1996",
        earth: "Earth Rats are blessed with a stable character, affording them a lively and happy life without much anguish. They’re also more adaptable than other zodiacs with the Earth element, making them well-liked in any group. They dislike taking risks and will never gamble, preferring instead to accumulate wealth over time. Earth Rats are dependable, but at times selfish and stingy with money—giving to the undeserving is risky, after all!",
        earth_years: "1948, 2008",
        compatibility: "In matters of the heart, Rats are soft-spoken, frank, and intuitive. They are eager and capable partners, although they can be very vain at times—thankfully, a rare occurrence that doesn’t spoil the total package. They’re attentive to the object of their desire and will show intense interest in getting to know the other person. Being in a relationship with them is never boring and will likely involve mutual affection, even for less traditionally compatible animals like the Rooster or Snake.",
        best: "Rat and Dragon",
        best_more: "Rat and Dragon may appear diametrically opposed to some, with the Rat being a careful workhorse and the Dragon, a magnanimous leader. But, in fact, those are the very traits that make them complement each other, leading to a surprisingly good relationship. This love compatibility is at its best when the Dragon leads at a high level, making the bigger decisions the Rat struggles with, while the Rat takes care of the details that the Dragon will likely overlook.",
        gender: "Female Rat and Male Dragon",
        gender_more: "This pairing will find their income on the up-and-up, while spending will naturally be curbed. Having their livelihood thus assured, the Rat can truly blossom in security. The Dragon will be energetic and bold, while the Rat is shrewd, dexterous, and sociable. This pairing will enjoy mutual trust in marriage—with the Rat almost worshiping her Dragon mate as a hero.",
        gender_reverse: "Female Dragon and Male Rat",
        gender_reverse_more: "Both partners are straightforward and courageous. They instill trust and mutual respect in their mate while leaving ample personal space for the other’s need for independence. Both Rat and Dragon share a positive and upbeat view on life. You will discover plenty of joy in married life that may not be apparent to outside observers.",
        best_2: "Rat and Monkey",
        best_more_2: "This is a relationship based on mutual admiration and a craving for the same type of lifestyle. Both zodiacs value a quick wit and a propensity to abundance, which they’ll find in spades in their partner. On top of that, the Rat will appreciate the Monkey’s extra logical mind, which they lack themselves, while the Rat seems the one capable of inspiring the usually self-centered Monkey to be a team player.",
        gender_2: "Female Rat and Male Monkey",
        gender_more_2: "This is a complementary pair not only in temperament but also in how they behave. Both find the other quite capable in ways that they aren’t themselves, and each respects their significant other as a result. So, this love affair will go smoothly from the start since they also have mutual understanding and great communication on their side, which are important ingredients for a relationship that will weather life’s inevitable storms.",
        gender_reverse_2: "Female Monkey and Male Rat",
        gender_reverse_more_2: "Monkey and Rat together will release both partners’ full potential for the greater good of their family. Monkey is an excellent long-term strategist, while Rat will take the reins of day-to-day living, which is also important. Both will strive to improve themselves constantly in their journey together, although neither will require the same from their partner, making this a loving and friendly marriage from the start that will prosper without fail.",
        best_3: "Rat and Ox",
        best_more_3: "The Rat and the Ox are neighbors on the list of zodiacs, and they are more similar than different. Both are risk-averse and don’t mind toiling away for years to build the life they want. Now that tenacity will be more than doubled. As neither will say, “I did the dishes last night; it’s your turn,” this giving quality will only encourage their partner to contribute even more love.",
        gender_3: "Female Rat and Male Ox",
        gender_more_3: "This pairing has a fated quality to it. Once they meet, Ox and Rat will likely end up together without needing to explore the dating scene any further, and they’ll decide to marry before too long. Rat is sensitive, while Ox is hardworking and dedicated to their partner, so their personalities complement each other in the best of ways and will provide the love that both crave in a romantic relationship.",
        gender_reverse_3: "Female Ox and Male Rat",
        gender_reverse_more_3: "You’re a naturally complementary pair. Rat is sensitive, with a vision for the sort of love life he wants, while Ox is hardworking, capable of giving without reserve once she’s in love, giving her all. Together, you’ll feel warmed to the core by your partner’s loving caress and attention. For a more satisfying partnership, however, Rat will need to take the initiative in creating passion for their more bashful partner.",
        worst: "Rat and Horse",
        worst_more: "These two Chinese zodiac signs clash naturally because Rats absolutely need to plan for the future, while Horses are passionate and impulsive. The way each thinks and behaves is very different. When two people with such divergent personalities come together in a relationship, the result can be disastrous since they’ll rarely see eye to eye, making each other’s life rather difficult until they split.",
        worst_2: "Rat and Goat",
        worst_more_2: "The Rat is suspicious, while the Goat can be jealous. Rather than making each partner want to give the other more reassurance, these traits seem to only lead to clashes. When together, this partnership is characterized by complaints from the Goat and a list of resentments from the Rat, neither of which spell marital bliss for the couple!",
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
        summary: "In Chinese astrology, the Ox is the second animal in the Chinese zodiac cycle. People born in the Year of the Ox are believed to possess certain personality traits and characteristics associated with this animal.",
        personality_1: "Ox are diligent with a strong sense of responsibility. Although not usually charismatic, they’re nonetheless loved for their ability to “anchor,” whether at work or in their love life. This is because although the Ox personality is gentle in nature, Oxen are capable of great courage when it’s time to step up—especially when no one else will, and overcome any difficulty, which many find rather reassuring.",
        strengths: "dependability",
        strengths_2: "hardworking",
        strengths_3: "stability",
        strengths_4: "patience",
        strengths_5: "family orientation",
        weaknesses: "stubbornness",
        weaknesses_2: "rigidity",
        weaknesses_3: "pessimism",
        weaknesses_4: "overcautiousness",
        weaknesses_5: "inflexibility",
        personality_2: "Oxen can also be stubborn to the point of insisting on their way or the highway, which can make these mild personalities appear arrogant or temperamental despite the best of intentions. In romance, their affection—although slow to ignite—will burn deep and remain bright for years to come, just like their ability to put their head down and work without complaint towards a career goal.",
        years: "Years of the Ox",
        years_1: "1925",
        years_2: "January 24, 1925",
        years_3:"February 12, 1926",
        years_4:"1937",
        years_5:"February 11, 1937",
        years_6:"January 30, 1938",
        years_7:"1949",
        years_8:"January 29, 1949",
        years_9:"February 16, 1950",
        years_10:"1961",
        years_11:"February 15, 1961",
        years_12:"February 4, 1962",
        years_13:"1973",
        years_14:"February 3, 1973",
        years_15:"January 22, 1974",
        years_16:"1985",
        years_17:"February 20, 1985",
        years_18:"February 8, 1986",
        years_19:"1997",
        years_20:"February 7, 1997",
        years_21: "January 27, 1998",
        years_22: "2009 ",
        years_23: "January 26, 2009",
        years_24: "February 13, 2010",
        years_25: "2021",
        years_26: "February 11, 2021",
        years_27: "January 31, 2022",
        years_28: "2033",
        years_29: "January 31, 2033",
        years_30: "January 18, 2034",
        overall: "Oxen are the hard workers in the background, intelligent and reliable, but never demanding praise.",
        metal: "Those born in the Year of the Metal Ox are more active than others, always keeping up a full plate in life. They’re capable of working all day, even forgetting to sleep or eat in their drive toward their ultimate goals. On the other hand, Metal Oxen aren’t blessed with great luck in love. If you’re lucky enough to find a partner, treat them and your relationship with care and dedication, and handle it with respect.",
        metal_years: "1961, 2021",
        water: "Water Oxen have a great sense of justice and make dependable leaders. They can also look at things from a subjective viewpoint, which gives them a flexibility that other Oxen natives do not possess. In matters of love, Water Oxen will be blessed to meet someone who checks all the boxes of their romantic ideal. They’ll have luck in business, where their friends are destined to bring them financial fortune.",
        water_years: "1973, 2033",
        wood: "Wood Oxen are straightforward with iron-clad values and standards that can prove offensive to some. In love, Wood Oxen should avoid petty quarrels with their partners since those hardly matter in the grand scheme. Despite their careful nature, Wood Oxen may fall prey to money problems and must stay away from risky ventures and gambling. Thankfully, they’re also likely to find help readily at hand in times like these.",
        wood_years: "1925, 2085",
        fire: "Fire Oxen can be self-centered and short-sighted and may find it difficult to build emotional intimacy with others. Therefore early on in life, their time would be best used by honing a skill to perfection. Later on, life will grow steadily easier for Fire Oxen as they mature emotionally. In particular, because their material wealth is all but guaranteed with a stable income and even frequent bonuses from unexpected quarters.",
        fire_years: "1937, 1997",
        earth: "Earth Oxen are even more diligent and thrifty than the rest, planning their every step with care. They’ll never extend themselves beyond their comfort zone, preferring to slowly gain confidence in life as they mature. While not particularly fortunate early on, once they reach middle age and beyond, Earth Oxen will begin to understand their blessings with the opposite sex, who’ll be attracted to their gentle nature throughout the years.",
        earth_years: "1949, 2009",
        compatibility: "Male or female, Oxen have a passionate heart with a romantic and rich inner world to match. They’re nurturing and steadfast, although it may take time before they feel ready to show their affectionate side. Even when they finally meet someone they like, Oxen may seem indifferent on the surface while they’re burning with passion underneath. Take proactive action and speak your feelings, Ox, so that love can be yours!",
        best: "Ox and Snake",
        best_more: "Ox and Snake are understated individuals who will never wear their hearts on their sleeves. Their love compatibility and courtship will surely be a slow one that takes time to reach its culmination—too slow to outside observers. These animal signs know their own and their partner’s worth and aren’t afraid to invest time in unraveling their partner’s mystery. Once committed, they’ll likely stand firmly by each other’s side until death do them part.",
        gender: "Female Ox and Male Snake",
        gender_more: "As a couple, you won’t hesitate to work together and support each other through thick and thin. Together, you’ll be capable of building a more comfortable life in no time, with equal contribution from both. You share the same values and beliefs with the same desire for stability, so you’ll be united in your striving. Before long, you’ll consider the other both a partner and the love of your life.",
        gender_reverse: "Female Snake and Male Ox",
        gender_reverse_more: "This is a harmonious union from the start. As they get to know each other, they’ll each feel as if they’ve found their other half. Once married, both partners will feel nourished by their family life. Ox will treat his partner with truthfulness and kindness, while Snake is gentle and dedicated to her loved ones—fitting Ox’s preference for traditional family life. In return, he’ll act the breadwinner role with pride.",
        best_2: "Ox and Rooster",
        best_more_2: "Rooster is one of the more brash signs, but they seem to appreciate the silent and tenacious ways of the Ox. And for once, the Ox doesn’t mind the attention of a more outgoing counterpart. Whether male or female, the Ox will let their Rooster half pursue, but their interest won’t be hard to interpret, either. With this encouragement, the Rooster will likely make the Ox theirs before too long.",
        gender_2: "Female Ox and Male Rooster",
        gender_more_2: "Ox and Rooster will happily grow old together and be everyone’s “relationship goals,” as you’re both willing to nurture your partner and, later, your family together. You may feel the desire to marry rather quickly. Rooster is honest and brave, their energy and optimism infectious for Ox. Even when facing difficulties in life, this team works well together, with Rooster leading the charge and Ox providing solid and loyal support.",
        gender_reverse_2: "Female Rooster and Male Ox",
        gender_reverse_more_2: "This will be a very happy pairing both partners working work hard in the professional sphere in their own way. THe Rooster will shine with natural charisma, dazzling their quiet Ox long before they notice. Once together, you’ll pool your resources and enable each other to thrive in new ways. You’ll appreciate each other’s best qualities and the way each is able to contribute to the longevity of your marriage.",
        best_3: "Ox and Rat",
        best_more_3: "The Rat and the Ox are neighbors on the list of zodiacs, and they are more similar than different. Both are risk-averse and don’t mind toiling away for years to build the life they want. Now that tenacity will be more than doubled. As neither will say, “I did the dishes last night; it’s your turn,” this giving quality will only encourage their partner to contribute even more love.",
        gender_3: "Female Rat and Male Ox",
        gender_more_3: "This pairing has a fated quality to it. Once they meet, Ox and Rat will likely end up together without needing to explore the dating scene any further, and they’ll decide to marry before too long. Rat is sensitive, while Ox is hardworking and dedicated to their partner, so their personalities complement each other in the best of ways and will provide the love that both crave in a romantic relationship.",
        gender_reverse_3: "Female Ox and Male Rat",
        gender_reverse_more_3: "You’re a naturally complementary pair. Rat is sensitive, with a vision for the sort of love life he wants, while Ox is hardworking, capable of giving without reserve once she’s in love, giving her all. Together, you’ll feel warmed to the core by your partner’s loving caress and attention. For a more satisfying partnership, however, Rat will need to take the initiative in creating passion for their more bashful partner.",
        worst: "Ox and Horse",
        worst_more: "These two may come together easily, but their pairing is not meant for the long term and will be characterized by frequent fights and disagreements enough to wear away any initial affection. Ox prefers a quiet and stable lifestyle, while Horse yearns for freedom, leading both to consider parting ways once the initial passion dies away. Unfortunately, fit is more important than attraction in a long-term relationship.",
        worst_2: "Ox and Goat",
        worst_more_2: "Both of these signs are characterized by the Earth element, although strangely, this leads to a “muddying” of boundaries instead of understanding. Even if the relationship lasts, it’ll likely turn codependent, to both parties’ detriment. These mild personalities are both stubborn, and neither will be likely to give way when they quarrel. The Ox may try to show that they care, but the Goat will find this suffocating and annoying.",
        lucky_1: "1, 4",
        lucky_2: "Blue, Yellow, Green",
        lucky_3: "North, South",
        lucky_4: "Tulip, Evergreen, Peach Blossom",
        lucky_5: "January, April, September, December",
        lucky_6: "Aquamarine, Jade",
        lucky_7: "Ox figurines or ornaments",
        unlucky_1: "3, 6",
        unlucky_2: "Red, White",
        unlucky_3: "East, Southeast",
        unlucky_4: "March, June, July, August",
        unlucky_5: "Ruby, Garnet",
    },
    tiger: {
        summary: "In Chinese astrology, the Tiger is the third animal sign in the twelve-year cycle and is associated with specific personality traits, characteristics, and symbolism. People born in the Year of the Tiger (which occurs every 12 years) are believed to inherit the traits associated with this animal. ",
        personality_1: "Tigers personality is fiercely independent, confident, and bold. Tigers are charismatic and enthusiastic by nature, although these big cats are usually not gregarious, and always seem to possess an endlessly infectious energy that keeps others engaged, especially as leaders at work. Anyone who’s crossed paths with Tigers would be struck by their natural presence. Their vitality is apparent at a glance, and people are instinctively drawn to this larger-than-life quality in these swashbuckling characters.",
        strengths: "dependability",
        strengths_2: "hardworking",
        strengths_3: "stability",
        strengths_4: "patience",
        strengths_5: "family orientation",
        weaknesses: "stubbornness",
        weaknesses_2: "rigidity",
        weaknesses_3: "pessimism",
        weaknesses_4: "overcautiousness",
        weaknesses_5: "inflexibility",
        personality_2: "Tigers usually possess a keen sense of justice from a young age and will take a stand for what’s right. However, they’re not exactly tactical with such confrontations, which may rub some the wrong way. Tigers are a loyal and honorable bunch who will, however, choose to service their ambition before attending to other aspects of life. Even a king requires a kingdom to truly inhabit their power, after all!",
        years: "Years of the Ox",
        years_1: "1925",
        years_2: "January 24, 1925",
        years_3:"February 12, 1926",
        years_4:"1937",
        years_5:"February 11, 1937",
        years_6:"January 30, 1938",
        years_7:"1949",
        years_8:"January 29, 1949",
        years_9:"February 16, 1950",
        years_10:"1961",
        years_11:"February 15, 1961",
        years_12:"February 4, 1962",
        years_13:"1973",
        years_14:"February 3, 1973",
        years_15:"January 22, 1974",
        years_16:"1985",
        years_17:"February 20, 1985",
        years_18:"February 8, 1986",
        years_19:"1997",
        years_20:"February 7, 1997",
        years_21: "January 27, 1998",
        years_22: "2009 ",
        years_23: "January 26, 2009",
        years_24: "February 13, 2010",
        years_25: "2021",
        years_26: "February 11, 2021",
        years_27: "January 31, 2022",
        years_28: "2033",
        years_29: "January 31, 2033",
        years_30: "January 18, 2034",
        overall: "Oxen are the hard workers in the background, intelligent and reliable, but never demanding praise.",
        metal: "Those born in the Year of the Metal Ox are more active than others, always keeping up a full plate in life. They’re capable of working all day, even forgetting to sleep or eat in their drive toward their ultimate goals. On the other hand, Metal Oxen aren’t blessed with great luck in love. If you’re lucky enough to find a partner, treat them and your relationship with care and dedication, and handle it with respect.",
        metal_years: "1961, 2021",
        water: "Water Oxen have a great sense of justice and make dependable leaders. They can also look at things from a subjective viewpoint, which gives them a flexibility that other Oxen natives do not possess. In matters of love, Water Oxen will be blessed to meet someone who checks all the boxes of their romantic ideal. They’ll have luck in business, where their friends are destined to bring them financial fortune.",
        water_years: "1973, 2033",
        wood: "Wood Oxen are straightforward with iron-clad values and standards that can prove offensive to some. In love, Wood Oxen should avoid petty quarrels with their partners since those hardly matter in the grand scheme. Despite their careful nature, Wood Oxen may fall prey to money problems and must stay away from risky ventures and gambling. Thankfully, they’re also likely to find help readily at hand in times like these.",
        wood_years: "1925, 2085",
        fire: "Fire Oxen can be self-centered and short-sighted and may find it difficult to build emotional intimacy with others. Therefore early on in life, their time would be best used by honing a skill to perfection. Later on, life will grow steadily easier for Fire Oxen as they mature emotionally. In particular, because their material wealth is all but guaranteed with a stable income and even frequent bonuses from unexpected quarters.",
        fire_years: "1937, 1997",
        earth: "Earth Oxen are even more diligent and thrifty than the rest, planning their every step with care. They’ll never extend themselves beyond their comfort zone, preferring to slowly gain confidence in life as they mature. While not particularly fortunate early on, once they reach middle age and beyond, Earth Oxen will begin to understand their blessings with the opposite sex, who’ll be attracted to their gentle nature throughout the years.",
        earth_years: "1949, 2009",
        compatibility: "Male or female, Oxen have a passionate heart with a romantic and rich inner world to match. They’re nurturing and steadfast, although it may take time before they feel ready to show their affectionate side. Even when they finally meet someone they like, Oxen may seem indifferent on the surface while they’re burning with passion underneath. Take proactive action and speak your feelings, Ox, so that love can be yours!",
        best: "Ox and Snake",
        best_more: "Ox and Snake are understated individuals who will never wear their hearts on their sleeves. Their love compatibility and courtship will surely be a slow one that takes time to reach its culmination—too slow to outside observers. These animal signs know their own and their partner’s worth and aren’t afraid to invest time in unraveling their partner’s mystery. Once committed, they’ll likely stand firmly by each other’s side until death do them part.",
        gender: "Female Ox and Male Snake",
        gender_more: "As a couple, you won’t hesitate to work together and support each other through thick and thin. Together, you’ll be capable of building a more comfortable life in no time, with equal contribution from both. You share the same values and beliefs with the same desire for stability, so you’ll be united in your striving. Before long, you’ll consider the other both a partner and the love of your life.",
        gender_reverse: "Female Snake and Male Ox",
        gender_reverse_more: "This is a harmonious union from the start. As they get to know each other, they’ll each feel as if they’ve found their other half. Once married, both partners will feel nourished by their family life. Ox will treat his partner with truthfulness and kindness, while Snake is gentle and dedicated to her loved ones—fitting Ox’s preference for traditional family life. In return, he’ll act the breadwinner role with pride.",
        best_2: "Ox and Rooster",
        best_more_2: "Rooster is one of the more brash signs, but they seem to appreciate the silent and tenacious ways of the Ox. And for once, the Ox doesn’t mind the attention of a more outgoing counterpart. Whether male or female, the Ox will let their Rooster half pursue, but their interest won’t be hard to interpret, either. With this encouragement, the Rooster will likely make the Ox theirs before too long.",
        gender_2: "Female Ox and Male Rooster",
        gender_more_2: "Ox and Rooster will happily grow old together and be everyone’s “relationship goals,” as you’re both willing to nurture your partner and, later, your family together. You may feel the desire to marry rather quickly. Rooster is honest and brave, their energy and optimism infectious for Ox. Even when facing difficulties in life, this team works well together, with Rooster leading the charge and Ox providing solid and loyal support.",
        gender_reverse_2: "Female Rooster and Male Ox",
        gender_reverse_more_2: "This will be a very happy pairing both partners working work hard in the professional sphere in their own way. THe Rooster will shine with natural charisma, dazzling their quiet Ox long before they notice. Once together, you’ll pool your resources and enable each other to thrive in new ways. You’ll appreciate each other’s best qualities and the way each is able to contribute to the longevity of your marriage.",
        best_3: "Ox and Rat",
        best_more_3: "The Rat and the Ox are neighbors on the list of zodiacs, and they are more similar than different. Both are risk-averse and don’t mind toiling away for years to build the life they want. Now that tenacity will be more than doubled. As neither will say, “I did the dishes last night; it’s your turn,” this giving quality will only encourage their partner to contribute even more love.",
        gender_3: "Female Rat and Male Ox",
        gender_more_3: "This pairing has a fated quality to it. Once they meet, Ox and Rat will likely end up together without needing to explore the dating scene any further, and they’ll decide to marry before too long. Rat is sensitive, while Ox is hardworking and dedicated to their partner, so their personalities complement each other in the best of ways and will provide the love that both crave in a romantic relationship.",
        gender_reverse_3: "Female Ox and Male Rat",
        gender_reverse_more_3: "You’re a naturally complementary pair. Rat is sensitive, with a vision for the sort of love life he wants, while Ox is hardworking, capable of giving without reserve once she’s in love, giving her all. Together, you’ll feel warmed to the core by your partner’s loving caress and attention. For a more satisfying partnership, however, Rat will need to take the initiative in creating passion for their more bashful partner.",
        worst: "Ox and Horse",
        worst_more: "These two may come together easily, but their pairing is not meant for the long term and will be characterized by frequent fights and disagreements enough to wear away any initial affection. Ox prefers a quiet and stable lifestyle, while Horse yearns for freedom, leading both to consider parting ways once the initial passion dies away. Unfortunately, fit is more important than attraction in a long-term relationship.",
        worst_2: "Ox and Goat",
        worst_more_2: "Both of these signs are characterized by the Earth element, although strangely, this leads to a “muddying” of boundaries instead of understanding. Even if the relationship lasts, it’ll likely turn codependent, to both parties’ detriment. These mild personalities are both stubborn, and neither will be likely to give way when they quarrel. The Ox may try to show that they care, but the Goat will find this suffocating and annoying.",
        lucky_1: "1, 3, 4",
        lucky_2: "Blue, Gray, White, Orange",
        lucky_3: "East, South, Southeast",
        lucky_4: "Yellow Lily, Cinquefoil",
        lucky_5: "February, May, June, Decemberv",
        lucky_6: "Sapphire, Aquamarine",
        lucky_7: "Tiger figurines or ornaments",
        unlucky_1: "6, 7, 8",
        unlucky_2: "Brown, Gold, Silver",
        unlucky_3: "North, West",
        unlucky_4: "March, April, October, November",
        unlucky_5: "Ruby, Garnet",
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
.perr th {
    border: 1px solid rgb(238, 228, 169);
    text-align: left;
    padding: 8px;    
    color: rgb(238, 228, 169);
    }
.perr td {
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
    text-align: justify;
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
text-align: center;
}
.earth h4{
    color: rgb(161, 41, 41);
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    text-align: center;   
}
.earth h2{
letter-spacing: 1px;
color: rgb(238, 228, 169);
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
text-align: center;
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
    border-radius: 10px;
    border: 3px solid rgb(238, 228, 169); 
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
