# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?

            MI a célja: Hibák felfedezése: A tesztelés segít a fejlesztés során felmerülő hibák, problémák és hiányosságok felismerésében.
                        Minőség biztosítása: A tesztelés célja, hogy a termék minősége megfeleljen a kívánt normáknak, és kielégítse a felhasználói igényeket.
                        Követelmények validálása: A tesztelés segít biztosítani, hogy a szoftver valóban azt a funkcionalitást nyújtsa, amit a felhasználók vagy a megrendelők elvárnak.
                        Rendszer integritásának ellenőrzése: Tesztelés során ellenőrizzük, hogy az egyes komponensek megfelelően működnek együtt, és a rendszer egésze is stabil marad.
                        Működési megbízhatóság biztosítása: A tesztelés célja annak biztosítása, hogy a szoftver hosszú távon is megbízhatóan működjön, különböző környezetekben és feltételek mellett.

#### ✅ Mik a tesztelési alapelvek?

            Mi nem a célja:A fejlesztés helyettesítése: A tesztelés nem arra való, hogy helyettesítse a fejlesztési folyamatot. A tesztelés a fejlesztési ciklus egy utólagos   fázisa, amelynek célja a már kifejlesztett szoftver minőségének ellenőrzése, nem pedig annak kifejlesztése.
                            Teljes körű hibamentesség garantálása: Még a legjobb tesztelés sem képes teljes mértékben garantálni, hogy a rendszer minden lehetséges hibától mentes lesz, hiszen mindig előfordulhatnak nem várt helyzetek, amelyek nem kerültek tesztelésre.
                            Felhasználói igények előrejelzése: Bár a tesztelés segíthet a funkciók helyességének ellenőrzésében, nem helyettesíti a felhasználói visszajelzések gyűjtését és az igények pontos megértését.
                            A rendszer teljesítményének optimalizálása: A tesztelés önállóan nem képes a teljesítményoptimalizálásra, bár segíthet az olyan problémák azonosításában, amelyek teljesítménybeli gondokat okozhatnak.
                            A dokumentáció helyettesítése: A tesztelés nem helyettesíti a fejlesztési dokumentációt vagy a specifikációkat, hanem azok alapján ellenőrzi, hogy a rendszer megfelel-e az előírt elvárásoknak.

#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?

            Az egységtesztelés (unit testing) egy szoftvertesztelési módszer, amely a szoftver legkisebb egységeit (általában egy-egy funkciót vagy metódust) külön-külön, izolált környezetben teszteli annak érdekében, hogy biztosítsa azok helyes működését. Az egységtesztelés célja, hogy ellenőrizze, hogy egy adott kódblokknak, például egy függvénynek vagy metódusnak, a bemeneti adatokra adott válasza megfelelő-e, és hogy a kód minden elágazása, ciklusa és feltételezése helyesen működik.

#### ✅ Mik a tesztszintek, és mi a különbség köztük?

        A szoftvertesztelés során különböző tesztszinteket alkalmazunk, amelyek mindegyike a rendszer egy-egy aspektusának validálására koncentrál. Minden tesztszint más-más szempontból vizsgálja a szoftver működését, és a különböző tesztek különböző mélységű tesztelést biztosítanak.

#### ✅ Mi a különbség a verifikáció és a validáció között?

        A verifikáció és a validáció két különböző, de szorosan összefüggő fogalom a szoftvertesztelésben és a minőségbiztosítási folyamatokban. Bár gyakran használják őket egymás szinonimájaként, van jelentős különbség a két fogalom között. A verifikáció célja annak ellenőrzése, hogy a rendszer a helyes módon lett-e megépítve. A validáció célja annak biztosítása, hogy a helyes terméket építettük meg.

#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?

        A tesztelési típusok különböző megközelítéseket alkalmaznak a szoftver minőségének és megbízhatóságának biztosítására. Az egyes típusok különböző aspektusokat vizsgálnak, mint például a funkcionalitás, a teljesítmény, a biztonság és az interoperabilitás. A következőkben ismertetem a leggyakoribb tesztelési típusokat és a köztük lévő különbségeket.

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?

        fehér doboz: Belső működés: A fehér doboz tesztelésnél a tesztelők teljes hozzáféréssel rendelkeznek a kód belső struktúrájához. Ismerik a program belső működését, a forráskódot, az adatfolyamokat és az algoritmusokat.
