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


            <div class="famous">
                <h2>Famous Births</h2>
                <div class="fam">
                <div class="fa">
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_2 }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more_2 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_3 }}</h3>
                     <p> {{ data[zodiacSign]?.birth_more_3 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_4 }}</h3>
                     <p>{{ data[zodiacSign]?.birth_more_4 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_5 }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more_5 }}
                    </p>
                </div>
            </div>
            <div class="fa">
            <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_6 }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more_6 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_7 }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more_7 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_8 }}</h3>
                     <p> {{ data[zodiacSign]?.birth_more_8 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_9 }}</h3>
                     <p>{{ data[zodiacSign]?.birth_more_9 }}
                    </p>
                </div>
                <div class="f">
                    <h3>{{ data[zodiacSign]?.birth_10 }}</h3> 
                    <p>{{ data[zodiacSign]?.birth_more_10 }}
                    </p>
                </div>
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
        summary: "Rats are well-behaved by nature and have fun and quirky personalities. They exude superb energy in life and do what they can to garner approval from others—even if misplaced. Rat personalities also tend to exude a sense of mystery, hoarding their own secrets while observing others and adjusting how they behave. Their mystery is strategic, not selfish, so they would make great team players.",
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
        personality_2: "Rats love being in a group and may feel lonely when they’re on their own. They are friendly and easy-going, finding it easy to make friends despite a slight inclination to secrecy and introversion. In terms of lifestyle, Rats are frugal with a tendency to save—even to hoard. As long as they learn to withstand temptations in this area, their life will turn out quite steady and prosperous.",
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
        birth: "William Shakespeare:",
        birth_more: "English playwright, poet, and actor.",
        birth_2: "Eminem:",
        birth_more_2: "American rapper, songwriter, and record producer.",
        birth_3: "Agatha Christie:",
        birth_more_3: "English writer known for her detective novels.",
        birth_4: "Queen Victoria:",
        birth_more_4: "Former Queen of the United Kingdom.",
        birth_5: "Charles Darwin:",
        birth_more_5: "English naturalist, geologist, and biologist.",
        birth_6: "Scarlett Johansson:",
        birth_more_6: "American actress and singer.",
        birth_7: "Queen Elizabeth I:",
        birth_more_7: "Former Queen of England and Ireland.",
        birth_8: "Mother Teresa:",
        birth_more_8: "Albanian-Indian Roman Catholic nun and missionary.",
        birth_9: "Marie Skłodowska-Curie:",
        birth_more_9: "Polish physicist and chemist",
        birth_10: "Coco Chanel:",
        birth_more_10: "French fashion designer and businesswoman, founder of the Chanel brand.",
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
        birth: "Vincent van Gogh:",
        birth_more: "Dutch post-impressionist painter.",
        birth_2: "Barack Obama:",
        birth_more_2: "44th President of the United States.",
        birth_3: "Adolf Hitler:",
        birth_more_3: "German dictator and leader of the Nazi Party during World War II.",
        birth_4: "Napoleon Bonaparte:",
        birth_more_4: "French military leader and Emperor of the French.",
        birth_5: "Michelle Obama:",
        birth_more_5: "Former First Lady of the United States, lawyer, and author.",
        birth_6: "Walt Disney:",
        birth_more_6: "Founder of The Walt Disney Company.",
        birth_7: "Rosa Parks:",
        birth_more_7: "American civil rights activist.",
        birth_8: "Jane Austen:",
        birth_more_8: "English novelist known for her classic works.",
        birth_9: "Princess Diana:",
        birth_more_9: "Former Princess of Wales and renowned humanitarian.",
        birth_10: "Malala Yousafzai:",
        birth_more_10: "Pakistani activist for female education.",
    },
    tiger: {
        summary: "In Chinese astrology, the Tiger is one of the twelve zodiac signs. Each year is associated with one of these signs in a twelve-year cycle, and the Tiger is the third sign in the cycle. People born in the year of the Tiger are believed to possess certain characteristics and traits associated with that animal. ",
        personality_1: "Tigers personality is fiercely independent, confident, and bold. Tigers are charismatic and enthusiastic by nature, although these big cats are usually not gregarious, and always seem to possess an endlessly infectious energy that keeps others engaged, especially as leaders at work. Anyone who’s crossed paths with Tigers would be struck by their natural presence. Their vitality is apparent at a glance, and people are instinctively drawn to this larger-than-life quality in these swashbuckling characters.",
        strengths: "courageous",
        strengths_2: "confident",
        strengths_3: "strong leadership qualities",
        strengths_4: "passionate",
        strengths_5: "adventurous",
        weaknesses: "impulsiveness",
        weaknesses_2: "hot-tempered",
        weaknesses_3: "risk-taking",
        weaknesses_4: "overconfidence",
        weaknesses_5: "stubbornness",
        personality_2: "Tigers usually possess a keen sense of justice from a young age and will take a stand for what’s right. However, they’re not exactly tactical with such confrontations, which may rub some the wrong way. Tigers are a loyal and honorable bunch who will, however, choose to service their ambition before attending to other aspects of life. Even a king requires a kingdom to truly inhabit their power, after all!",
        years: "Years of the Tiger",
        years_1: "1927",
        years_2: "February 2, 1927",
        years_3:"January 22, 1928",
        years_4:"1939",
        years_5:"February 19, 1939",
        years_6:"February 8, 1940",
        years_7:"1951",
        years_8:"February 6, 1951",
        years_9:"January 26, 1952",
        years_10:"1963",
        years_11:"January 25, 1963",
        years_12:"February 12, 1964",
        years_13:"1975",
        years_14:"February 11, 1975",
        years_15:"January 30, 1976",
        years_16:"1987",
        years_17:"January 29, 1987",
        years_18:"February 16, 1988",
        years_19:"1999",
        years_20:"February 16, 1999",
        years_21: "February 4, 2000",
        years_22: "2011 ",
        years_23: "February 3, 2011",
        years_24: "January 22, 2012",
        years_25: "2023",
        years_26: "January 22, 2023",
        years_27: "February 9, 2024",
        years_28: "2035",
        years_29: "February 8, 2035",
        years_30: "January 27, 2036",
        overall: "Rabbits are earnest with everything they do; they just ask that others treat them the same way.",
        metal: "Metal Rabbits are smart and creative, often struck with unexpected inspiration. They have a hidden depth most aren’t privy to. Relationships are key to their success, so it’s best to maintain a courteous but removed circle. Metal Rabbits will have opportunities to make small incomes throughout their life, but they must not make large gambles, which they’ll certainly lose. They spend freely, so budgeting is something they must learn as they mature.",
        metal_years: "1951, 2011",
        water: "Those born in the Year of the Water Rabbits are usually blessed with a comfortable life from the start. As such, they’ll likely be passive and rather mild compared to others, pursuing pleasure and comfort in life without any sense of urgency. Water Rabbits aren’t blessed with good luck and will go through many short-lived romances until they learn to change their lackluster approach to romance. In addition, they must keep a close eye on health throughout life.",
        water_years: "1963, 2023",
        wood: "Wood Rabbits are kind and conservative, disliking competition and indifferent towards success, although they seem to gravitate toward people who are competitive—perhaps as an inspiration or at least a complement to their own character. In life and in love, Wood Rabbits are richly imaginative and hate the mundane. They’re talented in money management, although things tend to break down around them, which will eat away from their budget unexpectedly.",
        wood_years: "1975, 2035",
        fire: "Fire Rabbits are clever and singularly marked for leadership among all Rabbit natives. They hold lofty ideals, are good with decision making, and aspire to power, and they will often leverage influence and support from the masses to achieve their goals. Fire Rabbits should heed others’ advice more, as their fiery temper can make them hot-headed in certain situations. They also have the tendency to provoke others when they are anxious, which may disrupt their relationships.",
        fire_years: "1927, 1987",
        earth: "Earth Rabbits are frank and straightforward. They are ambitious and more entrepreneurial than other Rabbit natives. Their ambition runs high, making them demanding at work, but once home, they’ll be more relaxed and like themselves. Earth Rabbits lack money management skills, so imposing a budget on themselves early in life is very important, although almost impossible to actually implement. Gentle, generous, and kind, they’ll be loved by their family unconditionally.",
        earth_years: "1939, 1999",
        compatibility: "In matters of the heart, Rabbits start out suspicious of others’ motives, since their cautious nature means that many of their ideas and understanding of the world—whether real or imaginary—tend toward the negative. Once they truly fall in love for the first time, they’ll learn to be honest with their feelings without being defensive. In many ways, true love will be the beginning of Rabbits’ farewell to loneliness.",
        best: "Rabbit and Dog",
        best_more: "Neither Rabbit or Dog is flashy or self-important. Where some relationships have one diva and one humble servant; in this one, both partners are equal in how humble and how loving they are to each other. It’s worth noting that this pairing may make both complacent, which is fine if neither aspires to more—but if you do, it would be a bad idea to give up your dreams for love.",
        gender: "Female Rabbit and Male Dog",
        gender_more: "Rabbit is capable and clever, while Dog is loyal and steady. When Rabbit tires of her whimsical adventures in the world, Dog is always there to welcome her back to their safe and comfortable nest. Even though they’re both gentle creatures, Dog and Rabbit should also nurture their life goals separately, which will serve as cornerstones to their romantic relationship. Being excellent communicators, they find it easy to talk together.",
        gender_reverse: "Female Dog and Male Rabbit",
        gender_reverse_more: "Both will put the other first and consider the other’s feelings more important than their own. This is because both are accustomed to giving too much, which won’t be taken for granted in this relationship. Rabbit excels at creating a loving environment for their partner, which is intoxicating for Dog, while Dog is naturally loyal, which Rabbit appreciates and values above many other qualities. A stable partnership built to last.",
        best_2: "Rabbit and Goat",
        best_more_2: "Rabbit and Goat, the softies of the 12 zodiacs, delight in their partner’s good nature and gentle temperament, and then curiously, they find strength and courage in the power of love to take on the world. Isn’t the meaning of love to make both partners the most expansive versions of themselves? That’s why at home where they feel safe, these two will share a pure, restorative, and nearly innocent love.",
        gender_2: "Female Rabbit and Male Goat",
        gender_more_2: "Rabbit and Goat make each other shine brighter when they come together and share a partnership not of intense passion but mutual understanding and care, which is both rare and vital to a long-term relationship. Rabbit is quicker than Goat, which Goat admires and praises, filling Rabbit (who’s secretly vain) with pride. This, in turn, motivates the Rabbit to show up in the relationship in an even more loving manner.",
        gender_reverse_2: "Female Goat and Male Rabbit",
        gender_reverse_more_2: "Both Rabbit and Goat are romantic to the core and believe love to be a vital part of life. They will get along well, and their partner will have a special place in their heart. They’re mild and gentle, so even when they quarrel—a rare occurrence—they’ll quickly apologize and make up. They prize communication, making this a solid connection that can weather any storm life throws at them.",
        best_3: "Rabbit and Pig",
        best_more_3: "This will likely be the most supportive and warm relationship Rabbit and Pig have ever experienced, and both partners will marvel at their luck in finding the perfect mate for many years to come. Rabbit has always been skittish because they feel uneasy in the world, which Pig’s laid back manner goes a long way to assuage. In return, Rabbit can add a certain charm and sparkle to Pig’s life.",
        gender_3: "Female Rabbit and Male Pig",
        gender_more_3: "Rabbit and Pig are both givers, which others take advantage of, so when they come together in this relationship and discover the same in their partner, they may just fall in love all over again. They can both give without fear when that happens, and their romance will become solid almost overnight. Pig takes care of Rabbit, which is such an attractive trait to her, while Rabbit charms Pig constantly.",
        gender_reverse_3: "Female Pig and Male Rabbit",
        gender_reverse_more_3: "Both partners will benefit from this relationship, as both will notice the positive characteristics in their partner that they would like to have themselves early on. As such, it’s a bond built upon mutual admiration. Rabbit is clever and usually a star in their discipline, which Pig adores. In the meantime, Pig is loyal and honest, an endlessly giving partner who will become a pillar of spiritual support for Rabbit.",
        worst: "Rabbit and Rooster",
        worst_more: "This isn’t an ideal match for love or marriage because Rooster and Rabbit look at the world in such fundamentally different ways that even as colleagues, they are likely to clash, not to mention love. As romantic partners, they’re bound to fight over every detail of their shared life. Rooster finds Rabbit vain, while Rabbit finds Rooster selfish. Neither will notice the other’s better qualities, making this an exhausting pairing.",
        worst_2: "Rabbit and Dragon",
        worst_more_2: "Rabbit can’t be themselves with Dragon as their mate because Dragon picks on Rabbit for being careless and complacent, resigning Rabbit to loneliness within the relationship until it becomes too much for this gentle creature. Their personalities clash because Dragon is decisive and overwrought, always wanting to press things forward relentlessly, which tires Rabbit out, while Rabbit is quiet and sensitive with a rich emotional life that Dragon will ignore. ",
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
        birth: "Marilyn Monroe:",
        birth_more: "Iconic American actress, singer, and model.",
        birth_2: "Lady Gaga:",
        birth_more_2: "Award-winning American singer, songwriter, and actress.",
        birth_3: "Leonardo DiCaprio:",
        birth_more_3: "American actor and environmental activist.",
        birth_4: "Queen Elizabeth II:",
        birth_more_4: "Longest-reigning current monarch and former Queen of the United Kingdom.",
        birth_5: "Ludwig van Beethoven:",
        birth_more_5: "German composer and pianist.",
        birth_6: "Bill Murray:",
        birth_more_6: "American actor and comedian.",
        birth_7: "Tom Cruise:",
        birth_more_7: "American actor and producer.",
        birth_8: "Penélope Cruz:",
        birth_more_8: "Spanish actress and model.",
        birth_9: "Emily Dickinson:",
        birth_more_9: "American poet known for her unique style and themes of death.",
        birth_10: "Karl Marx:",
        birth_more_10: "German philosopher, economist, and political theorist.",
    },

    rabbit: {
        summary: "In Chinese astrology, the Rabbit is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Rabbit (also known as the Year of the Hare) are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "Rabbits are elegant, imaginative, and courteous to others—even their enemies—because they hate any kind of conflict. They possess a keen perception of reality, which makes Rabbits the ultimate adapters to the real world. Unexpectedly, Rabbits are savvy in business and financial transactions and are good at finding win-win solutions in complex situations. They adore an abundant lifestyle and prefer not to be stressed out most of the time.",
        strengths: "gentleness",
        strengths_2: "intuition",
        strengths_3: "creativity",
        strengths_4: "diplomacy",
        strengths_5: "charm",
        weaknesses: "indecisiveness",
        weaknesses_2: "overly sensitive",
        weaknesses_3: "avoidance of conflict",
        weaknesses_4: "overthinking",
        weaknesses_5: "procrastination",
        personality_2: "Rabbits won’t tolerate a boring life. They’ll continuously create interest in life, hopping from one excitement to the next, so they’re not the best at delving into any subject for an extended period of time. The Rabbit personality can be overly cautious and jumpy. When a Rabbit is feeling down, may have the tendency to escape from reality. A key lesson for Rabbits is how to manage their emotions so that they can thrive. ",
        years: "Years of the Rabbit",
        years_1: "1926",
        years_2: "February 13, 1926",
        years_3:"February 1, 1927",
        years_4:"1938",
        years_5:"January 31, 1938",
        years_6:"February 18, 1939",
        years_7:"1950",
        years_8:"February 17, 1950",
        years_9:"February 5, 1951",
        years_10:"1962",
        years_11:"February 5, 1962",
        years_12:"January 24, 1963",
        years_13:"1974",
        years_14:"January 23, 1974",
        years_15:"February 10, 1975",
        years_16:"1986",
        years_17:"February 9, 1986",
        years_18:"January 28, 1987",
        years_19:"1998",
        years_20:"January 28, 1998",
        years_21: "February 15, 1999",
        years_22: "2010 ",
        years_23: "February 14, 2010",
        years_24: "February 2, 2011",
        years_25: "2022",
        years_26: "February 1, 2022",
        years_27: "January 21, 2023",
        years_28: "2034",
        years_29: "January 19, 2034",
        years_30: "February 7, 2035",
        overall: "Tigers are courageous and active people who love a good challenge and adventure in life.",
        metal: "Metal Tigers are self-possessed, self-confident, and occasionally self-righteous. It’s virtually impossible for them to watch others suffer without trying to remedy the situation somehow, and they’ll give freely if anyone asks them for any assistance. What Metal Tigers promise to do for others and decide to pursue for themselves will not be easily shaken by external opinions. It’s best to buy gold and other value-preserving goods, as they’re easily deceived.",
        metal_years: "1950, 2010",
        water: "Brash on the outside while often indecisive on the inside, people born in the Year of the Water Tiger tend to have good interpersonal relationships. They’re family-oriented and like to lead a quiet and peaceful family life without interference from their profession. Water Tigers are ambitious. If they can work hard and keep making progress, they’ll surely realize their wishes. They can find others’ advice off-putting, a hang-up they’ll have to get over in order to succeed.",
        water_years: "1962, 2022",
        wood: "Wood Tigers have excellent memories. They’re quick learners, with particular talent in innovation. Their professional fortunes are mixed, but if they can keep a circle of advisors, they’ll be able to realize a bright future. As they strive, it’s important for Wood Tigers to value the love and friendships they have; otherwise, they’ll lose their closest confidants. Arrogance, whether in love, work, or investment, could prove Wood Tigers’ greatest downfall.",
        wood_years: "1974, 2034",
        fire: "Fire Tigers are earnest, passionate, and strong-willed. Since they don’t love discussions, Fire Tigers might loudly express their opinion without giving others a chance to speak, which may lead others to think Fire Tigers are condescending. In actuality, Fire Tigers are generous to a fault, which makes them great husband and father material. They enjoy family bliss, and with the wealth they’re destined for, they will never be short of money.",
        fire_years: "1926, 1986",
        earth: "Earth Tigers are natural entrepreneurs since they know how to command attention and trust. As they’re in the habit of helping others, they’ll find others eager to help if they’re in need—it’s their karmic due. As entrepreneurs, Earth Tigers love to innovate, often coming up with brand-new ideas that they’ll share with their friends and try to implement together. However, they should be more considerate of their romantic partner.",
        earth_years: "1938, 1998",
        compatibility: "Tigers make great romantic partners but may sometimes come off as pushy in their exuberant courtship, which might overwhelm more reserved signs, while Tigers are obliviously intoxicated by romance—all good once they calm down. Despite their dominant exterior, Tigers often look forward to a life filled with romance with a child-like wonder, expecting fairy tales. Because they’re naturally passionate, their partner may not know how to match their passion.",
        best: "Tiger and Horse",
        best_more: "Tiger and Horse are two larger-than-life zodiac signs who, instead of clashing, recognize the other’s energy and ambition as on par with their own. In terms of compatibility, sharing their dreams with each other will come naturally to them. For Tiger, it’s essential that they not only like their partner but respect them, too. Horse’s activity and confidence inspire precisely that. It’s a union in which both partners move forward in the world together.",
        gender: "Female Tiger and Male Horse",
        gender_more: "This pair will have a lot in common since both will have plenty of energy and will most likely enjoy moving toward a common goal together. Together, they can make continuous progress and create a better life. The Horse is a confident and action-driven man, while the Tiger is a cheerful and charming presence inside the home. Tiger will take charge of the family, so there’ll be a clear division of duties.",
        gender_reverse: "Female Horse and Male Tiger",
        gender_reverse_more: "This is an energetic, warm, and harmonious pairing. Both partners are enthusiastic about life and rather cheerful, but neither will overindulge in family life, as both are very career-oriented, rejoicing in each other’s professional growth. Horse is intelligent and gentle with her partner and able to tolerate a certain degree of fickleness from her Tiger mate, which is exactly what Tiger needs—someone who listens to his many ideas every day.",
        best_2: "Tiger and Dog",
        best_more_2: "Tiger will be the undeniable leader in this relationship, but that doesn’t mean they’ll disrespect Dog. Instead, this will be a harmonious and cohesive partnership from which both parties will stand to benefit greatly. “Too many cooks” won’t be a problem in this kitchen, as Dog will take a step back when Tiger gets in a quarrelsome mood, which Tiger will compensate with ample affection when they calm down.",
        gender_2: "Female Tiger and Male Dog",
        gender_more_2: "This is a naturally good match, as both are kind and charitable idealists. They’ll be able to give each other the understanding they need as a married couple: the temperamental Tiger and the diplomatic Dog. This pair will enjoy physical and mental peace—a feeling of being at ease in their partner’s presence. Both are likely to become even more generous and humble as their relationship matures. A perfect match.",
        gender_reverse_2: "Female Dog and Male Tiger",
        gender_reverse_more_2: "This will be a sweet and mutually affectionate couple who will both work hard and stay dedicated to their family for years to come. Everything will start with their instant and natural attraction to each other. Dog is gentle and affectionate, while Tiger has a can-do attitude with a compassionate heart, which makes Dog feel safe investing in the relationship. This pairing will spur each other on to reach their full potential.",
        best_3: "Tiger and Pig",
        best_more_3: "You’d think Tiger would find Pig sloppy, but then you’d be wrong. Perhaps Tiger’s tired of being so independent and high-strung, but in any case, when they meet Pig, they’re going to be charmed instantly. Pig’s laid back attitude conceals a calm and generous nature, which Tiger finds attractive in their partner, while Tiger’s fiery personality inspires Pig to pursue their goals and grow to be an equal to their partner.",
        gender_3: "Female Tiger and Male Pig",
        gender_more_3: "Tiger and Pig are a pair that can motivate each other since Tiger is cheerful and high-spirited, and Pig is kind-hearted and generous toward others, making the compassionate yet aloof Tiger quite fond of them. They’ll know how to attract and keep each other’s attention from the beginning, which is why any shortcomings will likely be ignored by their mate in favor of their strengths. A very forgiving couple indeed.",
        gender_reverse_3: "Female Pig and Male Tiger",
        gender_reverse_more_3: "This pair shares a mutual motivation for a better life and will be there for their partner when they need it most. Both will be vigorously alive and regard their partner as more important than life itself. They’ll feel most liberated when they’re together, with the joint ability to maintain passion and understanding in their intimate relationship, which keeps this partnership fresh until they’re ready to enjoy a sweet old age together.",
        worst: "Tiger and Monkey",
        worst_more: "These two zodiac signs clash terribly since Tiger is strong-willed and ambitious but often incapable of listening to others’ ideas, while Monkey can be temperamental and unwilling to back down even when Tiger’s temper flares. As a couple, they will quarrel over everything and end with both being selfish toward their partner. This pairing will most likely not last for very long, with a hasty marriage inevitably ending in divorce.",
        worst_2: "Tiger and Snake",
        worst_more_2: "It’ll be difficult for this pairing to come together since they are almost polar opposites in temperament and preference and won’t find it easy to understand the other person’s opinion, position, or motivation in life. Tiger is passionate and direct, while Snake is cautious and suspicious. Snake finds Tiger overpowering, while Tiger finds Snake difficult to get to know. Without the ability to communicate, this pairing is destined to fail.",
        lucky_1: "3, 4, 6",
        lucky_2: "Pink, Purple, Blue",
        lucky_3: "East, South, Southeast",
        lucky_4: "Jasmine, Plantain Lily",
        lucky_5: "March, April, September, December",
        lucky_6: "Pearl, Moonstone",
        lucky_7: "Rabbit figurines or ornaments",
        unlucky_1: "1, 7, 8",
        unlucky_2: "Red, Brown, Black",
        unlucky_3: "West, Northwest",
        unlucky_4: "May, June, July, August",
        unlucky_5: "Ruby, Garnet",
        birth: "Albert Einstein",
        birth_more: "German-born theoretical physicist.",
        birth_2: "Lionel Messi:",
        birth_more_2: "Argentine professional footballer.",
        birth_3: "Angelina Jolie:",
        birth_more_3: "American actress, filmmaker, and humanitarian.",
        birth_4: "Whitney Houston:",
        birth_more_4: "American singer and actress known for her powerful voice.",
        birth_5: "Johnny Depp:",
        birth_more_5: "American actor known for his eccentric roles.",
        birth_6: "Brad Pitt:",
        birth_more_6: "American actor and film producer.",
        birth_7: "Serena Williams:",
        birth_more_7: "American professional tennis player.",
        birth_8: "Rosalind Franklin:",
        birth_more_8: "English chemist and X-ray crystallographer.",
        birth_9: "Stephen Hawking:",
        birth_more_9: "British theoretical physicist, cosmologist, and author.",
        birth_10: "Michael Jordan:",
        birth_more_10: "American former professional basketball player.",
    },
    dragon: {
        birth: "Bruce Lee:",
        birth_more: "Iconic Hong Kong-American martial artist, actor, director, and philosopher.",
        birth_2: "Vladimir Putin:",
        birth_more_2: "President of Russia and former Prime Minister.",
        birth_3: "Martin Luther King Jr.:",
        birth_more_3: "American Baptist minister and civil rights leader.",
        birth_4: "Rihanna:",
        birth_more_4: "Barbadian singer, songwriter, actress, and businesswoman.",
        birth_5: "Adele:",
        birth_more_5: "British singer-songwriter known for her powerful vocals.",
        birth_6: "Shakira:",
        birth_more_6: "Colombian singer-songwriter known for her distinctive voice.",
        birth_7: "Yuri Gagarin:",
        birth_more_7: "Soviet cosmonaut and the first human to journey into outer space.",
        birth_8: "Cindy Crawford:",
        birth_more_8: "American model and actress known for her success in the fashion.",
        birth_9: "Mahatma Gandhi:",
        birth_more_9: "Indian lawyer, anti-colonial nationalist, and political ethicist.",
        birth_10: "Elizabeth I:",
        birth_more_10: "Queen of England and Ireland from 1558 until her death in 1603.",
    },
    snake: {
        birth: "Abraham Lincoln:",
        birth_more: "US president, known for his leadership during the American Civil War",
        birth_2: "Charlie Chaplin:",
        birth_more_2: "English comic actor, filmmaker and composer.",
        birth_3: "Martha Stewart:",
        birth_more_3: "Retail businesswoman, writer and former model.",
        birth_4: "Audrey Hepburn:",
        birth_more_4: "Belgian-born British actress and humanitarian.",
        birth_5: "Mao Zedong:",
        birth_more_5: "Chinese communist revolutionary.",
        birth_6: "George Orwell:",
        birth_more_6: "British writer and journalist known for his dystopian novels.",
        birth_7: "Pablo Picasso:",
        birth_more_7: "Spanish painter, sculptor, and co-founder of the Cubist movement.",
        birth_8: "Frida Kahlo:",
        birth_more_8: "Mexican painter known for her self-portraits.",
        birth_9: "Grace Kelly:",
        birth_more_9: "American actress who became Princess of Monaco.",
        birth_10: "Johann Sebastian Bach:",
        birth_more_10: "German composer and musician of the Baroque period.",
    },
    horse: {
        birth: "Nelson Mandela:",
        birth_more: "South African anti-apartheid revolutionary and political leader",
        birth_2: "Denzel Washington:",
        birth_more_2: "American actor, director, and producer.",
        birth_3: "Angela Merkel:",
        birth_more_3: "German politician who served as Chancellor of Germany.",
        birth_4: "Jackie Chan:",
        birth_more_4: "Hong Kong martial artist, actor, director, and stuntman.",
        birth_5: "Margaret Thatcher:",
        birth_more_5: "British stateswoman who served as Prime Minister of the UK.",
        birth_6: "Nikola Tesla:",
        birth_more_6: "Inventor, electrical engineer, mechanical engineer, and futurist",
        birth_7: "Charles Dickens:",
        birth_more_7: "English writer and social critic known for his novels.",
        birth_8: "Margaret Mead:",
        birth_more_8: "American cultural anthropologist.",
        birth_9: "Natalie Portman:",
        birth_more_9: " Israeli-American actress known for her role in 'Black Swan' ",
        birth_10: "Julia Roberts:",
        birth_more_10: "American actress known for her role in 'Pretty Woman'",
    },
    goat: {
        birth: "Courteney Cox:",
        birth_more: "American actress known for her role as Monica Geller.",
        birth_2: "Bill Gates:",
        birth_more_2: "American business magnate, software developer, and philanthropist.",
        birth_3: "Michelangelo:",
        birth_more_3: "Italian sculptor, painter, architect, and poet of the High Renaissance.",
        birth_4: "Robert De Niro:",
        birth_more_4: "American actor, producer, and director.",
        birth_5: "Bruce Willis:",
        birth_more_5: "American actor known for his role in 'Pulp Fiction'.",
        birth_6: "Sofia Vergara:",
        birth_more_6: "Colombian-American actress, television producer, and model.",
        birth_7: "Winona Ryder:",
        birth_more_7: "American actress known for her role in 'Edward Scissorhands'.",
        birth_8: "Thomas Jefferson:",
        birth_more_8: "US president and author of the Declaration of Independence.",
        birth_9: "Rembrandt van Rijn:",
        birth_more_9: "Dutch painter and printmaker.",
        birth_10: "George Harrison:",
        birth_more_10: " British musician, singer, and songwriter.",
    },
    monkey: {
        birth: "Leonardo da Vinci:",
        birth_more: "Italian polymath known for his expertise in painting.",
        birth_2: "Julius Caesar:",
        birth_more_2: "Roman general, statesman, and historian.",
        birth_3: "Tom Hanks:",
        birth_more_3: "American actor and filmmaker known for his role in 'Forrest Gump'.",
        birth_4: "Diana Ross:",
        birth_more_4: "American singer, actress, and record producer.",
        birth_5: "Will Smith:",
        birth_more_5: "American actor, producer, and rapper.",
        birth_6: "Kim Kardashian:",
        birth_more_6: "American media personality, socialite, model and businesswoman.",
        birth_7: "Julius Erving:",
        birth_more_7: "American former professional basketball player known as 'Dr. J,'.",
        birth_8: "Halle Berry:",
        birth_more_8: "American actress known for her role in 'X-Men'.",
        birth_9: "Christina Aguilera:",
        birth_more_9: "American singer, songwriter, and actress.",
        birth_10: "Usain Bolt:",
        birth_more_10: "Jamaican former sprinter.",
    },
    rooster: {
        birth: "Jennifer Aniston:",
        birth_more: "American actress, producer, and businesswoman.",
        birth_2: "Justin Timberlake:",
        birth_more_2: "American singer, songwriter, actor, and record producer.",
        birth_3: "Britney Spears:",
        birth_more_3: "American singer, songwriter, dancer, and actress.",
        birth_4: "Pharrell Williams:",
        birth_more_4: "American singer, songwriter, record producer, and fashion designer.",
        birth_5: "Benjamin Franklin:",
        birth_more_5: "American polymath, scientist and founding father of the US",
        birth_6: "Winston Churchill:",
        birth_more_6: "British army officer who served as Prime Minister of the UK",
        birth_7: "Gloria Steinem:",
        birth_more_7: "American feminist, journalist, and social-political activist.",
        birth_8: "Celine Dion:",
        birth_more_8: "Canadian singer known for her powerful voice.",
        birth_9: "Jay-Z:",
        birth_more_9: "American rapper, songwriter, record executive, and entrepreneur.",
        birth_10: "Bruce Lee:",
        birth_more_10: "Chinese-American martial artist, actor, and filmmaker.",
    },
    dog: {
        birth: "Madonna:",
        birth_more: "American singer, songwriter, actress, and businesswoman.",
        birth_2: "Justin Bieber:",
        birth_more_2: "Canadian singer, songwriter, and pop sensation.",
        birth_3: "Michael Jackson:",
        birth_more_3: "American singer, songwriter, and dancer known as the 'King of Pop'.",
        birth_4: "Donald Trump:",
        birth_more_4: "45th President of the United States and businessman.",
        birth_5: "Jane Goodall:",
        birth_more_5: "British primatologist, ethologist, and anthropologist.",
        birth_6: "Anna Pavlova:",
        birth_more_6: "Russian prima ballerina known for her exceptional grace.",
        birth_7: "Alexander the Great:",
        birth_more_7: "King of Macedon who created one of the largest empires.",
        birth_8: "Wolfgang Amadeus Mozart:",
        birth_more_8: "Austrian composer and prodigy.",
        birth_9: "Amelia Earhart:",
        birth_more_9: "American aviation pioneer and author.",
        birth_10: "Isaac Newton:",
        birth_more_10: "English mathematician, physicist, and astronomer.",
    },
    pig: {
        birth: "Hillary Clinton:",
        birth_more: "American First Lady, Senator and Secretary of State.",
        birth_2: "Arnold Schwarzenegger:",
        birth_more_2: "Actor, filmmaker, author and professional bodybuilder",
        birth_3: "Stephen King:",
        birth_more_3: "American author known for his horror and fantasy novels",
        birth_4: "Tim Burton:",
        birth_more_4: "American filmmaker and animator known for his gothic style",
        birth_5: "Pamela Anderson:",
        birth_more_5: "Canadian-American actress, model, and activist.",
        birth_6: "Mike Tyson:",
        birth_more_6: "American former professional boxer.",
        birth_7: "Jamie Foxx:",
        birth_more_7: "American actor, singer, comedian, and producer.",
        birth_8: "P!nk:",
        birth_more_8: "American singer, songwriter, dancer, and actress.",
        birth_9: "Renée Zellweger:",
        birth_more_9: "American actress known for her role in 'Bridget Jones's Diary'.",
        birth_10: "Matthew McConaughey:",
        birth_more_10: "American actor and producer.",
    },
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
width: 80%;
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
font-size: x-large;   
color: rgb(161, 41, 41); 
font-family: fantasy;
border: 1px solid rgb(143, 143, 143);
padding: 3px;
padding-left: 10px;
padding-right: 10px;
border-radius: 10px;
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
color: rgb(26, 15, 32);
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
.five::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.elements{
display: flex;    
flex-direction: row;
justify-content: space-around;
}
.earth h2::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.earth h4::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.dropdown-content p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.dropdown:hover .dropdown-content {
    display: block;
    justify-content: baseline;
  }
