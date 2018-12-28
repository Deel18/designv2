Kmom05 - Laddningstider
========================
Uppgiften går ut på att analysera olika hemsidors laddningstider.

Urval

Jag valde att använda liknande sidor från förra analysen. Jag fick byta ut Jamie Olivers hemsida då den vägrade öppna när jag försökte nå webbplatsen. Jag valde att gå med dessa tre olika webbplatser då jag ville se hur stor skillnaden är mellan hemsidor som prioriterar olika saker.

Metod

Jag använde mig av Pagespeed Insights för att först notera ett betyg för varje hemsida. Sedan skapade jag ett kalkylark där jag skrev ner resultaten av testen. Jag mätte sidornas laddningstider genom att använda mig av Google Devtools - Networks. För snapshots så använde jag mig av Windows inbyggda Snippingtool.

[Kalkylark](https://docs.google.com/spreadsheets/d/10-e5G3dlsti3PSoE45IJUVsCtWOpCSEJQuojBCXm8oc/edit?usp=sharing)


Resultat

**Royal London**

Royal London fick 27 poäng i mobilt och 97 med Desktop enligt Pagespeed analysen. Det tog ungefär 6 sekunder för att få hela sidan laddad. Hemsidan använder inte många bilder men den verkar ändå skicka ut en hel del requests med 63 stycken. Datan som skickas ligger i genomsnitt på 1.8 mb.


[FIGURE src="../htdocs/img/123.PNG" class="royalLondon"]

Det jag märker av mest är hur lång tid det tar för footern i hemsidan att visa sig, det vill säga Cookie policyn. Sidan hade kunnat förbättras genom att minifiera CSS samt skjuta upp CSS kod som inte används. Det hade kunnat förbättra hemsidans laddningstid med upp till 4 sekunder i mobilt läge. Det verkar även som att hemsidan upprepar omdirigeringar väldigt mycket, då det hade kunnat förbättras med 1,26 s om man hade löst problemet. En annan sak som jag har märkt är att i responsivt läge så verkar den endast ändra layouten för hemsidan, vilket med all förmodan minskar hastigheten för mobila enheter och kan bidra till dess dåliga betyg inom Mobile kategorin. En lösning hade varit att designa hemsidan efter olika enheter och sedan ladda in designen till respektive enhet.


**Gordon Ramsay**

Webbplatsen fick 28 för mobile och 92 för desktop. Då själva hemsidan förlitar sig väldigt mycket på bilder så är det förväntat att laddningstiderna blir större. Det tar i genomsnitt 13,2 s för att ladda in hemsidan helt och den överför 3.1 mb.

[FIGURE src="../htdocs/img/1234.PNG" class="royalLondon"]

Det som verkar bidra mest till det dåliga betyget för mobilt läge är att bilderna skickas med gamla bildformat, då hemsidan hade förbättrats med 3,9 s om man hade skickat bilder i modernare format. I Desktop mode så hade hemsidan också gynnats av att skicka bilderna i ett modernare format samt använda bilder av rätt storlek. Det verkar finnas mycket som kan förbättras genom att börja använda bilder på "rätt" eller ett bättre sätt.

**Leetcode**

Leetcode fick 3 för Mobile och 76 för Desktop. Hemsidan är väldigt enkel så jag är förvånad över att den behöver i genomsnitt 3,8 s för att ladda in helt. Jag skulle tänka mig att det beror på att bilderna tar stor plats då hemsidan skickar i snitt 2 mb av data.

[FIGURE src="../htdocs/img/leetcode1.PNG" class="royalLondon"]

Det som hade kunnat förbättra upplevelsen på mobila enheter är att ta bort resurser som blockerar renderingen samt minifiera Javascript koden som körs. Det hade minskat laddningstiden upp till 4 sekunder. För Desktop så hade det minskat med 2 sekunder respektivt.


Analys

Jag tycker att laddningstider mellan 1-2 sekunder är bra och att allting över 7 sekunder är långsamt. Ingen av hemsidorna hade klarat sig igenom enligt mitt gränsvärde, däremot bör man tänka på att när man själv använder sidorna så tänker/märker man inte av att det tar + 3 sekunder att ladda en sida. Däremot, eftersom jag suttit och testat tiderna så har jag upplevt det som väldigt långsamt.

Den klara vinnaren är Leetcode i det här scenariot. Däremot beror det också på att den hemsidan använder sig inte av lika mycket bilder. Generellt sätt verkar inte företagen fokusera så mycket på att optimisera sidorna för mobila enheter då alla tre fick lågt betyg inom den kategorin.

Det beror mycket på vad för slags hemsida man försöker skapa för sin klient tycker jag. Royal London har en sida som ska ge information och leda användaren vidare, då bör man fokusera på att minska fördröjningar för det innehållet. Om man ska marknadsföra någon som Gordon Ramsay som är känd för sin mat så kan man förvänta sig att sidan kommer använda sig av många bilder, vilket innebär att mycket data kommer att skickas. Då bör man fokusera på att minska fördröjningar inom det området.

Det mest gemensamma temat för förbättring av laddningstider verkar vara relaterat till hur man hanterar bilder. Lyckas man hantera det på rätt sätt så kan det drastiskt minska laddningstiden.


Referenser


Övrigt
Rapporten genomfördes enskilt av mig, DEEL18.
