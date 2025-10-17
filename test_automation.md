# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

## A tesztelés alapjai:
#### Mi a tesztelés célja? Mi nem az?
 A tesztelés elsődleges célja, hogy a fejlesztés során minél korábban felfedezze a hibákat, így csökkentve azok javításának költségeit. Nem tartozik a teszteléshez a program részeinek összeépítése, vagyis maga a fejlesztési folyamat.
 https://hu.wikipedia.org/wiki/Szoftvertesztel%C3%A9s





#### Mi a kapcsolat a tesztelés és a hibamegelőzés között?
Minél korábban derül fény egy hibára a fejlesztés során, annál kisebb ráfordítással lehet azt kijavítani, ezért a tesztelés hatékony eszköz a hibák megelőzésében és kezelésében.
 https://hu.wikipedia.org/wiki/Szoftvertesztel%C3%A9s





#### Miért fontos, hogy a tesztelők függetlenek legyenek a fejlesztőktől?
 A tesztelők és a fejlesztők külön szakmai területet képviselnek, eltérő tudással. A tesztelőknek átfogóan ismerniük kell a projekt üzleti oldalát is, így független szemlélettel tudják értékelni a szoftvert, nem befolyásolva az eredményeket a fejlesztők szempontjai szerint.
 https://www.jtechlog.hu/2022/08/20/fejlesztok-es-tesztelok.html





#### Mi a veszélye annak, ha a fejlesztő maga teszteli a saját kódját?
 A fejlesztő belső nézőpontja miatt nem biztos, hogy észreveszi azokat a hibákat, amelyeket egy független, új felhasználó könnyebben felfedezne. Emellett a fejlesztők nem mindig rendelkeznek a megfelelő tesztelési módszertani ismeretekkel.
 https://www.jtechlog.hu/2022/08/20/fejlesztok-es-tesztelok.html






#### Mik a tesztelési alapelvek?
A tesztelés azt jelzi, hogy hibák vannak, de nem bizonyítja a hiányukat. Nem lehet minden lehetséges esetet letesztelni, ezért a tesztelést minél korábban kell elkezdeni. A hibák hajlamosak egyes területeken összpontosulni, ezért célzott tesztelés szükséges. A tesztelés eredménye nagyban függ a körülményektől, és a hibátlan rendszer illúziója veszélyes.
https://teveli.info/index.php/teszteles/01-alapok/05-szoftvertesztelesi-alapelvek





#### Mit jelent az „alapvető tesztelési elv”, hogy „a kimerítő tesztelés lehetetlen”?
Nem lehet minden bemeneti variációt teljesen lefedni, mivel a lehetséges kombinációk száma rendkívül nagy (például egy 10 karakterből álló bemenetnél 256^10 lehetőség van). Ezért a tesztelés során főként a legkritikusabb, legkockázatosabb részekre koncentrálunk.
https://teveli.info/index.php/teszteles/01-alapok/05-szoftvertesztelesi-alapelvek





#### Mit jelent az „alapvető tesztelési elv”, hogy „a hibák halmozódnak”?
Mivel a rendelkezésre álló tesztelési idő korlátozott, ezért a tesztelés fókuszát a leginkább hibára hajlamos modulokra és bemenetekre helyezzük, például a szélsőértékekre, ahol nagyobb eséllyel fordulnak elő problémák.
https://teveli.info/index.php/teszteles/01-alapok/05-szoftvertesztelesi-alapelvek




#### Mit jelent az „alapvető tesztelési elv”, hogy „a tesztelés a kontextustól függ”?
A tesztelési módszerek és mélység változhatnak a projekt jellegétől és körülményeitől függően. Másképp vizsgálunk egy atomerőmű szoftvert, és máshogy egy egyszerű beadandót, illetve számít az is, hogy mennyi idő áll rendelkezésre a tesztelésre.
https://teveli.info/index.php/teszteles/01-alapok/05-szoftvertesztelesi-alapelvek



## 2. Tesztelés a szoftverfejlesztés életciklusán át
#### Mik a tesztszintek, és mi a különbség köztük?
Unit teszt: Itt a fejlesztés alatt álló alkalmazás legkisebb egységeit vizsgáljuk. Célja, hogy stabil alapot biztosítson a további fejlesztésekhez és összetevők felépítéséhez.
Modul (integrációs) teszt: Amikor az alkalmazás különálló részei modulokká állnak össze, a tesztelők ezeket az összekapcsolt kódrészeket tesztelik, hogy megbizonyosodjanak azok helyes együttműködéséről.
Rendszerteszt: Ekkor már elérhető az alkalmazás felhasználói felülete (GUI) és bizonyos funkciók működnek. A tesztelők dokumentáció alapján teszteseteket készítenek, ütemeznek és végrehajtanak, hogy ellenőrizzék a specifikációnak való megfelelést.
Elfogadási teszt: Ez a tesztelési szint a végfelhasználó számára segít eldönteni, hogy elfogadja-e az újonnan szállított terméket. Az ideális esetben a tesztesetek kidolgozása és elfogadása közösen történik a megrendelő és a szállító részéről.
https://tesztelesagyakorlatban.hu/a-tesztelesi-szintek/



