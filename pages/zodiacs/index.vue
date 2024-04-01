<template>
    <PageHeader></PageHeader>
    <ZodiacHeader></ZodiacHeader>
    
    <main>
        <div class="zs">
            <p>
            How to know which zodiac sign are you?
            </p> 
        </div>
        <div class="zs2">
            <p>
                Your birth year determines your Chinese zodiac sign, but it can get tricky, as the lunar calendar varies from the solar, or Gregorian, calendar.
                Because the dates of Chinese New Year change every year, individuals born in January or February will need to pay special attention to their birth date in addition to their birth year.    
            </p>    
        </div>           
    </main>
</template>

<style>
.zs p {
    display: flex;
    justify-content: center;
    font-size: xxx-large;  
    font-family: fantasy;
    color: rgb(161, 41, 41);
    padding-right: 30px;
    padding-top: 30px;  
    letter-spacing: 1px;  
}

.zs p::selection {
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}

.zs2 p {
    padding: 1px 30px;
    color: rgb(238, 228, 169);
    text-align: justify;
    font-size: larger;
    Line-height: 30px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    letter-spacing: 1px; 
    padding-bottom: 30px;  
    border-bottom: 10px double rgb(212, 198, 119);  
}

.zs2::selection {
    color: rgb(143, 143, 143);
    background: rgb(75, 12, 12);    
}
</style>

<script>

</script>