Cél: A cél, hogy biztosítsák, hogy a rendszer minden kódblokkját megfelelően tesztelték, és minden elágazás, ciklus és útvonal lefedésre kerüljön. Ezzel biztosítható, hogy a kód minden részlete megfelelően működik.
Módszer: A tesztelő a kódot elemzi, és olyan teszteket tervez, amelyek a kód minden egyes részét (például függvényeket, ciklusokat, elágazásokat) lefedik. Az eredményeket a kód belső struktúrája alapján értékelik.

        szürke doboz:Belső működés részleges ismerete: A szürke doboz tesztelésnél a tesztelők részleges hozzáféréssel rendelkeznek a rendszer belső működéséhez. Nem ismerik teljes mértékben a kódot, de információval rendelkeznek a rendszer architektúrájáról és esetleges funkcionális specifikációiról.
Cél: A tesztelők célja a rendszer működésének tesztelése az alkalmazás logikája és struktúrája alapján, de nem szükséges, hogy minden egyes kódrészletet ismerjenek. A tesztelő így képes a hibák azonosítására a kód belső logikája alapján, de nem minden részletre van rálátása.
Módszer: A tesztelő a rendszer egyes funkcióit a belső működés alapján teszteli, de a tesztelés a felhasználói interakciók, valamint az alkalmazás és a háttérrendszerek közötti kommunikáció szempontjából is történik. A tesztelés során általában használnak API tesztelést, integrációs tesztelést és részleges kódellenőrzést.


        fekete doboz:Belső működés ismerete nélkül: A fekete doboz tesztelésnél a tesztelő nem rendelkezik semmilyen információval a rendszer belső működéséről vagy kódjáról. A tesztelés kizárólag a rendszer bemenetére és kimenetére koncentrál.
Cél: A cél annak biztosítása, hogy a rendszer a megfelelő módon reagáljon a bemeneti adatokra, és hogy a várt kimenetet adja vissza, anélkül, hogy bármit is tudnának annak belső működéséről.
Módszer: A tesztelők bemeneteket biztosítanak a rendszer számára, és figyelik a kimenetet, hogy meggyőződjenek arról, hogy a rendszer megfelel a specifikációkban és a felhasználói elvárásokban meghatározott működésnek.

#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?

        A felhasználói elfogadási teszt (UAT) és a rendszerteszt két különböző típusú tesztelési fázist jelölnek a szoftverfejlesztési életciklus során. Bár mindkettő a rendszer működésének validálására szolgál, különböző célokat, módszereket és résztvevőket érintenek.
        Felhasználói elfogadási teszt (UAT - User Acceptance Testing):
Célja: Az UAT célja annak biztosítása, hogy a szoftver megfeleljen a végfelhasználók igényeinek és elvárásainak, és hogy a szoftver a valós felhasználói környezetben is megfelelően működjön.
Fókusz: Az üzleti követelmények, a felhasználói elvárások és a rendszer funkcionális szempontjai. Az UAT során a felhasználók tesztelik a rendszert, hogy ellenőrizzék, hogy az valóban úgy működik, ahogyan azt a vállalati igények szerint elvárták.
Módszer: A tesztelés a szoftver végfelhasználóinak a részvételével történik, akik nem a fejlesztők, hanem a cégen belüli üzleti szakemberek, termékmenedzserek, vagy akár tényleges felhasználók lehetnek.

Rendszerteszt (System Testing):
Célja: A rendszerteszt célja annak biztosítása, hogy az összes rendszerkomponens és funkció együtt megfelelően működjön. A tesztelés során a szoftver teljes rendszert vizsgálják, hogy az integrált részek helyesen működnek-e és együttműködnek-e.
Fókusz: A rendszertesztelés a rendszer architektúráját, a különböző modulok közötti interakciókat, valamint az összes technikai követelményt ellenőrzi.
Módszer: A tesztelők a rendszer minden aspektusát átvizsgálják, beleértve a funkcionalitást, a biztonságot, a teljesítményt, a kompatibilitást és a megbízhatóságot. A rendszertesztelést általában a fejlesztőcsapat vagy tesztelőcsapat végzi.

#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
Ha egy webalkalmazás új funkciókat kap, a regressziós tesztelés során ellenőrzik, hogy a régi funkciók (például a bejelentkezés, adatkezelés, vagy vásárlási folyamat) nem sérültek-e a módosítások miatt.