.dropdown span {
    border-radius: 25px;
    background: rgb(161, 41, 41);
}
.dropdown span::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.comp h1{
    display: flex;
    justify-content: center;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(161, 41, 41); 
    letter-spacing: 1px;
    justify-content: center;
}
.comp h1::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.comp h2::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.comp p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.co h3::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.compa p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.com h3::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.kw h2::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.kw h2 {
    padding: 30px;
    padding-bottom: 0px; 
}
.gender {
    gap: 20px; 
    padding: 20px; 
    padding-top: 0px;
    background-color: rgb(26, 15, 32);
    border-radius: 10px;
    border: 3px solid rgb(238, 228, 169); 
}
.gender h2::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.gender h2{
    color: rgb(75, 12, 12);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
}
.gender span::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.g-content p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
        opacity: 1;
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
.lucky h2::selection{
    background: rgb(143, 143, 143);
    color: rgb(75, 12, 12);    
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
.things li::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.things h4::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.things h2::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.things p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
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
.famous {
    padding: 30px;
}
.famous h2 {
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(238, 228, 169); 
    letter-spacing: 1px;
    justify-content: center;
}
.fam {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
}
.fa{
    display: grid;
    grid-gap: 20px;
    background-color: rgb(26, 15, 32);
}
.f {
    background: rgb(161, 41, 41);
    width: 300px;
    transition: width 2s;
    display: flex;
    flex-direction: row;
    padding-top: 0px;
    padding-left: 20px;
    padding-bottom: 5px;
    padding-right: 20px;
    overflow: hidden;
    white-space: nowrap;
}
.f p {
    color:rgb(26, 15, 32);
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
}
.f h3 {
    color:rgb(238, 228, 169);
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
    font-weight: bold; 
    padding-right: 10px;
}
.f:hover {
    width: 800px;
}
.out p::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.out p{
    color: rgb(238, 228, 169);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
}
.out a::selection{
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
.out a{
color: rgb(161, 41, 41); 
}
.out a:hover{
    color:rgb(75, 12, 12);
}

</style>