#### Miért nem érdemes mindig ugyanazokat a teszteseteket futtatni (regressziós torzítás)?
Ha mindig ugyanazokat a teszteket futtatjuk, előfordulhat, hogy új hibákat nem találunk meg, mert a tesztesetek nem fedik le a változtatások teljes spektrumát.
https://tesztelesagyakorlatban.hu/hogyan-javitsd-a-regresszios-teszteleseid-eredmenyesseget-30-kal/






#### Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Egységtesztelés a program egy-egy kis egységének tesztelése. A fejlesztők általában felelősek az egységtesztek írásáért.
https://learn.microsoft.com/hu-hu/dotnet/architecture/maui/unit-testing





#### Mi a különbség a verifikáció és a validáció között?
Verifikáció és validáció: Az MI modell teljesítményének és megbízhatóságának értékelése és ellenőrzése különböző adathalmazokon vagy környezetekben. A verifikáció és validáció fontos lépései az MI modell fejlesztési folyamatának. A verifikáció a modell implementációjának és implementációs folyamatának ellenőrzését jelenti annak érdekében, hogy biztosítsák a helyes működést és a specifikációknak való megfelelést. 
https://siteland.hu/2023/07/11/verifikacio-es-validacio/




#### Mik a tesztelési típusok, és mi a különbség köztük?
Funkcionális tesztelés: a funkciók helyességét vizsgálja.
 Nem-funkcionális tesztelés: teljesítmény, használhatóság, biztonság stb. vizsgálata.
https://www.guru99.com/types-of-software-testing.html






#### Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
A szürke dobozos tesztelés a tesztelés olyan formája, amely a fehérdobozos és a fekete dobozos tesztelést ötvözi, felhasználva a mögöttes tervezés és a rendszer megvalósítási módjának részleges megértését.Ez a kombináció azt jelenti, hogy a tesztelő a háttérben zajló folyamatok egy részét ismeri anélkül, hogy teljes mértékben ismerné a kódot, ami nagyobb rálátást biztosít a szoftverben felmerülő problémák lehetséges okaira, amikor azok felmerülnek.
Az egyik leggyakoribb módszer, amelyet a vállalatok tesztelésre használnak, a fekete dobozos tesztelés, egy olyan technika, amely távolságot teremt a fejlesztők és a tesztelők között a pontos eredmények biztosítása és az elfogultság kiküszöbölése érdekében.
A fehérdobozos teszt (más néven tiszta dobozos teszt, üvegdobozteszt, átlátszódobozteszt és strukturális teszt) egy olyan szoftveres tesztelési módszer, amely az alkalmazás belső struktúráit vagy működését teszteli, szemben annak funkcionalitásával (azaz a feketedobozos teszteléssel). A fehérdobozos tesztelés során a rendszer belső perspektíváját, valamint a programozási készségeket használják a tesztesetek megtervezéséhez
https://hu.wikipedia.org/wiki/Feh%C3%A9rdobozos_tesztel%C3%A9s
https://www.zaptest.com/hu/szurke-doboz-teszteles-mely-merules-a-mi-ez-tipusok-folyamat-megkozelitesek-eszkozok-es-tobb
https://www.zaptest.com/hu/fekete-doboz-teszteles-mi-az-tipusok-folyamat-megkozelitesek-eszkozok-es-meg-sok-mas





#### Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
A rendszertesztelés a szoftvertesztelés egy olyan típusa, amely a rendszer egészének ellenőrzését végzi.Ez magában foglalja az Ön által kifejlesztett szoftver minden egyes moduljának és komponensének integrálását, hogy tesztelje, hogy a rendszer az elvárásoknak megfelelően működik-e együtt.
A fejlesztési folyamat során kritikus fontosságú annak biztosítása, hogy a szoftver a kiadás előtt az elvárásoknak megfelelően működjön. Ehhez rendkívül alapos tesztelési folyamatokon kell keresztülmennie a teljes fejlesztési időszak alatt, beleértve annak biztosítását, hogy a termék megfelelő legyen a felhasználó számára.
https://www.zaptest.com/hu/uat-teszteles-mely-merules-a-felhasznaloi-elfogadas-jelentesebe-tipusok-folyamatok-megkozelitesek-eszkozok-es-meg-sok-mas
https://www.zaptest.com/hu/mi-az-a-rendszerteszteles-melyre-merules-a-megkozelitesek-tipusok-eszkozok-tippek-es-trukkok-es-meg-sok-mas





#### Mi a különbség a statikus és dinamikus tesztelés között?
A dinamikus tesztelés a szoftvertesztelésben egy értékes szoftvertesztelési technika, amely magában foglalja az alkalmazás forráskódjának végrehajtását és annak megfigyelését, hogy az hogyan viselkedik futás közben.
A statikus tesztelés egy széles körben használt szoftvertesztelési technika, amely a kód végrehajtása nélkül keresi a szoftver hibáit. A hibák korai felismerésének részét képezi, és jellemzően a szoftverfejlesztési életciklus (SDLC) korai szakaszában történik.
https://www.zaptest.com/hu/statikus-teszteles-a-szoftvertesztelesben-mi-az-tipusok-folyamat-megkozelitesek-eszkozok-es-meg-sok-mas
https://www.zaptest.com/hu/dinamikus-teszteles-a-szoftvertesztelesben-mi-az-tipusok-folyamat-megkozelitesek-eszkozok-es-meg-sok-mas