Egy új verzió telepítése után ellenőrzik, hogy az alkalmazás elindul-e, a fő menük és funkciók válaszolnak-e, és hogy nincs-e súlyos hiba, amely miatt a tesztelést le kellene állítani.

#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?

statikus: A statikus tesztelés célja a kód vagy dokumentáció átvizsgálása anélkül, hogy azt futtatnánk. Ez a tesztelési típus a rendszer szintaktikai és formai hibáit próbálja kiszűrni, valamint a fejlesztési dokumentációk és kódrészletek megfelelőségét ellenőrzi.

Dinamikus: A dinamikus tesztelés célja annak biztosítása, hogy a rendszer működése és funkcionalitása megfeleljen az elvárásoknak. A dinamikus tesztelés során a szoftver fut, és a tesztelő különböző bemeneti adatokat biztosít annak ellenőrzésére, hogy a program megfelelően reagáljon és a várt eredményeket adja.

### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!

    V model: A V-modell a vízesés modell egy kiterjesztett változata, ahol a fejlesztési és tesztelési tevékenységek párhuzamosan, szorosan összekapcsolva történnek. A "V" alak arra utal, hogy a fejlesztés és a tesztelés fázisai szimmetrikusan követik egymást: a bal oldalon a fejlesztési tevékenységek (tervezés, kódolás), míg a jobb oldalon a tesztelési tevékenységek (ellenőrzés, validálás) zajlanak.

    Vizesés:A vízesés modell a szoftverfejlesztés egyik klasszikus megközelítése, amely szigorú, lineáris fázisokat követ. Az egyes fázisok (tervezés, fejlesztés, tesztelés, karbantartás) egymás után következnek, és a tesztelés csak a fejlesztési szakasz befejezése után kezdődik.

    Angile megközelítés: Az Agile (agilis) módszertan iteratív és inkrementális fejlesztési megközelítést alkalmaz. Az Agile szerint a szoftverfejlesztés gyorsan változó környezetben történik, ahol a fejlesztést és tesztelést folyamatosan, ciklikusan végezzük. Az Agile hangsúlyozza a folyamatos együttműködést, a visszajelzéseket és a változásokra való gyors reagálást.


<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">





## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
-Hiba reprodukálása

-Hiba elemzése

-Kód ellenőrzése

-Hiba megoldása

-Tesztelés és validálás

-Dokumentálás

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!

-Tesztelési esettanulmány (Test Case Report)

-Funkcionális tesztelés (Functional Testing Report)

-Regressziós tesztelés (Regression Testing Report)

-Teljesítménytesztelés (Performance Testing Report)

-Biztonsági tesztelés (Security Testing Report)

#### ✅ Mit tartalmaz egy hibajelentés?

-Hiba azonosító

-Hiba leírása

-Környezet

-Reprodukciós lépések

-Várt eredmény

-Tényleges eredmény

-Súlyosság

-Mellékletek

#### ✅ Hogyan rangsorolnál egy hibát?

1. Súlyosság:

    -Kritikus: A hiba a rendszer működését teljesen megakadályozza, és azonnali javítást igényel.

    -Magas: A hiba jelentős működési problémát okoz, de van megoldás a munkavégzéshez. A hiba javítása sürgős, de nem kritikus.

    -Közepes: A hiba hatással van a felhasználói élményre, de nem akadályozza a rendszer fő funkcióit. A javítás nem sürgős, de fontos.

    -Alacsony: A hiba nem jelentős és nem okoz komoly problémát. A javítás késleltethető.

2. Frekvencia

3. Hatókör

4. Biztonság

5. Időbeli határ


## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
Ismétlődő feladatok: Azokat a teszteket, amiket gyakran kell futtatni, például regressziós teszteket, mivel az automatizálás segít csökkenteni az időt és az emberi hibákat.

Nagy adathalmazokkal végzett tesztek: Amikor több ezer adatot kell ellenőrizni, az automatizált tesztek gyorsabban végezhetik el a munkát.

Komplex, sok lépést igénylő tesztek: Automatizált tesztekkel jobban kezelhetők a több lépést és interakciót tartalmazó műveletek.

Platform- és böngészők közötti tesztelés: Ha több különböző platformon vagy böngészőben kell tesztelni a rendszert, az automatizált tesztelés hatékony megoldást kínál.

