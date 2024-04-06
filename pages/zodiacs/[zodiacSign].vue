<template>
    <PageHeader></PageHeader>
    <ZodiacHeader></ZodiacHeader>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />

    <main>    
        <div class="r">
            <div v-html="data[zodiacSign]?.letter"></div>
        <div class="rs">     
        <p> {{ data[zodiacSign]?.summary }} </p>  
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
                <input type="checkbox" id="toggle">
                <label for="toggle">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                    <input type="checkbox" id="toggle2">
                <label for="toggle2">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                <input type="checkbox" id="toggle3">
                <label for="toggle3">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                    <input type="checkbox" id="toggle4">
                <label for="toggle4">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                    <input type="checkbox" id="toggle5">
                <label for="toggle5">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                    <input type="checkbox" id="toggle6">
                <label for="toggle6">
                <span class="material-symbols-outlined" style="font-size: xxx-large;color:rgb(75, 12, 12);">
                    expand_circle_down
                </span>
                </label>
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
                <p>Check out the <NuxtLink to="{{ data[zodiacSign]?.daily }}">
               daily
            </NuxtLink>/<NuxtLink to="{{ data[zodiacSign]?.yearly }}">
               yearly
            </NuxtLink>
                horoscope for {{ data[zodiacSign]?.out }}</p>
            </div>
        </footer>
</template>

<script setup lang="ts">

const { params } = useRoute();
const zodiacSign: string = params.zodiacSign as string;

