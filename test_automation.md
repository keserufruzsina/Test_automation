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


### Szoftverfejlesztési és tesztelési modellek(vízesés, V-modell, agilis modell):
#### Vízesés modell:
A vízesésmodell a projekt tevékenységeinek sorozatos lineáris szakaszokra bontása, ahol az egyes szakaszok az előző fázis eredményeitől függnek, és az adott feladat specializációjának felelnek meg.
szoftverfejlesztésben inkább a kevésbé iteratív és rugalmatlan megközelítések közé tartozik

<img src="https://centroszet.hu/tananyag/szervezes2/image003.jpg" alt="image" width="450" height="220">

#### V-modell:
A szoftverfejlesztés során a V modell olyan fejlesztési folyamatot képvisel, amelyet a vízesésmodell kiterjesztésének tekinthetünk, és egy esete az általános V modellnek. A V modell a nevét onnan kapta, hogy két szára van, és így egy V betűhöz hasonlít. A modell ábrája a fejlesztés két folyamatának két megközelítését tükrözi, bemutatja a kapcsolatokat a fejlesztési életciklus egyes szakaszai és a kapcsolódó tesztelési szakaszok között. Top-down megközelítésként kifejezi a tervezési folyamat fentről lefelé történő haladását a diagram bal oldali ágában, míg bottom-up megközelítésben a jobb oldali ágban a tesztelési folyamat lentről felfelé halad. A vízszintes és a függőleges tengely az időt vagy a projekt teljességét (balról jobbra) és az absztrakció szintjét jelöli.

<img src="https://szit.hu/lib/exe/fetch.php?media=oktatas:programozas:v-modell_uj.png" alt="image" width="450" height="300">

####  Agilis modell:
Az agilis tesztelés akkor kezdődik, amikor a projekt fejlesztése megkezdődik. Röviden, a tesztelést és a fejlesztést minden szakaszban integrálja. A legtöbb fejlesztő az agilis tesztelési piramisra hivatkozva gondol erre a folyamatra (erről később).
Az agilis módszertan alkalmazása a tesztelésben azt jelenti, hogy a tesztelés a fejlesztési folyamat során folyamatosan történik, és szinte minden szakaszban bevonja a fejlesztőket, a tesztelőket és a tulajdonosokat.

<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" alt="image" width="450" height="300">

### TDD modell
A tesztvezérelt fejlesztés (Test-driven development, TDD) egy szoftverfejlesztési folyamat, ami egy nagyon rövid fejlesztési ciklus ismételgetésén alapul, tehát a követelményeket speciális teszt esetekként fogalmazzuk meg, a kódot pedig ehhez mérten írjuk meg, így az át fog menni a teszten. Ez tökéletes ellentéte a hagyományos szoftverfejlesztésnek, ami megengedi olyan kódrészletek meglétét is, amelyek nem felelnek meg teljesen a követelményeknek. A TDD összefüggésben áll az extrém programozás koncepciójával, miszerint először teszteljünk és ha minél többet tesztelünk, annál több hibát tudunk kiküszöbölni a kódban.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0b/TDD_Global_Lifecycle.png/1920px-TDD_Global_Lifecycle.png" alt="image" width="300" height="220">
<img src="https://cdn.codegym.cc/images/article/9d5eca2d-4750-4470-83bc-9d0147b2d611/512.jpeg" alt="image" width="300" height="220">

### BDD modell
A viselkedésvezérelt fejlesztés (behavior-driven development, BDD) egy agilis szoftverfejlesztési folyamat, amely ösztönzi az együttműködést a fejlesztők, a QA és a nem műszaki vagy üzleti résztvevők között egy szoftverkészítő projektben. Arra ösztönzi a csapatokat, hogy beszélgetéssel és konkrét példákkal hivatalossá tegyék az alkalmazás működésének közös megértését. A tesztvezérelt fejlesztésből (TDD) alakult ki. A viselkedésvezérelt fejlesztés ötvözi a TDD általános technikáit és elveit a tartományvezérelt tervezés és objektumorientált elemzés és tervezés ötleteivel, hogy a szoftverfejlesztő és -kezelő csapatok számára megosztott eszközöket és közös folyamatot biztosítson a szoftverfejlesztésben való együttműködéshez.