Regression tesztelés: Azok a tesztek, amelyek az új kódok integrálása után a régi funkcionalitást ellenőrzik.

Nem érdemes automatizálni:

Egyszeri tesztek: Ha egy teszt csak egyszer fut le, nincs értelme automatizálni, mivel a kezdeti beruházás nem térül meg.

Dizájn és UI/UX tesztelés: Az emberi szem és intuíció jobb az UI/UX tesztelésben, mivel az automatizált tesztek nem mindig tudják pontosan értékelni a felhasználói élményt.

Dynamic content tesztelése: Ha a weboldalon dinamikusan változó tartalom van (pl. időjárás előrejelzés, hírek), az automatizált tesztelés nehezebbé válik.

Bonyolult hibaelhárítási tesztek: Az olyan tesztek, amelyek speciális környezetet igényelnek vagy hibák kezelésére vannak kitalálva, gyakran nem könnyen automatizálhatók.



#### ✅ Írj le egy jó automatizált tesztet!
from selenium import webdriver
from selenium.webdriver.common.keys import Keys
import unittest

class TestLogin(unittest.TestCase):
    def setUp(self):
        self.driver = webdriver.Chrome()  # Válaszd a megfelelő böngészőt
        self.driver.get("https://yourwebsite.com/login")

    def test_valid_login(self):
        driver = self.driver
        # Felhasználónév mező keresése és kitöltése
        username = driver.find_element_by_name("username")
        username.send_keys("testuser")

        # Jelszó mező keresése és kitöltése
        password = driver.find_element_by_name("password")
        password.send_keys("securepassword")

        # Bejelentkezés gomb keresése és rákattintás
        login_button = driver.find_element_by_name("login_button")
        login_button.click()

        # Ellenőrizzük, hogy sikeres bejelentkezés után a megfelelő oldalra jutottunk
        self.assertIn("Dashboard", driver.title)

    def tearDown(self):
        self.driver.quit()

if __name__ == "__main__":
    unittest.main()