const data: Record<string, Record<string, string>> = {
    rat: {
        letter: '<svg width="87.3" height="92.607" viewBox="0 0 87.3 92.607" xmlns="http://www.w3.org/2000/svg"><g id="svgGroup" stroke-linecap="round" fill-rule="evenodd" font-size="9pt" stroke="#000" stroke-width="0.25mm" fill="#000" style="stroke:#000;stroke-width:0.25mm;fill:#000"><path d="M 77.5 3.8 L 43.9 3.8 L 43.9 13 L 65.7 13 L 65.7 18.4 L 44.5 18.4 L 44.5 27.3 L 65.7 27.3 L 65.7 33.1 L 14.8 33.1 L 14.8 27.2 L 35.8 27.2 L 35.8 18.3 L 14.8 18.3 L 14.8 12.7 C 22.2 11.8 30 10.5 36.4 8.9 L 30.7 0 C 23.567 1.981 12.703 3.963 3.362 5.166 A 229.209 229.209 0 0 1 3.1 5.2 L 3.1 42.3 L 77.5 42.3 L 77.5 3.8 Z M 50.3 62 L 44.4 68.1 L 44.4 45.2 L 33.6 45.2 L 33.6 76.1 A 10.367 10.367 0 0 1 33.391 78.242 C 32.83 80.901 31.232 82.293 29.7 83.1 A 10.874 10.874 0 0 1 30.176 83.747 C 31.561 85.77 33.102 89.17 33.756 91.456 A 13.062 13.062 0 0 1 33.9 92 C 36.3 90.8 39.9 89.9 61.4 86.8 A 32.502 32.502 0 0 1 61.321 85.602 C 61.205 83.25 61.231 79.963 61.4 77.6 L 44.4 79.7 L 44.4 68.3 C 47.698 70.528 52.029 73.551 54.631 75.811 A 24.141 24.141 0 0 1 55.5 76.6 L 61.7 69.6 A 30.437 30.437 0 0 0 60.313 68.503 C 57.54 66.424 53.422 63.856 50.3 62 Z M 15.3 79.6 L 15.3 45.1 L 4 45.1 L 4 75.9 C 4 79.643 2.249 81.553 0.499 82.618 A 9.239 9.239 0 0 1 0 82.9 A 12.666 12.666 0 0 1 0.476 83.608 C 1.86 85.811 3.401 89.447 4.055 91.91 A 14.819 14.819 0 0 1 4.2 92.5 A 10.035 10.035 0 0 1 5.067 92.08 C 7.239 91.149 11.314 90.243 24.463 88.227 A 1175.178 1175.178 0 0 1 28.6 87.6 A 30.333 30.333 0 0 1 28.528 86.522 C 28.406 84.118 28.442 80.579 28.7 78 L 15.3 79.6 Z M 73.3 44.7 L 61.7 44.7 A 314.588 314.588 0 0 0 62.139 60.261 C 63.304 80.783 67.031 92.6 76.7 92.6 A 11.355 11.355 0 0 0 81.243 91.818 C 84.37 90.462 86.176 87.142 87.014 80.341 A 62.232 62.232 0 0 0 87.3 77.4 A 19.827 19.827 0 0 1 85.7 76.739 C 83.675 75.802 81.495 74.433 79.851 72.933 A 15.686 15.686 0 0 1 79.6 72.7 C 79.447 77.597 79.06 80.035 78.349 80.91 A 0.935 0.935 0 0 1 77.6 81.3 A 2.088 2.088 0 0 1 75.999 79.852 C 74.011 75.938 72.819 64.117 73.3 44.7 Z M 50.4 46.9 L 44.8 53.1 A 269.454 269.454 0 0 1 46.746 54.355 C 50.029 56.492 53.793 59.059 55.7 60.8 L 61.6 53.9 A 32.013 32.013 0 0 0 60.324 52.937 C 57.973 51.244 54.552 49.132 51.627 47.548 A 63.714 63.714 0 0 0 50.4 46.9 Z M 27.1 60.2 L 33.3 53.5 A 56.737 56.737 0 0 0 32.262 52.732 C 29.623 50.82 25.588 48.163 22.7 46.5 L 16.8 52.4 A 135.335 135.335 0 0 1 18.634 53.664 C 21.685 55.802 25.113 58.378 27.1 60.2 Z M 26.4 75.5 L 32.7 68.5 A 58.549 58.549 0 0 0 31.617 67.741 C 29.053 65.982 25.273 63.617 22.419 61.969 A 101.938 101.938 0 0 0 22.3 61.9 L 16.4 68.1 A 157.327 157.327 0 0 1 18.185 69.309 C 20.795 71.101 23.718 73.218 25.631 74.83 A 27.154 27.154 0 0 1 26.4 75.5 Z" vector-effect="non-scaling-stroke"/></g></svg>',
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
        personality_2: "Rats love being in a group and may feel lonely when they’re on their own. They are friendly and easy-going, finding it easy to make friends despite a slight inclination to secrecy and introversion. ",
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
        daily: "/horoscope/rat/daily",
        yearly: "horoscope/rat/yearly",
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
        summary: "In Chinese astrology, the Dragon is one of the twelve animal signs that represent different personality traits and characteristics. The Dragon is the only mythical creature among the twelve signs.",
        personality_1: "Dragons present themselves as magnificent yet benevolent rulers who’re confident, generous, idealistic, and ambitious. In Chinese culture, these mythical creatures are in a class of their own, regarded as the givers of abundance and longevity. Dragon’s confidence is neither false nor empty, as they hold lofty ideals they’re striving toward— usually for the benefit of their community instead of themselves. They are independent thinkers who’ll never yield their highest conviction.",
        strengths: "ambition",
        strengths_2: "leadership",
        strengths_3: "charisma",
        strengths_4: "courage",
        strengths_5: "independence",
        weaknesses: "arrogance",
        weaknesses_2: "hot-tempered",
        weaknesses_3: "overbearing",
        weaknesses_4: "overly ambitious",
        weaknesses_5: "impatience",
        personality_2: "Dragons are wise and adventurous and, at times, temperamental and impulsive. They’ll be loved and admired by many but find it difficult to return such affection. This will be one of Dragon’s most important lessons. Even though they may not care to invest in relationships, Dragons cannot stay alone for too long without feeling desolate. Once they find that special someone, Dragons will guard that person as their treasure horde.",
        years: "Years of the Dragon",
        years_1: "1928",
        years_2: "February 23, 1928",
        years_3:"February 9, 1929",
        years_4:"1940",
        years_5:"February 9, 1940",
        years_6:"January 26, 1941",
        years_7:"1952",
        years_8:"January 27, 1952",
        years_9:"February 13, 1953",
        years_10:"1964",
        years_11:"February 13, 1964",
        years_12:"February 1, 1965",
        years_13:"1976",
        years_14:"January 31, 1976",
        years_15:"February 17, 1977",
        years_16:"1988",
        years_17:"February 17, 1988",
        years_18:"February 5, 1989",
        years_19:"2000",
        years_20:"February 5, 2000",
        years_21: "January 23, 2001",
        years_22: "2012 ",
        years_23: "January 23, 2012",
        years_24: "February 9, 2013",
        years_25: "2024",
        years_26: "February 10, 2024",
        years_27: "January 25, 2025",
        years_28: "2036",
        years_29: "January 28, 2036",
        years_30: "February 14, 2037",
        overall: "Dragons are strong and independent figures, but they yearn for support and love. ",
        metal: "Metal Dragons are straightforward and expressive, possibly emotionally volatile and capricious when they’re young. If success is desired, they must go through a difficult period that shapes them into a more tenacious and steady person. Metal Dragons have an excessive need for the finer things in life, and they’ll have opportunities to create wealth, but they must learn the art of money management to ensure a comfortable retirement for themselves.",
        metal_years: "1940, 2000",
        water: "Water Dragons are energetic and persevering, but unlike other Dragons, they may appear to lack personality and self-possession. Their water-like nature means they prefer to go with the flow, although they also have a selfish streak. To succeed in life, they’ll need to become more decisive instead of leaning on others’ input. Independence is key, even if they’ll be blessed with close friends who can act as mentors throughout their careers.",
        water_years: "1952, 2012",
        wood: "Wood Dragons are intelligent, attractive, and usually well-loved. They’re blessed with the ability to make good use of their environment and have an intuitive sense of timing, so success will not be difficult to attain. They’re very popular and move in different social circles, but because of their fiery temper, Wood Dragons may not be as lucky or auspicious in their intimate relationships. In finances, Wood Dragons’ fortunes often come enviably quickly.",
        wood_years: "1964, 2036",
        fire: "Fire Dragons are loving, enterprising, and hardworking. They put 110% into everything they do, and their energy is often infectious and attractive, ensuring extraordinary personal achievements as well as success for the team they’re on. Love comes to them naturally without any pretension. Once they find it, they’ll show such loyalty to move even the coldest of hearts and put the interest of that special someone before even their own.",
        fire_years: "1976, 2036",
        earth: "Earth Dragons are taciturn introverts who care little about fame or fortune. They’re talented and have a superb ability to get things done, although they’ll continue to shy away from public recognition or the limelight. Despite their low-key presence, Earth Dragons are conquerors and will never be satisfied with easy work—they need challenges to propel them forward and difficulties to overcome. It’s the only path to happiness for them.",
        earth_years: "1928, 1988",
        compatibility: "In matters of the heart, Rabbits start out suspicious of others’ motives, since their cautious nature means that many of their ideas and understanding of the world—whether real or imaginary—tend toward the negative. Once they truly fall in love for the first time, they’ll learn to be honest with their feelings without being defensive. In many ways, true love will be the beginning of Rabbits’ farewell to loneliness.",
        best: "Dragon and Rat",
        best_more: "Dragon and Rat seem so different, yet they share the same practical quality that both will use to affect reality in some way. It’s a breath of fresh air to find someone who understands that! Dragons believe in making the world a better place as advocates and pioneers, while Rats build a comfortable nest—their own little world. Together, these zodiacs are so energized that both visions can be realized.",
        gender: "Female Dragon and Male Rat",
        gender_more: "Both partners are intelligent and quick, qualities they will find admirable in their partner and attract them to each other. Dragon makes Rat feel safe, so neither will suffer jealousy or insecurity in their relationship. If both had time to mature, their relationship should have few disruptions or confrontations since they have the power to create a family filled with excitement and common interests, making them the envy of others.",
        gender_reverse: "Female Rat and Male Dragon",
        gender_reverse_more: "When these partners join hands, they will be able to build a steady financial foundation that ensures no matter what difficulties they face in the future, they’ll work as a team to ultimately emerge triumphant. In this pairing, Dragon is courageous and intelligent, easily achieving success in the workplace, while Rat is economically prudent, growing into the kind of wife who leaves their husband worry-free to pursue their professional goals.",
        best_2: "Dragon and Monkey",
        best_more_2: "For signs known for their sharp intellect, Dragon and Monkey seem to love each other in that completely illogical way that many find foolish. Underneath the passion, however, is the meeting of two equal minds. Monkey seems the only one who can bring their mighty Dragon down to earth and teach them how to delight in the little things, while Dragon lends a higher vantage point to their whimsical partner.",
        gender_2: "Female Dragon and Male Monkey",
        gender_more_2: "Dragon is intelligent, ambitious, and goal-oriented. They’re unlikely to devote all their energy to love. Fortunately, this is precisely what Monkey seeks in their ideal mate, and they’ll work hard to match Dragon’s great strides. The best way for them to be together is to establish a common goal—whether professional or personal—which will spur both partners to achieve more. It’s that camaraderie that’ll keep them glued for life.",
        gender_reverse_2: "Female Monkey and Male Dragon",
        gender_reverse_more_2: "Both parties are logical and sensible, yet after they meet, this pair will discover the hidden romance in their own personality traits and shower their partner with affection. They will sincerely appreciate the other’s best qualities. After making a commitment, these two will turn their gaze towards the future and each work to build the life they want. They’ll help each other professionally and feel closer as success arrives for both.",
        best_3: "Dragon and Rooster",
        best_more_3: "Dragon and Rooster seem to share one trait—their vanity. But while this may rub others the wrong way, they will recognize the pride in who they are and what they achieve that’s hidden underneath. Undeniably high-achieving, Dragon and Rooster can learn to be the kind of power couple that are most resilient where they are not only there to celebrate the other’s success, but to nurse their failure, too.",
        gender_3: "Female Dragon and Male Rooster",
        gender_more_3: "This is a complementary pair, as Dragon is intelligent but at times impulsive, while Rooster is logical and analytical. The Rooster man will be the voice of reason much needed in the Dragon woman’s life. Rooster’s enthusiasm for love usually comes quickly, although it tends to wane just as quickly, but Dragon’s vitality and independent streak will certainly leave Rooster always hankering for more—for the rest of their lives!",
        gender_reverse_3: "Female Rooster and Male Dragon",
        gender_reverse_more_3: "These zodiac signs are usually able to reach the top of their respective disciplines on their own since they’re both proud, capable, and independent, but this relationship will give them the personal satisfaction they crave. Rooster woman is not one to be conquered easily, so Dragon will have to put in more effort than he’s used to earlier on in the relationship. Once they’re together, nothing will ever break them apart.",
        worst: "Dragon and Dog",
        worst_more: "This is not an ideal match for love and marriage since Dragon and Dog will have little in common and often find themselves mute in each other’s company. Not exactly the warm relationship either craves. Dragon cares about the world and may find Dog, who’s more concerned about their day-to-day life, rather dull, while to Dog, Dragon is just a touch too condescending. They’re not built for the same lifestyle.",
        worst_2: "Dragon and Rabbit",
        worst_more_2: "Rabbit can’t be themselves with Dragon as their mate because Dragon picks on Rabbit for being careless and complacent, resigning Rabbit to loneliness within the relationship until it becomes too much for this gentle creature. Their personalities clash because Dragon is decisive and overwrought, always wanting to press things forward relentlessly, which tires Rabbit out, while Rabbit is quiet and sensitive with a rich emotional life that Dragon will ignore. ",
        lucky_1: "1, 6, 7",
        lucky_2: "Gold, Silver, White",
        lucky_3: " East, North, West",
        lucky_4: "Bleeding Heart Vine, Dragon Flowers",
        lucky_5: "March, July, August, November",
        lucky_6: "Ruby, Amethyst",
        lucky_7: "Dragon figurines or ornaments",
        unlucky_1: "3, 8, 9",
        unlucky_2: "Red, Black",
        unlucky_3: "South, Southeast",
        unlucky_4: "April, May, June, October",
        unlucky_5: "Aquamarine",
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
        summary: "In Chinese astrology, the Dragon is one of the twelve animal signs that represent different personality traits and characteristics. The Dragon is the only mythical creature among the twelve signs.",
        personality_1: "Snakes are sensitive, effective, and adaptable, positive personality traits often complemented by a considerable intelligence. They are usually amiable and even-tempered, showing a cool and calm exterior punctuated by occasional bouts of perfectly-timed energy and passion. They move elegantly through the social sphere, armed with their wide range of interests and hobbies, which add to their intrigue and mystery. They’re often artistic, which makes them taste-makers others look to for guidance.",
        strengths: "wisdom",
        strengths_2: "intelligence",
        strengths_3: "gracefulness",
        strengths_4: "intuition",
        strengths_5: "self-reliance",
        weaknesses: "manipulativeness",
        weaknesses_2: "secretiveness",
        weaknesses_3: "vindictiveness",
        weaknesses_4: "suspiciousness",
        weaknesses_5: "jealousy",
        personality_2: "Snakes show their true value by remaining calm and collected in emergencies, not losing an ounce of their ability to analyze the situation and come up with the best solution while remaining a dependable presence. In daily life, Snake people are easy-going and fascinating for their mystery while also needing alone time to smooth their sensitivities. If they can learn to be vulnerable, Snake will find a new world opening to them.",
        years: "Years of the Snake",
        years_1: "1929",
        years_2: "February 10, 1929",
        years_3:"January 29, 1930",
        years_4:"1941",
        years_5:"January 27, 1941",
        years_6:"February 14, 1942",
        years_7:"1953",
        years_8:"February 14, 1953",
        years_9:"February 2, 1954",
        years_10:"1965",
        years_11:"February 2, 1965",
        years_12:"January 20, 1966",
        years_13:"1977",
        years_14:"February 18, 1977",
        years_15:"February 6, 1978",
        years_16:"1989",
        years_17:"February 6, 1989",
        years_18:"January 26, 1990",
        years_19:"2001",
        years_20:"January 24, 2001",
        years_21: "February 11, 2002",
        years_22: "2013 ",
        years_23: "February 10, 2013",
        years_24: "January 30, 2014",
        years_25: "2025",
        years_26: "January 29, 2025",
        years_27: "February 16, 2026",
        years_28: "2037",
        years_29: "February 15, 2037",
        years_30: "February 3, 2038",
        overall: "Snakes are often characterized by their wisdom, intuition, and grace, navigating life with calculated precision and a mysterious allure.",
        metal: "Metal Snakes are powerful and have no shortage of courage to make progress. They are also strong-willed, determined, and capable, and as a result, will often find themselves surrounded by many admiring subordinates at work. Metal Snakes are dazzling and elegant, a standout in a crowd in every way, but they may come off as overconfident and even conceited if they aren’t careful. In fact, they’re supportive leaders, teachers, and advisors.",
        metal_years: "1941, 2001",
        water: "Water Snakes are active, smart, and creative, but they may suffer a great deal of emotional turbulence, especially in their youth. That may also be why they’re adventurers—they’re seeking something that isn’t as easily found. Water Snakes are very considerate of others and a pleasure to be around. In terms of wealth, they may receive unexpected financial gains, which they should invest wisely in real estate, gold, or index funds.",
        water_years: "1953, 2013",
        wood: "Wood Snakes prefer order, so they’ll make sure their environment is neat and beautifully decorated. They are naturally accurate when making analyses and calculations, making them an excellent fit for a career in academia or finance. Outside work, Wood Snakes love antiques and anything that looks beautiful and unique. They can be passive and lack motivation at work, so they’ll need the encouragement of their mentors and loved ones to succeed.",
        wood_years: "1965, 2025",
        fire: "Fire Snakes are wise and insightful, often keen observers who can take stock of any situation, which endows them with social skills. But they can be emotionally stingy, requiring others to make the first move. At work, Fire Snakes can be impatient, needing constant stimulation. They’re innovators, above all, and with the right environment, they’ll be able to succeed on the merit of what they create with their active imagination.",
        fire_years: "1977, 2037",
        earth: "Earth Snakes are loyal and sincere, popular for their quick mind, physical prowess, and compassion, and they’re able to make friends for life. At the same time, the slightest criticism can make Earth Snakes feel depressed. They’re hardworking, goal-oriented and will constantly strive to improve themselves at work. Love doesn’t seem to come easily for this group, but if they keep working at it, they’ll definitely find the right life partner.",
        earth_years: "1929, 1989",
        compatibility: "Snakes are passionate and delicate in love, which may surprise their romantic interests. Over time, they’ll also grow into loyal marriage partners, even if their charm means Snakes will usually face many temptations throughout life. In return, Snakes demand the same loyalty from their partner and become suspicious. It’s best for Snake to express their emotions and doubts with honesty, which the right partner will respond to with loving affirmation.",
        best: "Snake and Rooster",
        best_more: "Snake is one of those effortlessly cool zodiacs, while Rooster seems to be ferocious in all their endeavors. Together, their love compatibility is like water and fire, but instead of fizzling out, they’re the definition of opposites attract. In fact, they’re alike in subtle ways that only the two of them recognize. Rooster is logical and analytical despite the appearance of being hot-headed, while like Rooster, Snake possesses a passion that runs deep.",
        gender: "Female Snake and Male Rooster",
        gender_more: "This is a beautiful match as Rooster is proud and passionate, while Snake is calm and principled. They will keep each other entertained and in check and move up in society as an admirable power couple. Snake is gentle and considerate of her more outgoing mate, while Rooster will, in turn, happily shoulder the responsibility for the finances and material abundance of this relationship and make Snake feel safe and happy.",
        gender_reverse: "Female Rooster and Male Snake",
        gender_reverse_more: "Snake men appear mature and stable, although at heart, they appreciate beauty greatly and often place an emphasis on their other half’s appearance. And Rooster women are certainly one of the most beautiful zodiac signs. But more than that, Snake also adores Rooster’s wisdom and emotional intelligence under their eye-catching appearance, inspiring them to put in a great deal of effort to pursue Rooster, and Rooster will appreciate Snake’s devotion.",
        best_2: "Snake and Ox",
        best_more_2: "Who ever pictured these two together? Ox is apparent in their diligent tenacity, while Snake is inscrutable in their cautious mystery. But in fact, they share values that reassure their partner of a stable partnership. This couple will quietly build a safe nest together. They won’t be much heard of until they emerge having hit the important milestones in life. That’s the nature of both their personalities and their love.",
        gender_2: "Female Snake and Male Ox",
        gender_more_2: "This couple shares many common values and, therefore, will be able to build a steady relationship in which both work hard to create a stable lifestyle. Neither will be impatient either in work or in their private life but will prove excellent and constant support for the other person. In such a relationship, both partners are likely to find work going better than before because neither is wasting energy on romantic woes. They spur each other on to become the best versions of themselves.",
        gender_reverse_2: "Female Ox and Male Snake",
        gender_reverse_more_2: "Ox women are steadfast and traditional. Although Snake may, funnily enough, find his mate hard to understand at first, he will quickly grow to appreciate Ox’s stable emotion and disposition, as he’s prone to suspicion. In addition, Snake can relax around Ox, and in return, Snake offers loyalty and support to his Ox mate and contributes an emotional richness to the relationship that Ox isn’t likely to ever have experienced.",
        best_3: "Snake and Monkey",
        best_more_3: "Both Snake and Monkey are known for their intelligence, although Monkey’s quicker and cleverer, while Snake is more analytical. They will recognize the quality of the other’s intellect, fostering respect before the emergence of love. The division of labor within this union will be natural—Monkey is much more outgoing, while Snake prefers to be behind the scenes despite their innate charm. Together, they’ll represent an integrated union built on solid ground.",
        gender_3: "Female Snake and Male Monkey",
        gender_more_3: "Snake and Monkey are both quick and observant, while at the same time, both are prone to suspicion and neuroticism. They’ll share a reassured understanding that they are unlikely to find with any other zodiac. One area of growth is they’ll have to learn to be honest with each other, which takes trust from both. Once that happens, nothing will stop this couple from living their elegant and lively life.",
        gender_reverse_3: "Female Monkey and Male Snake",
        gender_reverse_more_3: "Monkey women are lively and cheerful. They are skilled at and enjoy socializing. These are traits that Snake admires in their enchanting mate, and he’ll give his all to his optimistic partner, even spoiling her. Once married, Snake will be patient with Monkey and contribute all their wealth to the partnership, which Monkey appreciates. Unless Monkey is immature and decides the relationship isn’t enough, this will be a long-lasting marriage.",
        worst: "Snake and Pig",
        worst_more: "Quarreling will be the least of this couple’s problems, as being together means that they somehow always find themselves in accidents or wounding each other. Either way, someone’s going to get hurt until they split! Snake and Pig never seem to hear each other’s real concerns and always find the other person incomprehensible. They want different things, so it’ll take something of a miracle for these two zodiacs to find happiness together.",
        worst_2: "Snake and Tiger",
        worst_more_2: "Despite both partners’ charms, these two find each other annoying when they spend any amount of time together since they aspire to such different lifestyles that they’ll find the other person’s dreams vain and useless. Tiger’s cocky, while Snake can’t show their authentic self in this relationship, which will quickly lead to disputes as if they are not even speaking the same language. Why drag yourselves through this relationship muck?",
        lucky_1: "2, 8, 9",
        lucky_2: "Red, Light Yellow, Black",
        lucky_3: "Northeast, Southwest",
        lucky_4: "Orchid, Cactus",
        lucky_5: "March, May, June, October",
        lucky_6: "Topaz, Jasper",
        lucky_7: "Snake figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Ruby",
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
        summary: "In Chinese astrology, the Horse is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Horse are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "Horses are leaders who rarely accept defeat, so they can motivate themselves to put up an active fight in everything they do. This can come off as tenacity, endurance, stubbornness, or even foolhardiness in certain situations. Once Horse matures and learns to harness this energy, they’ll be unstoppable since they’re agile and shrewd thinkers who innately understand human nature. They’re also principled, so their efforts will be put toward a good cause.",
        strengths: "energy and vitality",
        strengths_2: "adventurous spirit",
        strengths_3: "optimism",
        strengths_4: "passion",
        strengths_5: "versatility",
        weaknesses: "lack of focus",
        weaknesses_2: "overconfidence",
        weaknesses_3: "recklessness",
        weaknesses_4: "stubbornness",
        weaknesses_5: "impulsiveness",
        personality_2: "Socially, Horse has an outgoing and agreeable personality. They speak as quickly as they think and act, and they aren’t shy about showing off their talents and capabilities because to be falsely self-effacing wouldn’t be authentic.",
        years: "Years of the Horse",
        years_1: "1918",
        years_2: "February 11, 1918",
        years_3:"January 31, 1919",
        years_4:"1930",
        years_5:"January 30, 1930",
        years_6:"February 16, 1931",
        years_7:"1942",
        years_8:"February 15, 1942",
        years_9:"February 4, 1943",
        years_10:"1954",
        years_11:"February 3, 1954",
        years_12:"January 23, 1955",
        years_13:"1966",
        years_14:"January 21, 1966",
        years_15:"February 8, 1967",
        years_16:"1978",
        years_17:"February 7, 1978",
        years_18:"January 27, 1979",
        years_19:"1990",
        years_20:"January 27, 1990",
        years_21: "February 14, 1991",
        years_22: "2002",
        years_23: "February 12, 2002",
        years_24: "January 31, 2003",
        years_25: "2014",
        years_26: "January 31, 2014",
        years_27: "February 18, 2015",
        years_28: "2026",
        years_29: "February 17, 2026",
        years_30: "February 5, 2027",
        overall: "Horses embody strength, independence, and an adventurous spirit, navigating life with resilience and an unwavering pursuit of freedom and excitement.",
        metal: "Metal Horses are kind-hearted, outspoken, and willing to help others. They dislike advice or criticism from others, so they may be stuck on the wrong idea for too long and end up not accomplishing much. They’re just as stubborn when it comes to love, as once married, their devotion to their partner and family will prove immovable, with Metal Horses themselves maturing into calm rationality as time goes on.",
        metal_years: "1930, 1990",
        water: "Water Horses have a self-sacrificial spirit, although they can also be impatient and emotional. They’re thoughtful and suitable for great ambition because they’ll often receive unexpected help from unlikely quarters, especially from the opposite gender. Although they’re not particularly sexy, Water Horses can easily attract attention with their cheery personality. A relationship with them will require patience from their partner, but once married, they’ll quickly grow into their true potential.",
        water_years: "1942, 2002",
        wood: "Wood Horses have a rich imagination and inspired insights. They can read others and make themselves likable, while they also tend to be impatient and overly emotional, and will need to cultivate perseverance and patience. In love, Wood Horses are popular and will remain so even after they settle down. Extramarital affairs are a real risk with Wood Horses and will likely prove detrimental to the stability of their life.",
        wood_years: "1954, 2014",
        fire: "Fire Horses are lively, passionate, and unrestrained by nature. They’re leaders who can become headstrong, well-intentioned helpers who can become condescending, and ardent lovers who can become overbearing—in summary; they’re too much of everything! But that’s also why Fire Horses will be blessed with wealth since they tend to work very hard, have great love affairs that seem destined for the book pages, and be remembered for their generosity and vitality.",
        fire_years: "1966, 2026",
        earth: "Earth Horses are optimistic and kind-hearted souls who are dedicated to their friends. They’ll never feel lonely in life, and in return, they’ll be blessed with many friends who will love them for their giving spirit. Earth Horses will have ample fortune in wealth and money, but they’re advised to save. In love, they’ll appear less attractive, but once their dense exterior is penetrated, their partner will discover a passionate lover.",
        earth_years: "1918, 1978",
        compatibility: "Horses are energetic, lively, and generous, so they will be popular with the opposite sex. When it comes to love compatibility, their hot temper and stubborn nature mean they tend to gravitate towards romantic partners who are more easygoing and gentle. They prefer to take the assertive role and enjoy the pursuit and eventual conquest of the object of their affection. Horses need freedom, so if their partner is needy or clingy, Horses may feel stifled.",
        best: "Horse and Tiger",
        best_more: "Tigers may represent characteristics that Horses dislike about themselves— they’re temperamental, hot-headed, and often cocky. But in fact, they bring out the best in each other and allow the other to grow out of their worst. It’s as if both Tiger and Horse finally have someone who can keep up with their own breakneck speed, which can be thrilling to Horse, who would have gotten bored with a less charismatic partner.",
        gender: "Female Horse and Male Tiger",
        gender_more: "This is a surprisingly good match because Tiger can provide domestic intimacy and calmness for Horse, making it easy for Horse to mature into a good wife and mother in addition to their career ambition. They’re an energetic and hardworking pair, working together to create a beautiful atmosphere at home. Although both can be temperamental, it seems Tiger and Horse understand each other well enough, which will prevent most disagreements.",
        gender_reverse: "Female Tiger and Male Horse",
        gender_reverse_more: "Although Horses tend to prefer mellower zodiac signs, with Tiger, they’re willing to make an exception because these two signs have a lot in common —seemingly, birds of the same feather end up flocking together!.  Both Tiger and Horse are energetic and ambitious, so if they find a common goal or cause, they will prove unstoppable. In each other’s company, they’ll revel in the joy of being in true communion.",
        best_2: "Horse and Dog",
        best_more_2: "Dog is practically Horse’s dream come true when it comes to romance since this spirited and high-strung zodiac has always dreamed of a mellower partner who can give them a respite from their own passionate nature. In return, Horse will take on the leadership role in the relationship—as they naturally prefer—and give their more homely partner a sense of direction and movement in life, exactly what Dog wants, too.",
        gender_2: "Female Horse and Male Dog",
        gender_more_2: "There isn’t anyone more loyal than Dog, which Horse loves in her man. This couple will support each other while intuitively leaving enough personal space for their faithful partner, giving them the space to grow. Neither will be excessively critical since both are genuinely impressed by their partner’s sincerity and ability to communicate. Horse will find Dog to be a mature partner, often giving her a new perspective in life.",
        gender_reverse_2: "Female Dog and Male Horse",
        gender_reverse_more_2: "This pair is likely to grow old together because they’re both generous and cheerful and full of vitality and love for life. They’ll start a family and build a home life that’s never short of joy. Horse is intelligent and insightful, while Dog is sincere and forgiving—a quality he’ll need. In return, Horse will value Dog’s loyalty and show her the love she’ll need to flourish in her own right.",
        best_3: "Horse and Goat",
        best_more_3: "Who else can better soothe the passionate Horse when they’re riled up than the gentle and mild Goat? A few well-chosen words and a knowing touch from their better half, and Horse will magically settle down. Many misunderstand Goat to be ambition-less, but not Horse. They know their Goat to be as hardworking—or even stubborn—as themselves when it comes to something they care about, which Horse respects and adores.",
        gender_3: "Female Horse and Male Goat",
        gender_more_3: "This is a union with an easygoing heart-to-heart connection since Goat is generally sentimental, kind, and family-oriented, while Horse is cheerful and independent. Together, these two are destined for a lifetime of happiness and fulfillment. Goat won’t hesitate to take the reins in making sure they stay intimate and close emotionally, which gives Horse a sense of a happy family while allowing them a wide berth for their independent nature.",
        gender_reverse_3: "Female Goat and Male Horse",
        gender_reverse_more_3: "This couple will fall in love and get married before long because neither will find a better match. Although Horse is fiery while Goat is mild, they share the same goals and values in life. Once they marry, this pair will spur each other on to reach their true potential because they can compensate for each other’s weaknesses while greatly appreciating their strengths. A warm and joyous union is assured.",
        worst: "Horse and Rat",
        worst_more: "Horse and Rat cannot seem to stay together for long, even if the relationship started as a loving union, because while they are agreeable and well-liked, they’re also both too headstrong to make any concessions. Horse is demanding and asks Rat to give in to their needs, while Rat will react by ignoring Horse. This leads to frequent conflicts that neither will bother to resolve, making theirs a difficult match.",
        worst_2: "Horse and Ox",
        worst_more_2: "Horse and Ox find their way to each other and may start a relationship, but soon conflicts and disputes arrive, and neither can remember why they were drawn to the other in the first place. Horse loves freedom, which makes Ox feel insecure, while Ox’s stability and steadiness bore Horse. What started quickly as a passionate love affair is more likely to result in a bitter breakup rather than a happy marriage.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        summary: "In Chinese astrology, the Goat, also known as the Sheep or Ram, is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Goat are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "Goats (sometimes also translated as Rams) are the most tender and mild of the zodiac signs, known for their honest, kind, and empathic nature. They’re selflessly giving, willing to lend their last penny to their closest friends without a second thought. They’re born compassionate, so when they meet others who have suffered, Goats may grow despondent themselves. They’re also creative, almost indulgently so, with no shortage of whimsical images and ideas floating around in their mind.",
        strengths: "gentleness",
        strengths_2: "creativity",
        strengths_3: "harmony",
        strengths_4: "intuition",
        strengths_5: "resilience",
        weaknesses: "indecisiveness",
        weaknesses_2: "over-sensitivity",
        weaknesses_3: "passivity",
        weaknesses_4: "over-idealization",
        weaknesses_5: "dependence on others",
        personality_2: "Socially, Goats are soft-spoken, elegant, and personable, meek on the outside yet strong and resilient on the inside. If anyone mistakes their docility as a weakness, however, Goats will be sure to deliver a rude awakening.",
        years: "Years of the Goat",
        years_1: "1919",
        years_2: "February 1, 1919",
        years_3:"February 19, 1920",
        years_4:"1931",
        years_5:"February 17, 1931",
        years_6:"February 5, 1932",
        years_7:"1943",
        years_8:"February 5, 1943",
        years_9:"January 24, 1944",
        years_10:"1955",
        years_11:"January 24, 1955",
        years_12:"February 11, 1956",
        years_13:"1967",
        years_14:"February 9, 1967",
        years_15:"January 29, 1968",
        years_16:"1979",
        years_17:"January 28, 1979",
        years_18:"February 15, 1980",
        years_19:"1991",
        years_20:"February 15, 1991",
        years_21: "February 3, 1992",
        years_22: "2003",
        years_23: "February 1, 2003",
        years_24: "January 21, 2004",
        years_25: "2015",
        years_26: "February 19, 2015",
        years_27: "February 7, 2016",
        years_28: "2027",
        years_29: "February 6, 2027",
        years_30: "January 25, 2028",
        overall: "Horses embody strength, independence, and an adventurous spirit, navigating life with resilience and an unwavering pursuit of freedom and excitement.",
        metal: "Metal Goats are kind-hearted, ambitious, with a strong sense of responsibility and ownership. They’re very principled but also stubborn and lack flexibility; therefore, they’re advised to specialize in a certain discipline until they become experts. Unlike their decisive work persona, in love Metal Goats are wishy-washy, taking one step forward before two steps back during courtship. Even when a relationship has run its course, they’ll have a hard time leaving.",
        metal_years: "1931, 1991",
        water: "Water Goats are gentle and self-sacrificial creatures loved by friends and family. They’re not competitive per se, although they’re motivated to seek knowledge, which means they will make excellent researchers, especially in the tech world. Water Goats are destined for a happy family life since they’ll find a suitable mate quite easily early in life. On the other hand, their fortune in wealth is less dependable, especially with financial investment.",
        water_years: "1943, 2003",
        wood: "Wood Goats are amiable, compassionate, and always willing to lend a helping hand. Unfortunately, it seems people rarely step up to help them, even among their intimate circle, so Wood Goats may often feel lonely. They’ll enjoy a stable love life despite frequent separations due to work. They seem able to maintain a solid relationship with their mate even when external temptations appear, which they’ll shrug off with ample grace.",
        wood_years: "1955, 2015",
        fire: "Fire Goats have a gentle and amiable personality, so they’re rarely disliked. They’re straightforward and loyal but prone to emotional turbulence in their younger years, so they’ll have to wait until middle age for success. To facilitate emotional maturation, Fire Goats are advised not to isolate themselves. Instead, they should gather a group of like-minded friends who can provide valuable insights and shed a different light on Fire Goats’ temperamental tunnel vision.",
        fire_years: "1967, 2027",
        earth: "Earth Goats are judicious and upright, with the propensity to speak their mind without much consideration. They’re not ones to scheme or calculate, which will allow them to find friends who appreciate their unique personalities. They’re likely to marry early, meeting someone in school, and ending up with this first love for the rest of their lives. Wealth may prove a major headache since investment often seems to go awry.",
        earth_years: "1919, 1979",
        compatibility: "Goats remain their mild selves in love, although they have the tendency to lose themselves in a relationship by being overly obedient to their other half, that is, unless it’s something they care deeply about. It’s more likely that Goats will become pushovers rather than pushy in love. As such, most Goats will share compatibility with equally amiable zodiacs like Rabbit and Pig, although some prefer charismatic and leader-like signs like Horse.",
        best: "Goat and Rabbit",
        best_more: "This is one of those couples that strikes everyone as enviably warm and caring towards each other since they’re similar in temperament and the kind of laid-back lifestyle that they want to create for themselves. There are still subtle differences to these mild zodiacs, as Rabbit is less easygoing and needs attention from their partner, while Goat is selfless and has no problem giving it to the object of their affection.",
        gender: "Female Goat and Male Rabbit",
        gender_more: "When these two come together, they often find themselves mirroring each other since both are easy-going, approachable, and romantic. The marriage will be full of joy as a result, with the attachment lasting a lifetime. Goat and Rabbit will fall in love in such a smooth way that others may believe love to always be this easy. They’re a match that knows how to accommodate the needs of their partner.",
        gender_reverse: "Female Rabbit and Male Goat",
        gender_reverse_more: "This is a match made in heaven since both are considerate and caring towards each other. Since both Goat and Rabbit are sweet-tempered, this union will likely lead to a warm and pleasant home life. Goat is a romantic and kind man who admires Rabbit’s delightful way of living—indeed, he’s proud to show her off. Meanwhile, Rabbit is good at reading Goat’s mind and giving him what he needs.",
        best_2: "Goat and Pig",
        best_more_2: "Goat appear mild, but they’re actually romantic and creative, which no one recognizes and appreciates better than Pig when these two come together. Goats beauty, indeed, shines most brightly in the eye of their beholder. Their home will be a sight to behold as well since Goat’s natural creative talents will have the backing of their generous Pig partner. Since both are agreeable introverts, they’ll love spending time together there.",
        gender_2: "Female Goat and Male Pig",
        gender_more_2: "This couple will naturally feel attracted to each other, as their personality traits are complementary, even as they share the same values and attitudes in life. Together, these two can revel in the simple pleasures. Goat and Pig can both live in the present without putting much pressure on their mate, so the relationship is one of harmony. Goat is more emotional, while Pig will bring a sense of security.",
        gender_reverse_2: "Female Pig and Male Goat",
        gender_reverse_more_2: "A beautiful pairing with both partners willing to sacrifice and make concessions for the good of the family. There will be few conflicts in this marriage, as they bring out the best in each other. Goat is usually sentimental and reserved with their mate, although they may occasionally experience some anxious moments. Pig is generous and sociable and will quickly put her husband’s mind at ease when this happens.",
        best_3: "Goat and Horse",
        best_more_3: "Who else can better soothe the passionate Horse when they’re riled up than the gentle and mild Goat? A few well-chosen words and a knowing touch from their better half, and Horse will magically settle down. Many misunderstand Goat to be ambition-less, but not Horse. They know their Goat to be as hardworking—or even stubborn—as themselves when it comes to something they care about, which Horse respects and adores.",
        gender_3: "Female Horse and Male Goat",
        gender_more_3: "This is a union with an easygoing heart-to-heart connection since Goat is generally sentimental, kind, and family-oriented, while Horse is cheerful and independent. Together, these two are destined for a lifetime of happiness and fulfillment. Goat won’t hesitate to take the reins in making sure they stay intimate and close emotionally, which gives Horse a sense of a happy family while allowing them a wide berth for their independent nature.",
        gender_reverse_3: "Female Goat and Male Horse",
        gender_reverse_more_3: "This couple will fall in love and get married before long because neither will find a better match. Although Horse is fiery while Goat is mild, they share the same goals and values in life. Once they marry, this pair will spur each other on to reach their true potential because they can compensate for each other’s weaknesses while greatly appreciating their strengths. A warm and joyous union is assured.",
        worst: "Goat and Ox",
        worst_more: "If this pair ends up together, both must do their best not to interfere with their partner’s privacy. Keeping a distance from each other is the only way for Ox and Goat to make their love work. Even then, once jealousy and possessiveness permeate the romance, it’s basically over between them, as both will unleash their most stubborn selves and collide. It’ll be difficult to communicate and get along with each other.",
        worst_2: "Goat and Rat",
        worst_more_2: "This is not an ideal marriage, but thankfully, they most likely won’t find their way to each other, whether at work or in love, since both are introverts who aren’t used to being the pursuer. It’s odd that even though both want a stable family life, somehow, Goat and Rat are unable to provide that sense of security for each other. Over time, the resentment builds until the relationship disintegrates.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        summary: "In Chinese astrology, the Goat, also known as the Sheep or Ram, is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Goat are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "It seems Monkey can always come up with the most innovative ideas, making many envious or resentful. Their creativity is synonymous with their unpredictability, so you never know what to expect with this mercurial sign. Monkeys are social—they’ll grow despondent if left alone for too long. As such, they need sounding boards in their friends and colleagues when they’re creating, as opposed to being locked away on their own.",
        strengths: "gentleness",
        strengths_2: "creativity",
        strengths_3: "harmony",
        strengths_4: "intuition",
        strengths_5: "resilience",
        weaknesses: "indecisiveness",
        weaknesses_2: "over-sensitivity",
        weaknesses_3: "passivity",
        weaknesses_4: "over-idealization",
        weaknesses_5: "dependence on others",
        personality_2: "This is a very practical sign, and their calculations often involve numbers, profits and losses, and the accumulation of wealth. With this advantage in intelligence, less evolved Monkeys can often feel rather superior to others.",
        years: "Years of the Monkey",
        years_1: "1920",
        years_2: "February 20, 1920",
        years_3:"February 7, 1921",
        years_4:"1932",
        years_5:"February 6, 1932",
        years_6:"January 25, 1933",
        years_7:"1944",
        years_8:"January 25, 1944",
        years_9:"February 12, 1945",
        years_10:"1956",
        years_11:"February 12, 1956",
        years_12:"January 30, 1957",
        years_13:"1968",
        years_14:"January 30, 1968",
        years_15:"February 16, 1969",
        years_16:"1980",
        years_17:"February 16, 1980",
        years_18:"February 4, 1981",
        years_19:"1992",
        years_20:"February 4, 1992",
        years_21: "January 22, 1993",
        years_22: "2004",
        years_23: "January 22, 2004",
        years_24: "February 8, 2005",
        years_25: "2016",
        years_26: "February 8, 2016",
        years_27: "January 27, 2017",
        years_28: "2028",
        years_29: "January 26, 2028",
        years_30: "February 12, 2029",
        overall: "Horses embody strength, independence, and an adventurous spirit, navigating life with resilience and an unwavering pursuit of freedom and excitement.",
        metal: "Metal Monkeys are clever and tough, cunning and decisive, and eloquent and stubborn. This group is naturally confident, so they make perfect entrepreneurs who won’t have to look far for investors who believe in their vision. They’ll marry later, if they do at all, because their priority will be to build a career and professional reputation first. They won’t lack friends, which will provide the emotional support they need earlier on.",
        metal_years: "1920, 1980",
        water: "Water Monkeys possess a rather infectious vitality, although their energetic presence is accompanied by pushiness and a more hands-on leadership style. They have the tendency to behave with arrogance, which may arouse resentment in their team. In marriage and romance, Water Monkeys will have strong, if not passionate, relationships all their lives. In terms of wealth, however, they’ll need to deal with fluctuating fortunes, so prepare and save for lean years.",
        water_years: "1932, 1992",
        wood: "Wood Monkeys are ambitious, and they stand to realize their career aspirations and enjoy an otherwise flourishing life. Although Monkeys are usually selfish, Wood Monkeys are compassionate in their actions and love to help friends. Because they’re workaholics, Wood Monkeys may neglect their romantic partner. Do not mistake this for an absence of love, however, because they’re dedicated to their union, even if they don’t remember to express their affections.",
        wood_years: "1944, 2004",
        fire: "Fire Monkeys are smart and passionate. They care about making a difference in the world, if only for their personal vision—they value justice and hold ideals for the way the world ought to be. Fire Monkeys will have a solid marriage that’s supplemented by a large social circle. But they’re advised not to jump into a relationship when they’re young, as they may well mature into a different person.",
        fire_years: "1956, 2016",
        earth: "Earth Monkeys are careful planners and hard workers. They don’t care about fame or fortune, but by applying themselves consistently, they can rise to the top of their field—even if in a quieter fashion. They’ll do their best to create a happy family as they instinctively feel the need for warmth and support. Fortune often comes to them unexpectedly because they don’t need much to feel abundant in life.",
        earth_years: "1968, 2028",
        compatibility: "Those born in years of the Monkey may seem vain on the surface and appear to care too much about their potential partner’s appearance, but inside, they’re actually yearning for deep and earth-shattering love compatibility. With the right partner, Monkeys will develop a mature depth to their character, as if with the assurance of true love, they’re finally able to discard the more changeable and capricious aspects of their personality.",
        best: "Monkey and Rat",
        best_more: "Rat is steady, whereas Monkey is mercurial, but that’s what attracts them to each other. As their relationship deepens, however, these two may well find that they have more in common than at first glance. Rat doesn’t want every day to be the same, although that’s exactly what they’d build if left to their own devices, while Monkey sometimes cannot execute their grand plans. Well, no need to look further here!",
        gender: "Female Monkey and Male Rat",
        gender_more: "Monkey and Rat together will release both partners’ full potential for the greater good of their family. Monkey is an excellent long-term strategist, while Rat will take the reins of day-to-day living, which is also important. Both will strive to improve themselves constantly in their journey together, although neither will require the same from their partner, making this a loving and friendly marriage from the start that will prosper without fail.",
        gender_reverse: "Female Rat and Male Monkey",
        gender_reverse_more: "This is a complementary pair not only in temperament but also in how they behave. Both find the other quite capable in ways that they aren’t themselves, and each respects their significant other as a result. So, this love affair will go smoothly from the start since they also have mutual understanding and great communication on their side, which are important ingredients for a relationship that will weather life’s inevitable storms.",
        best_2: "Monkey and Dragon",
        best_more_2: "It takes a spirited zodiac like Monkey to stand up to Dragon’s domineering ways because, goodness, does Monkey know how to rein Dragon in! With Monkey’s expert hand, Dragon can be almost as agreeable as Rabbit. That’s only where the couple’s harmonious home life is concerned because both partners will thrive and succeed out in the world in their different ways. Monkey will gain insight into the bigger picture they often lack.",
        gender_2: "Female Monkey and Male Dragon",
        gender_more_2: "This is a surprisingly romantic pairing, even though both are perceived as rational. Away from the public eye, however, these two seem to discover and stimulate the hidden passion within their partner—ooh la la! Both zodiac signs are social and well-liked, but Dragon brings a daring that Monkey doesn’t possess, while Monkey brings the fun that Dragon loves in his woman. Neither can seem to stop praising their mate.",
        gender_reverse_2: "Female Dragon and Male Monkey",
        gender_reverse_more_2: "This relationship will almost always lead to marriage, as Monkey and Dragon share characteristics, such as ambition and objectivity, that will allow both to thrive in their own right and as an indomitable family unit. Monkeys are practical and intelligent, while Dragons are tenacious and strong leaders. Both will discover their mate’s strengths right away and lean on each other as they become a pair destined for greatness and success.",
        best_3: "Monkey and Snake",
        best_more_3: "Monkey and Snake are certainly a match on the outside since both are stylish and together make a dashing couple. But that’s actually the least they have in common and find intriguing in their partner. Monkey has that lively zest for life that Snake secretly craves, while Snake’s calm and elegant persona is downright alluring to Monkey. Soon enough, their glitzy attraction to each other will deepen into true love.",
        gender_3: "Female Monkey and Male Snake",
        gender_more_3: "This is a pair that may come together quicker than anyone expects, and even more surprisingly, it’s a match that will last despite all the noise and not infrequent quarrels long into their prosperous retirement. Monkey and Snake have different personalities and interests, which is why they do disagree on certain subjects, but that’s precisely what gives them a life filled with surprises and richness instead of strife and misunderstanding.",
        gender_reverse_3: "Female Snake and Male Monkey",
        gender_reverse_more_3: "This couple is well-suited for each other, although early in the relationship, they’ll need to disarm their partner’s vigilance so that they can see each other as they truly are without any sensitivity or anxiety. Once that happens, both will give up their previous reservations and misbeliefs about love and finally reveal the full extent of their personalities. It’s only then that both will receive the best blessings in life.",
        worst: "Monkey and Tiger",
        worst_more: "This is a terrible pairing characterized by power plays from both sides. They’re certainly an ambitious couple, but both are more concerned with gaining the upper hand than working toward a common goal aspiration. Monkey wants to conquer Tiger and usually succeeds in this pairing, while Tiger, who’s usually confident, may become uncertain of their own abilities and lose themselves—a sad sight to witness in any zodiac sign.",
        worst_2: "Monkey and Pig",
        worst_more_2: "This is a damaging aspect for both zodiac signs, but they seem to strike gold after they marry, which leads them to stay together. They’ll soon discover that they can’t be themselves around their partner. Monkey will become unscrupulous in reaching their goals in this relationship, which will soon make Monkey and Pig a couple that looks enviable and successful on the outside—but miserable and inauthentic on the inside.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        summary: "In Chinese astrology, the Goat, also known as the Sheep or Ram, is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Goat are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "Goats (sometimes also translated as Rams) are the most tender and mild of the zodiac signs, known for their honest, kind, and empathic nature. They’re selflessly giving, willing to lend their last penny to their closest friends without a second thought. They’re born compassionate, so when they meet others who have suffered, Goats may grow despondent themselves. They’re also creative, almost indulgently so, with no shortage of whimsical images and ideas floating around in their mind.",
        strengths: "gentleness",
        strengths_2: "creativity",
        strengths_3: "harmony",
        strengths_4: "intuition",
        strengths_5: "resilience",
        weaknesses: "indecisiveness",
        weaknesses_2: "over-sensitivity",
        weaknesses_3: "passivity",
        weaknesses_4: "over-idealization",
        weaknesses_5: "dependence on others",
        personality_2: "Socially, Goats are soft-spoken, elegant, and personable, meek on the outside yet strong and resilient on the inside. If anyone mistakes their docility as a weakness, however, Goats will be sure to deliver a rude awakening.",
        years: "Years of the Rooster",
        years_1: "1921",
        years_2: "February 8, 1921",
        years_3:"January 27, 1922",
        years_4:"1933",
        years_5:"January 26, 1933",
        years_6:"February 13, 1934",
        years_7:"1945",
        years_8:"February 13, 1945",
        years_9:"February 1, 1946",
        years_10:"1957",
        years_11:"January 31, 1957",
        years_12:"February 17, 1958",
        years_13:"1969",
        years_14:"February 17, 1969",
        years_15:"February 15, 1970",
        years_16:"1981",
        years_17:"February 5, 1981",
        years_18:"January 24, 1982",
        years_19:"1993",
        years_20:"January 23, 1993",
        years_21: "February 9, 1994",
        years_22: "2005",
        years_23: "February 9, 2005",
        years_24: "January 28, 2006",
        years_25: "2017",
        years_26: "January 28, 2017",
        years_27: "February 15, 2018",
        years_28: "2029",
        years_29: "February 13, 2029",
        years_30: "February 2, 2030",
        overall: "Horses embody strength, independence, and an adventurous spirit, navigating life with resilience and an unwavering pursuit of freedom and excitement.",
        metal: "Metal Horses are kind-hearted, outspoken, and willing to help others. They dislike advice or criticism from others, so they may be stuck on the wrong idea for too long and end up not accomplishing much. They’re just as stubborn when it comes to love, as once married, their devotion to their partner and family will prove immovable, with Metal Horses themselves maturing into calm rationality as time goes on.",
        metal_years: "1930, 1990",
        water: "Water Horses have a self-sacrificial spirit, although they can also be impatient and emotional. They’re thoughtful and suitable for great ambition because they’ll often receive unexpected help from unlikely quarters, especially from the opposite gender. Although they’re not particularly sexy, Water Horses can easily attract attention with their cheery personality. A relationship with them will require patience from their partner, but once married, they’ll quickly grow into their true potential.",
        water_years: "1942, 2002",
        wood: "Wood Horses have a rich imagination and inspired insights. They can read others and make themselves likable, while they also tend to be impatient and overly emotional, and will need to cultivate perseverance and patience. In love, Wood Horses are popular and will remain so even after they settle down. Extramarital affairs are a real risk with Wood Horses and will likely prove detrimental to the stability of their life.",
        wood_years: "1954, 2014",
        fire: "Fire Horses are lively, passionate, and unrestrained by nature. They’re leaders who can become headstrong, well-intentioned helpers who can become condescending, and ardent lovers who can become overbearing—in summary; they’re too much of everything! But that’s also why Fire Horses will be blessed with wealth since they tend to work very hard, have great love affairs that seem destined for the book pages, and be remembered for their generosity and vitality.",
        fire_years: "1966, 2026",
        earth: "Earth Horses are optimistic and kind-hearted souls who are dedicated to their friends. They’ll never feel lonely in life, and in return, they’ll be blessed with many friends who will love them for their giving spirit. Earth Horses will have ample fortune in wealth and money, but they’re advised to save. In love, they’ll appear less attractive, but once their dense exterior is penetrated, their partner will discover a passionate lover.",
        earth_years: "1918, 1978",
        compatibility: "Horses are energetic, lively, and generous, so they will be popular with the opposite sex. When it comes to love compatibility, their hot temper and stubborn nature mean they tend to gravitate towards romantic partners who are more easygoing and gentle. They prefer to take the assertive role and enjoy the pursuit and eventual conquest of the object of their affection. Horses need freedom, so if their partner is needy or clingy, Horses may feel stifled.",
        best: "Horse and Tiger",
        best_more: "Tigers may represent characteristics that Horses dislike about themselves— they’re temperamental, hot-headed, and often cocky. But in fact, they bring out the best in each other and allow the other to grow out of their worst. It’s as if both Tiger and Horse finally have someone who can keep up with their own breakneck speed, which can be thrilling to Horse, who would have gotten bored with a less charismatic partner.",
        gender: "Female Horse and Male Tiger",
        gender_more: "This is a surprisingly good match because Tiger can provide domestic intimacy and calmness for Horse, making it easy for Horse to mature into a good wife and mother in addition to their career ambition. They’re an energetic and hardworking pair, working together to create a beautiful atmosphere at home. Although both can be temperamental, it seems Tiger and Horse understand each other well enough, which will prevent most disagreements.",
        gender_reverse: "Female Tiger and Male Horse",
        gender_reverse_more: "Although Horses tend to prefer mellower zodiac signs, with Tiger, they’re willing to make an exception because these two signs have a lot in common —seemingly, birds of the same feather end up flocking together!.  Both Tiger and Horse are energetic and ambitious, so if they find a common goal or cause, they will prove unstoppable. In each other’s company, they’ll revel in the joy of being in true communion.",
        best_2: "Horse and Dog",
        best_more_2: "Dog is practically Horse’s dream come true when it comes to romance since this spirited and high-strung zodiac has always dreamed of a mellower partner who can give them a respite from their own passionate nature. In return, Horse will take on the leadership role in the relationship—as they naturally prefer—and give their more homely partner a sense of direction and movement in life, exactly what Dog wants, too.",
        gender_2: "Female Horse and Male Dog",
        gender_more_2: "There isn’t anyone more loyal than Dog, which Horse loves in her man. This couple will support each other while intuitively leaving enough personal space for their faithful partner, giving them the space to grow. Neither will be excessively critical since both are genuinely impressed by their partner’s sincerity and ability to communicate. Horse will find Dog to be a mature partner, often giving her a new perspective in life.",
        gender_reverse_2: "Female Dog and Male Horse",
        gender_reverse_more_2: "This pair is likely to grow old together because they’re both generous and cheerful and full of vitality and love for life. They’ll start a family and build a home life that’s never short of joy. Horse is intelligent and insightful, while Dog is sincere and forgiving—a quality he’ll need. In return, Horse will value Dog’s loyalty and show her the love she’ll need to flourish in her own right.",
        best_3: "Horse and Goat",
        best_more_3: "Who else can better soothe the passionate Horse when they’re riled up than the gentle and mild Goat? A few well-chosen words and a knowing touch from their better half, and Horse will magically settle down. Many misunderstand Goat to be ambition-less, but not Horse. They know their Goat to be as hardworking—or even stubborn—as themselves when it comes to something they care about, which Horse respects and adores.",
        gender_3: "Female Horse and Male Goat",
        gender_more_3: "This is a union with an easygoing heart-to-heart connection since Goat is generally sentimental, kind, and family-oriented, while Horse is cheerful and independent. Together, these two are destined for a lifetime of happiness and fulfillment. Goat won’t hesitate to take the reins in making sure they stay intimate and close emotionally, which gives Horse a sense of a happy family while allowing them a wide berth for their independent nature.",
        gender_reverse_3: "Female Goat and Male Horse",
        gender_reverse_more_3: "This couple will fall in love and get married before long because neither will find a better match. Although Horse is fiery while Goat is mild, they share the same goals and values in life. Once they marry, this pair will spur each other on to reach their true potential because they can compensate for each other’s weaknesses while greatly appreciating their strengths. A warm and joyous union is assured.",
        worst: "Horse and Rat",
        worst_more: "Horse and Rat cannot seem to stay together for long, even if the relationship started as a loving union, because while they are agreeable and well-liked, they’re also both too headstrong to make any concessions. Horse is demanding and asks Rat to give in to their needs, while Rat will react by ignoring Horse. This leads to frequent conflicts that neither will bother to resolve, making theirs a difficult match.",
        worst_2: "Horse and Ox",
        worst_more_2: "Horse and Ox find their way to each other and may start a relationship, but soon conflicts and disputes arrive, and neither can remember why they were drawn to the other in the first place. Horse loves freedom, which makes Ox feel insecure, while Ox’s stability and steadiness bore Horse. What started quickly as a passionate love affair is more likely to result in a bitter breakup rather than a happy marriage.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        summary: "In Chinese astrology, the Goat, also known as the Sheep or Ram, is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Goat are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "Dogs are friendly, fun-loving, and fiercely loyal to their friends and family, maintaining these relationships over a lifetime of sincerity. They are also compassionate, innocent, and romantic souls who possess a strong intuition to boot. They need praise and encouragement when they exhibit their instinct to follow and protect. This makes Dogs more of a dependable team player than a strong leader, both at work and in their love life.",
        strengths: "gentleness",
        strengths_2: "creativity",
        strengths_3: "harmony",
        strengths_4: "intuition",
        strengths_5: "resilience",
        weaknesses: "indecisiveness",
        weaknesses_2: "over-sensitivity",
        weaknesses_3: "passivity",
        weaknesses_4: "over-idealization",
        weaknesses_5: "dependence on others",
        personality_2: "Their logic in life is simple, so you can always count on their actions and feelings to match their words. If they flout rules—unthinkable for their own sake—it’s to protect those they love.",
        years: "Years of the Dog",
        years_1: "1922",
        years_2: "January 28, 1922",
        years_3:"February 15, 1923",
        years_4:"1934",
        years_5:"February 14, 1934",
        years_6:"February 3, 1935",
        years_7:"1946",
        years_8:"February 2, 1946",
        years_9:"January 21, 1947",
        years_10:"1958",
        years_11:"February 18, 1958",
        years_12:"February 7, 1959",
        years_13:"1970",
        years_14:"February 6, 1970",
        years_15:"January 26, 1971",
        years_16:"1982",
        years_17:"January 25, 1982",
        years_18:"February 12, 1983",
        years_19:"1994",
        years_20:"February 10, 1994",
        years_21: "January 30, 1995",
        years_22: "2006",
        years_23: "January 29, 2006",
        years_24: "February 17, 2007",
        years_25: "2018",
        years_26: "February 16, 2018",
        years_27: "February 4, 2019",
        years_28: "2030",
        years_29: "February 3, 2030",
        years_30: "January 22, 2031",
        overall: "Honest and loyal, Dogs are the truest friends and most reliable partner.",
        metal: "Metal Horses are kind-hearted, outspoken, and willing to help others. They dislike advice or criticism from others, so they may be stuck on the wrong idea for too long and end up not accomplishing much. They’re just as stubborn when it comes to love, as once married, their devotion to their partner and family will prove immovable, with Metal Horses themselves maturing into calm rationality as time goes on.",
        metal_years: "1930, 1990",
        water: "Water Horses have a self-sacrificial spirit, although they can also be impatient and emotional. They’re thoughtful and suitable for great ambition because they’ll often receive unexpected help from unlikely quarters, especially from the opposite gender. Although they’re not particularly sexy, Water Horses can easily attract attention with their cheery personality. A relationship with them will require patience from their partner, but once married, they’ll quickly grow into their true potential.",
        water_years: "1942, 2002",
        wood: "Wood Horses have a rich imagination and inspired insights. They can read others and make themselves likable, while they also tend to be impatient and overly emotional, and will need to cultivate perseverance and patience. In love, Wood Horses are popular and will remain so even after they settle down. Extramarital affairs are a real risk with Wood Horses and will likely prove detrimental to the stability of their life.",
        wood_years: "1954, 2014",
        fire: "Fire Horses are lively, passionate, and unrestrained by nature. They’re leaders who can become headstrong, well-intentioned helpers who can become condescending, and ardent lovers who can become overbearing—in summary; they’re too much of everything! But that’s also why Fire Horses will be blessed with wealth since they tend to work very hard, have great love affairs that seem destined for the book pages, and be remembered for their generosity and vitality.",
        fire_years: "1966, 2026",
        earth: "Earth Horses are optimistic and kind-hearted souls who are dedicated to their friends. They’ll never feel lonely in life, and in return, they’ll be blessed with many friends who will love them for their giving spirit. Earth Horses will have ample fortune in wealth and money, but they’re advised to save. In love, they’ll appear less attractive, but once their dense exterior is penetrated, their partner will discover a passionate lover.",
        earth_years: "1918, 1978",
        compatibility: "Horses are energetic, lively, and generous, so they will be popular with the opposite sex. When it comes to love compatibility, their hot temper and stubborn nature mean they tend to gravitate towards romantic partners who are more easygoing and gentle. They prefer to take the assertive role and enjoy the pursuit and eventual conquest of the object of their affection. Horses need freedom, so if their partner is needy or clingy, Horses may feel stifled.",
        best: "Horse and Tiger",
        best_more: "Tigers may represent characteristics that Horses dislike about themselves— they’re temperamental, hot-headed, and often cocky. But in fact, they bring out the best in each other and allow the other to grow out of their worst. It’s as if both Tiger and Horse finally have someone who can keep up with their own breakneck speed, which can be thrilling to Horse, who would have gotten bored with a less charismatic partner.",
        gender: "Female Horse and Male Tiger",
        gender_more: "This is a surprisingly good match because Tiger can provide domestic intimacy and calmness for Horse, making it easy for Horse to mature into a good wife and mother in addition to their career ambition. They’re an energetic and hardworking pair, working together to create a beautiful atmosphere at home. Although both can be temperamental, it seems Tiger and Horse understand each other well enough, which will prevent most disagreements.",
        gender_reverse: "Female Tiger and Male Horse",
        gender_reverse_more: "Although Horses tend to prefer mellower zodiac signs, with Tiger, they’re willing to make an exception because these two signs have a lot in common —seemingly, birds of the same feather end up flocking together!.  Both Tiger and Horse are energetic and ambitious, so if they find a common goal or cause, they will prove unstoppable. In each other’s company, they’ll revel in the joy of being in true communion.",
        best_2: "Horse and Dog",
        best_more_2: "Dog is practically Horse’s dream come true when it comes to romance since this spirited and high-strung zodiac has always dreamed of a mellower partner who can give them a respite from their own passionate nature. In return, Horse will take on the leadership role in the relationship—as they naturally prefer—and give their more homely partner a sense of direction and movement in life, exactly what Dog wants, too.",
        gender_2: "Female Horse and Male Dog",
        gender_more_2: "There isn’t anyone more loyal than Dog, which Horse loves in her man. This couple will support each other while intuitively leaving enough personal space for their faithful partner, giving them the space to grow. Neither will be excessively critical since both are genuinely impressed by their partner’s sincerity and ability to communicate. Horse will find Dog to be a mature partner, often giving her a new perspective in life.",
        gender_reverse_2: "Female Dog and Male Horse",
        gender_reverse_more_2: "This pair is likely to grow old together because they’re both generous and cheerful and full of vitality and love for life. They’ll start a family and build a home life that’s never short of joy. Horse is intelligent and insightful, while Dog is sincere and forgiving—a quality he’ll need. In return, Horse will value Dog’s loyalty and show her the love she’ll need to flourish in her own right.",
        best_3: "Horse and Goat",
        best_more_3: "Who else can better soothe the passionate Horse when they’re riled up than the gentle and mild Goat? A few well-chosen words and a knowing touch from their better half, and Horse will magically settle down. Many misunderstand Goat to be ambition-less, but not Horse. They know their Goat to be as hardworking—or even stubborn—as themselves when it comes to something they care about, which Horse respects and adores.",
        gender_3: "Female Horse and Male Goat",
        gender_more_3: "This is a union with an easygoing heart-to-heart connection since Goat is generally sentimental, kind, and family-oriented, while Horse is cheerful and independent. Together, these two are destined for a lifetime of happiness and fulfillment. Goat won’t hesitate to take the reins in making sure they stay intimate and close emotionally, which gives Horse a sense of a happy family while allowing them a wide berth for their independent nature.",
        gender_reverse_3: "Female Goat and Male Horse",
        gender_reverse_more_3: "This couple will fall in love and get married before long because neither will find a better match. Although Horse is fiery while Goat is mild, they share the same goals and values in life. Once they marry, this pair will spur each other on to reach their true potential because they can compensate for each other’s weaknesses while greatly appreciating their strengths. A warm and joyous union is assured.",
        worst: "Horse and Rat",
        worst_more: "Horse and Rat cannot seem to stay together for long, even if the relationship started as a loving union, because while they are agreeable and well-liked, they’re also both too headstrong to make any concessions. Horse is demanding and asks Rat to give in to their needs, while Rat will react by ignoring Horse. This leads to frequent conflicts that neither will bother to resolve, making theirs a difficult match.",
        worst_2: "Horse and Ox",
        worst_more_2: "Horse and Ox find their way to each other and may start a relationship, but soon conflicts and disputes arrive, and neither can remember why they were drawn to the other in the first place. Horse loves freedom, which makes Ox feel insecure, while Ox’s stability and steadiness bore Horse. What started quickly as a passionate love affair is more likely to result in a bitter breakup rather than a happy marriage.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        summary: "In Chinese astrology, the Goat, also known as the Sheep or Ram, is one of the twelve animal signs representing a twelve-year cycle. People born in the Year of the Goat are believed to inherit certain personality traits and characteristics associated with this zodiac sign.",
        personality_1: "According to Chinese horoscopes, Pigs are calm and cheerful, with the ability to speak and act with tact. They possess an unusual innocence and optimism, making them appear angelic and almost childlike, leading others to show their true selves. Their joy in life won’t be sacrificed in favor of their ambition, however. Instead, they’ll aim to achieve a balanced, emotionally rich lifestyle, which is only possible for someone with their wisdom and natural talent.",
        strengths: "gentleness",
        strengths_2: "creativity",
        strengths_3: "harmony",
        strengths_4: "intuition",
        strengths_5: "resilience",
        weaknesses: "indecisiveness",
        weaknesses_2: "over-sensitivity",
        weaknesses_3: "passivity",
        weaknesses_4: "over-idealization",
        weaknesses_5: "dependence on others",
        personality_2: "Socially, Pigs are renowned for their generosity, even though they’re excellent with their money and a common symbol of wealth. If they’re cheated owing to their trusting and kind-hearted nature, Pigs may grow jaded and begin to suspect everything in life.",
        years: "Years of the Pig",
        years_1: "1923",
        years_2: "February 16, 1923",
        years_3:"February 4, 1924",
        years_4:"1935",
        years_5:"February 4, 1935",
        years_6:"January 23, 1936",
        years_7:"1947",
        years_8:"January 22, 1947",
        years_9:"February 9, 1948",
        years_10:"1959",
        years_11:"February 8, 1959",
        years_12:"January 27, 1960",
        years_13:"1971",
        years_14:"January 27, 1971",
        years_15:"February 24, 1972",
        years_16:"1983",
        years_17:"February 13, 1983",
        years_18:"February 1, 1984",
        years_19:"1995",
        years_20:"January 31, 1995",
        years_21: "February 18, 1996",
        years_22: "2007",
        years_23: "February 18, 2007",
        years_24: "February 6, 2008",
        years_25: "2019",
        years_26: "February 5, 2019",
        years_27: "January 24, 2020",
        years_28: "2031",
        years_29: "January 23, 2031",
        years_30: "February 10, 2032",
        overall: "Pigs have a beautiful personality and are blessed with good fortune in life.",
        metal: "Metal Pigs are conscientious and well-informed people who take good care of their friends and family and always seem willing to lend a helpful hand. They may tend to be a little lazy by nature. They’ll express their feelings directly and honestly soon after meeting someone, but Metal Pigs’ effusiveness shouldn’t be taken for flightiness, as their words are backed by a genuine intention to shower that person with love.",
        metal_years: "1911, 1971",
        water: "Water Pigs can be quite stubborn. Once they decide on something, others’ opinions or criticisms will fall by the wayside because they’ll decide to proceed anyway, even if they may live to regret earlier decisions. They can’t seem to achieve a balance in their romantic relationships, and they go from stubborn to yielding, depending on the kind of partner they end up with, and never seem to find a happy medium.",
        water_years: "1923, 1983",
        wood: "Wood Pigs appear simple-minded and almost adorably naive, but that appearance conceals a perseverance that won’t be overwhelmed by setbacks. Aside from that, Wood Pigs are indeed as innocent and happy-go-lucky as they appear. They won’t demand extraordinary beauty in their partner, preferring instead a deeper relationship built on mutual trust. Therefore, they tend to take their time in courtship and allow the relationship to take its natural course.",
        wood_years: "1935, 1995",
        fire: "Fire Pigs prefer cooperative work because they seem to lack firm personal opinions when it comes to most subjects. They love being with friends and will gladly absorb opinions and guidance extended from their friends. They’re not the most adroit in love, but Fire Pigs have one thing on their side—perseverance, which means working steadily to win over the object of their affections with their steadfast affection and devotion.",
        fire_years: "1947, 2007",
        earth: "Unlike most Earth zodiac signs, Earth Pigs are popular to the point of being social butterflies. They’re good-natured and excel at keeping many friends of various types and intimacy in their hearts without trouble. By contrast, they aren’t exactly masters at love, even if Earth Pigs offer the same sincerity to potential partners that they do to new friends. This vulnerability is touching and attractive to the right person.",
        earth_years: "1959, 2019",
        compatibility: "Pigs like to pursue contentment and enjoyment in life, which applies to their love life as well, preferring signs with the same gentle and easy-going temperament, although some would gravitate towards a more dominant partner. For these romantic souls, love is hoped to last for a lifetime. Indeed, when they find love compatibility with the right partner, Pigs are likely to remain loyally in love with the same person for the rest of their life.",
        best: "Pig and Rabbit",
        best_more: "Rabbit is known for being a little jumpy, which Pig’s gravitas practically cures— at least enough so that Rabbit has the emotional bandwidth to work on themselves. So it’s a rather healing attraction for Rabbits. For Pig, on the other hand, Rabbit brings such sweet pleasure and joys to Pig’s day that it enhances the latter’s immersion in life—hardly a tough choice for someone who revels in beauty and joy.",
        gender: "Female Pig and Male Rabbit",
        gender_more: "Rabbit is humorous, bringing the more withdrawn Pig out of her shell. This pair will live together in a light-hearted yet deeply felt way as a result, and each will be an emotional rock for the other. Rabbit’s affections can wane quickly, especially in day-to-day life, but with Pig, this won’t be an issue as this woman’s gentle and forgiving affections will be enough to envelope Rabbit in a cocoon of happiness.",
        gender_reverse: "Female Rabbit and Male Pig",
        gender_reverse_more: "Rabbit loves her Pig man, who’s knowledgeable, wise, and gentle. Pig may initially be reluctant to act on his feelings—Rabbit’s elegance seems out of reach—but Rabbit will offer Pig plenty of heartfelt encouragement. Their personalities will complement each other as both grow, with Rabbit encouraging Pig to act more assertively at work, while Pig’s silent but lasting love will nurture a sense of security in his nervous partner.",
        best_2: "Pig and Goat",
        best_more_2: "There’s nothing to worry about when two gentle and easygoing signs like Pig and Goat come together. They’ll hardly ever exchange a harsh word with each other, in fact, which isn’t exactly easy to find. Beneath their soft exteriors, Pig’s sharp intellect and Goat’s shrewd analytical skill ensure that their life will not only be easy but prosperous as well. It’s the ordinary sort of happiness these signs will share.",
        gender_2: "Female Pig and Male Goat",
        gender_more_2: "Pig can be sensitive and easily wounded in a relationship and may be hurt by men of other zodiac signs in unexpected ways, but that won’t happen with her Goat because he’s very sensitive himself. This relationship will be characterized by both partners constantly wanting the best for the other’s well-being. They’ll appreciate the effort the other has invested into the relationship and feel the depth of their long-lasting love.",
        gender_reverse_2: "Female Goat and Male Pig",
        gender_reverse_more_2: "Goat is rarely a leader, except in emotional matters where she may become a guiding light for her Pig man because nothing in Pig’s wealth of knowledge has taught them how to express their feelings. Until they meet Goat, that is. With her gentle prodding, Pig will express his rich feelings and surprising humor like he’s never felt possible before. They’ll have such fun built upon steadfast love and support.",
        best_3: "Pig and Tiger",
        best_more_3: "Tiger seems an unlikely choice for Pig, who doesn’t like to try too hard in life, which is unthinkable for Tiger. But in fact, both need some reminder of their polar opposite to truly thrive. Tiger’s ambition and drive remind Pig that there’s more in life than a good time, and they shouldn’t sell themselves short, while Pig’s laidback attitude reminds Tiger to take a breather and smell the roses.",
        gender_3: "Female Pig and Male Tiger",
        gender_more_3: "Most assertive men will scare Pig off, but Tiger’s charisma is just the right kind for Pig. She loves taking care of him and will end each day by preparing his favorite dishes for him. Tiger can be prideful at times, but Pig’s his perfect mate. The effort Pig invests in the relationship will never go unnoticed by Tiger, which is all Pig will ask in return for her love.",
        gender_reverse_3: "Female Tiger and Male Pig",
        gender_reverse_more_3: "This pair is a surprisingly good fit. Tiger can seem aggressive to many, but Pig will somehow disarm all her sharp edges with his shy yet steady affections, allowing him to finally hug her close. With his thirst for knowledge, Pig will appreciate Tiger’s intellect more than so-called traditional feminine qualities. In addition, being the natural provider that he is, Pig will give all the affection his demanding lover desires.",
        worst: "Pig and Snake",
        worst_more: "This will be a chaotic pair if they get married. Both Pig and Snake seem to find some aspect of their partner’s personality too different from their own, and as such, will always disagree, quarrel, fight, and divorce. Such a discordant relationship will lead to poor fortune for both since the one place both need to feel comfortable and recharge, the home, is the one place neither can do so in this marriage.",
        worst_2: "Pig and Monkey",
        worst_more_2: "This is a damaging aspect for both zodiac signs, but they seem to strike gold after they marry, which leads them to stay together. They’ll soon discover that they can’t be themselves around their partner. Monkey will become unscrupulous in reaching their goals in this relationship, which will soon make Monkey and Pig a couple that looks enviable and successful on the outside—but miserable and inauthentic on the inside.",
        lucky_1: "1, 5, 6",
        lucky_2: "Brown, Black, Gray",
        lucky_3: "North, Northwest",
        lucky_4: "Sunflower, Jasmine",
        lucky_5: "March, April, May, July",
        lucky_6: "Topaz, Aquamarine",
        lucky_7: "Horse figurines or ornaments",
        unlucky_1: "1, 6, 7",
        unlucky_2: "White, Gold",
        unlucky_3: "West, Northwest",
        unlucky_4: "February, April, August, September",
        unlucky_5: "Garnet",
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
        birth_more_9: "American actress known for her role in \"Bridget Jones's Diary\".",
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
.r svg{
padding-right: 30px;
}
.r p{
padding-left: 30px;
padding-right: 10px;
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);   
}
.rs {
background-color: rgb(161, 41, 41);
outline: 10px double rgb(26, 15, 33);
width: 80%;
}
.rp{
font-size: 100px;
float: left;
}
.rp svg::selection{
    color: rgb(194, 181, 178);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.pers p {
    padding: 1px 30px;
    color: rgb(26, 15, 33);
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
border: 3px solid rgb(194, 181, 178);
padding: 3px;
padding-left: 10px;
padding-right: 10px;
border-radius: 10px;
}
.pers p::selection {
    color: rgb(194, 181, 178);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.perr table {
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;    
    border: 2px solid rgb(26, 15, 33);
    border-collapse: collapse;
}
.perr th {
    border: 1px solid rgb(26, 15, 33);
    text-align: left;
    padding: 8px;    
    color: rgb(26, 15, 33);
    }
.perr td {
    border: 1px solid rgb(26, 15, 33);
    text-align: left;
    padding: 8px;    
    color: rgb(26, 15, 33);
}
.perr td:hover{
        background-color:rgb(75, 12, 12); 
        color: rgb(238, 228, 169);   
}    

.perr td::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
    }
.perr th::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.person {
    display: flex; 
    justify-content: space-between;
    gap: 20px; 
    padding: 20px; 
    background-color: rgb(238, 228, 169); 
    }
.perso h2{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    height: 50px;
    color: rgb(75, 12, 12);
    }
.perso h2::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
    }    
.person p{
    padding: 1px 30px;
    color: rgb(26, 15, 33);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;   
    text-align: center;
    flex-direction: row-reverse;
    }
.person p::selection{
        color: rgb(194, 181, 178);
        background: rgb(75, 12, 12);    
    }    
.perso li {
    padding: 1px 30px;
    color: rgb(75, 12, 12);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.perso p {
    align-items: flex-start;  
   }
.perso p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}   
.perso{
    display: flex;
    flex-direction: column;  
    width: 300px;
    text-align: center;
    background-color: rgb(194, 181, 178);     
    }
.persona p{
    padding: 1px 30px;
    color: rgb(26, 15, 33);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
    text-align: justify;
}
.persona p::selection{
    color: rgb(194, 181, 178);
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
color: rgb(26, 15, 33);
}
.sum {
background-image: url(https://i.pinimg.com/564x/29/cc/06/29cc0670039ecfcf49a96ed26e800dde.jpg);    
border-bottom: 30px double rgb(238, 228, 169);
border-top: 30px double rgb(238, 228, 169);  
}
.sum p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.five {
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(75, 12, 12); 
    letter-spacing: 1px;
    justify-content: center;   
    padding-top: 80px;
}
.five::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.elements{
display: flex;    
flex-direction: row;
justify-content: space-around;
}
.earth h2::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.earth h4::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.dropdown {
padding-left: 70px;
padding-right: 80px;  
}
  
.dropdown-content {
    display: none;
    background-color: rgb(194, 181, 178);
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    padding: 20px;
    z-index: 1;
    opacity: 0;
    transition-duration: 2s;
  }
.dropdown-content p{ 
    color: rgb(26, 15, 33);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    text-align: justify;
    padding-right: 20px;
    padding-left: 20px;
} 
.dropdown-content p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.dropdown:hover .dropdown-content {
    display: block;
    justify-content: baseline;
    opacity: 1;
}


.dropdown span {
    border-radius: 25px;
    background: rgb(161, 41, 41);
}
.dropdown span::selection{
    color: rgb(194, 181, 178);
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
color: rgb(75, 12, 12);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.comp h2::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.comp p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.comp p{
    color: rgb(26, 15, 33);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.compa {
padding: 30px;    
border-left: 10px double rgb(26, 15, 33);   
}
.compa p{
display: flex;
flex-wrap: wrap;
color: rgb(26, 15, 33);
font-size: larger;
line-height: 30px;
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
letter-spacing: 1px; 
text-align: justify;
}
.compa p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.com h3::selection{
    color: rgb(194, 181, 178);
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
background-color: rgb(75, 12, 12);
text-align: center;
}
.kw h2::selection{
    color: rgb(194, 181, 178);
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
    background-color: rgb(238, 228, 169);
    border-radius: 10px;
    border: 3px solid rgb(26, 15, 33); 
}
.gender h2::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.gender h2{
    color: rgb(194, 181, 178);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
}
.gender span::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.gender span{
    border-radius: 25px;
    background: rgb(194, 181, 178);
}
.g-content {
        display: none;
        background-color: rgb(161, 41, 41);
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        padding: 20px;
        z-index: 1;
        
}
#toggle:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle {
    display:none;
}
#toggle2:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle2 {
    display:none;
}
#toggle3:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle3 {
    display:none;
}
#toggle4:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle4 {
    display:none;
}
#toggle5:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle5 {
    display:none;
}
#toggle6:checked + label + .g-content {
    display: block; /* Show content when checkbox is checked */
}
#toggle6 {
    display:none;
}
.g-content p::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.g-content p{ 
        color: rgb(238, 228, 169);
        font-size: larger;
        line-height: 30px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        letter-spacing: 1px; 
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
    background: rgb(194, 181, 178);
    color: rgb(75, 12, 12);    
}
.lucky h2{
    display: flex;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(194, 181, 178); 
    letter-spacing: 1px;
    justify-content: center;
}
.u {
display: flex; 
flex-direction: row;  
justify-content: space-evenly;
}
.things li::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.things h4::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.things h2::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.things li::marker{
    color: rgb(161, 41, 41);
    font-size: 23px;   
}
.things {
    background-color: rgb(194, 181, 178);
    border-radius: 20px;
    padding: 20px;
    width: 40%;
    color:rgb(26, 15, 33);
    font-size: larger;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;
}
.things p::selection{
    color: rgb(194, 181, 178);
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
    color: rgb(26, 15, 33); 
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
    background-color: rgb(238, 228, 169);
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
    color:rgb(26, 15, 33);
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
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.out p{
    color: rgb(26, 15, 33);
    font-size: x-large;
    line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px;    
    font-variant: small-caps;
    text-align: center;
    border-bottom: 10px double rgb(75, 12, 12);
    border-top: 10px double rgb(75, 12, 12);
    padding: 30px;
    background-color: rgb(194, 181, 178);
    font-weight: bold;
}
.out a::selection{
    color: rgb(194, 181, 178);
    background: rgb(75, 12, 12);    
}
.out a{
color: rgb(161, 41, 41); 
}
.out a:hover{
    color:rgb(75, 12, 12);
}

</style>