#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
Selenium: A Selenium egy népszerű, nyílt forráskódú automatizálási keretrendszer, amelyet webalkalmazások tesztelésére használnak. Különböző programozási nyelvekkel (például Python, Java, C#, Ruby) kompatibilis, és lehetővé teszi a web böngészők automatizált vezérlését.

Selenium IDE (Integrated Development Environment):

A Selenium IDE egy böngészőbővítmény, amely lehetővé teszi a tesztek felvételét és lejátszását anélkül, hogy kódolni kellene.

Főleg fejlesztők és tesztelők számára használható gyors prototípusok készítésére.

A tesztet grafikus felületen rögzíthetjük és módosíthatjuk, de nem olyan rugalmas, mint a Selenium WebDriver.

Selenium WebDriver:

A Selenium WebDriver egy fejlettebb API, amely lehetővé teszi a weboldalak programozott vezérlését. Ezt a Selenium használatával írt tesztekhez használják.

A WebDriver közvetlenül irányítja a böngészőt, tehát nincs szükség egy másik rétegre (mint a Selenium RC esetében).

A WebDriver segítségével könnyen kezelhetők különböző böngészők és platformok.

#### ✅ Hogyan lehet azonosítani a webes elemeket?
ID (azonosító): Az ID-k egyedi azonosítók minden HTML elemen belül. Ha egy elemnek van ID-je, az a legjobb módszer az azonosításra.

Class Name (osztály név): Ha több elem is rendelkezik ugyanazzal az osztálynévvel, akkor egy listát kaphatunk, amit végig iterálhatunk.

Name (név): A name attribútum is egy hasznos azonosító.

XPath: Az XPath segítségével a DOM struktúrában való navigálással találhatunk meg elemeket.

CSS Selector: CSS selektorokat is használhatunk, amelyek rugalmas módot biztosítanak az elemek azonosítására.

Link Text / Partial Link Text: Ha egy elem hivatkozás, akkor a teljes vagy részleges szövege alapján is kereshetünk rá.

#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!

Webes tesztelésnél sokszor előfordul, hogy az elemek nem azonnal elérhetők, ezért szükséges várakozni, amíg az adott elem betöltődik vagy interakcióba léphetünk vele. A Selenium-ban kétféle várakozást különböztetünk meg:

Statikus várakozás (Thread.sleep):

Probléma: Ez a módszer nem túl hatékony, mivel a teszt a megadott időpontig folytatja, akkor is, ha az elem már elérhető, vagy éppen nem elérhető.

Hiba: A túlzott statikus várakozás lassítja a tesztet, és nem garantálja, hogy az elem tényleg elérhetővé válik a megadott időpontig.

Dinamikus várakozás (Explicit Wait):

Javítás: Az explicit várakozás során meghatározhatjuk, hogy hány másodpercig várjon a teszt, és várja meg, hogy az elem megjelenjen vagy elérhetővé váljon egy feltétel alapján.

Példa (Python + Selenium):

python
Másolás
Szerkesztés
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC

driver = webdriver.Chrome()
driver.get("https://example.com")
wait = WebDriverWait(driver, 10)  # 10 másodpercig várunk

# Várjuk, hogy az elem megjelenjen
element = wait.until(EC.presence_of_element_located((By.ID, "login_button")))
Implicite várakozás:

Probléma: Az implicite várakozás globálisan hat a tesztre, és minden egyes elem keresésekor alkalmazza, amit nem biztos, hogy minden tesztnél megfelelő.

Javítás: Használhatjuk akkor, ha az egész tesztesetben szeretnénk várakozási időt beállítani.

Lehetséges hibák és okok:

Elem nem található: A leggyakoribb hiba, amikor az elem, amire várunk, nem található meg a megadott locatorral, vagy nem töltődik be időben.

Nem megfelelő várakozási idő: Ha túl rövid az idő, a teszt nem találja meg az elemet, ha túl hosszú, akkor a teszt feleslegesen lassú lesz.

Synchronizációs problémák: Az oldal dinamikus tartalommal rendelkezik (pl. AJAX hívások), és a Selenium nem várja meg a tartalom betöltődését, így a teszt hibát ad.

Elem láthatatlansága: Az elem már létezik, de nem látható vagy nem interakcióképes (pl. egy modal ablak mögött van).

#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
POM (Page Object Model):

Minden oldalnak saját osztálya van, amely az oldalon található elemeket és azok interakcióit tartalmazza.

Előnyök: Kód újrafelhasználhatóság, könnyű karbantartás, elkülöníti a tesztet az implementációtól.

Hátrányok: Kódolási nehézségek, ha az oldal struktúrája gyakran változik.

Keyword Driven Testing:

A tesztelők a tesztet kulcsszavak segítségével írják meg, például "Klikk", "Írj", "Ellenőrizd", ami végül meghatározza a teszt lépéseit.

Előnyök: Tesztelők nem szükségesek, hogy programozni tudjanak, a tesztek könnyen olvashatók.

Hátrányok: Kód újrafelhasználás korlátozott, hibák könnyen előfordulhatnak, ha a kulcsszavak nincsenek jól definiálva.

#### ✅ Mi a különbség a TDD és BDD között?

TDD (Test-Driven Development): A tesztek írása előzi meg a kód megírását. A teszt először meghatározza a kívánt funkciót, majd a fejlesztő írja meg hozzá a kódot.

Cél: A kód minőségének biztosítása.

BDD (Behavior-Driven Development): A teszteket "viselkedés" alapú nyelven írják, amelyek a végfelhasználói élményre összpontosítanak. A tesztelők és fejlesztők közösen dolgoznak a teszt szcenáriókon.

Cél: A felhasználói igények és a funkciók jobb megértése.

#### ✅ Mi az API tesztelés és miért hasznos?
API tesztelés során az alkalmazás programozási interfészeinek (API) működését teszteljük. Ez magában foglalja az adatbevitel, kimenet, hibakezelés és válaszidők ellenőrzését.

Miért hasznos?

Részletes validáció: Teszteli az adatcserét két rendszer között, és biztosítja, hogy az API helyesen válaszol.

Funkcionális és teljesítmény tesztelés: API-tesztekkel könnyen vizsgálható a rendszer hatékonysága és megbízhatósága.



#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?

Az adatvezérelt tesztelés során különböző bemeneti adatokat alkalmazunk ugyanarra a tesztre, hogy validáljuk a rendszer viselkedését különböző adatokkal.

Miért hasznos?

Széleskörű tesztelés: Nagy adatváltozásokkal ellenőrizhető a rendszer.

Költséghatékony: Egyetlen teszt többször is végrehajtható különböző bemeneti adatokkal, ami csökkenti a tesztelés költségeit és időtartamát.