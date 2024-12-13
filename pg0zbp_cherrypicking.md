
# Pontvadász ZH


## Árlap


### Windows Forms Application



##### User Interface



-   `1x2p` Az alkalmazásból a **kilépés csak megerősítő kérdés után** lehetséges.
- Megvalósítva a Form1-en.
    
-   `3x2p` Olyan alkalmazás **elrendezés, melyben gombok lenyomására UserControl-ok kerülnek elhelyezésre egy Panel vezérlőben**, teljesen kitöltve azt. Minden gombra jár a pont, amennyiben az funckuonlalitással rendelkező UserControl-t tölt be.
- 2 megvalósítva TanarCotroll és ErtekelesControll neveken, illetve a Form1-en a panel és a gombok.
    
-   `3x1p` **Többablakos alkalmazás** legalább két felugró ablakkal. Minden Form-nak saját osztályon kell alapulnia, és funcionalitással kell rendelkeznie. Az ablakok nyílhatnak gombokkal vagy felső menüből is.
- Megvalósítva az új értékelés hozzáadása formon. Ugyan az új értékelés hozzáadása funkció nem működik, de a form megnyílik és a textboxok adatkötve vannak.

-   `1x2p` **Anchorok alkalmazása**: az alkalmazás egészében meg van oldva, hogy az ablak átméretezésekor ki legyen használva a rendelkezésre álló terület.
- Megvalósítva a Formokon, UserControllokon.
    

##### Tábla adatainak megjelenítése `ListBox`-ban.



-   `1x2p` Adatok megjelenítése
- Megvalósítva a TanarControllon.


-   `2x2p` Ha az adatok tetszőleges módszerrel, pl. `TextBox`-on keresztül szűrhetőek.
- Megvalósítva a TanarControllon.

-   `1x2p` Ha a tábla adatforrása saját osztály.
- Megvalósítva a TanarControllon (amennyiben az adatbázis példányosítása annak számít. Amennyiben nem, nem salyát osztály az adatforrás).

##### Tábla adatainak megjelenítése `DataGridView`-ban



-   `1x2p` Adatok megjelenítése
- Megvalósítva az ErtekelesControllon.

-   `1x2p` Ha a tábla adatforrása saját osztály.
- Megvalósítva az ErtekelesControllon (amennyiben az adatbázis példányosítása annak számít. Amennyiben nem, nem salyát osztály az adatforrás).

##### Adatkötés `BindingSource` -on keresztül



-   `1x2p` Működő `BindingSource`
- Megvalósítva a UserControllokon.

-   `3x1p` Egy `BindingSource`-ra egy gyűjemény megjelenítésére alkalmas vezérlő (ListÍBox, ComboBox, DataGridVIew) mellett más adatkötött vezérlő is van kötve, mint `TextBox`, `DateTimePicker`, `ComboBox` idegen kulcs értékének beállítására, stb.
- Megvalósítva az ErtekelesFormon. 

##### Új rekord rögzítése (Funkció nem működik)

-   `1x1p` Ha legalább egy nem kulcs mező, pl. _Mennyiség_ is fel van véve
- A felvételt nem lehet megvalósítani a megoldásom alapján, viszont az értékelés számmal opciónál egy numerikus értéket lehetne felvenni az új rekord egyik mezőjébe.

-   `1x2p` Felugró ablakon keresztül történik _Ok_ és _Mégse_ gombbal
- A funkció nem működik, de a kód tartalmazza ezt a pontot, így a megvalósítás sikertelen, de próba a megvalósításra történt.


##### Rekord törlése



-   `1x2p` Sikeres törlés
- Megvalósítva az ErtekelesControllon.

-   `1x2p` Megerősítéshez kötött törlés
- Megvalósítva az ErtekelesControllon.



### ASP .NET


ASP .NET alkalmazás, melyet lehet a Forms alapú projekttel közös solution-ben létrehozni.

-   `1x2p` `program.cs` beállítása `wwwroot` mappában tárolt statikus tartalmak megosztására
- Megvalósítva a cseresznye_pg0zbp projekten belül.

##### API végpontok



-   `1x3p` Teljes SQL tábla adatainak szolgáltatása API végponton keresztül
- Megvalósítva a tanarControlleren.

-   `2x2p` SQL tábla egy választható rekordjának szolgáltatása API végponton keresztül
- Megvalósítva kétszer a tanarControlleren.

-   `1x3p` SQL tábla egy választható rekordjának törlése
- Megvalósítva a tanarControlleren.

-   `1x5p` Új rekord felvétele `HttpPost` metóduson keresztül SQL táblába
- Megvalósítva a tanarControlleren.


##### Javascript



-   `2x5p` (pl: szöveg és kép) DOM feltöltése javascripttel (vizsgán írandó, NEM HOZOTT, aki ezt választja az a hozott anyagba nem rakhatja bele a js kódot amivel feltölti a tartalommal a DOM-ot, tehát ez az előre feltöltött `hozott.js`-ben nem lehet benne, vizsgán kell megírni egy `vizsga.js` fájlba.)
- Megvalósítva a vizsga.js-en (adatokkal való feltöltés és adat hozzáadása).


##### Saját Adatbázis



SQL script formájában, de legjobb Azure SQL szerveren hosztolni

-   `3x1p` Az alkalmazásban használt táblánként pont
- Megvalósítva kétszer a windowsform projektben.

-   `1x1p` Az adatbázis adatainak forrásmegjelölése értsd: miből készült és hogyan
- Az adatbázis három táblából áll Tanarok, Ertekelesek és Tantargyak. Ezek adatait a ChatGPT által generált adatokkal töltöttem fel SSMS-ben. Maga az adatbázis Azure-ban készült.

-   `1x2p` Az adatbázis saját Azure SQL szerveren van
- Megvalósítva, egy SQL server ennek a projektnek, melynek neve tanarDB, kapcsolódásnál a felhasználónév veghbalazs, a jelszó pedig Password12345. A connection string pedig: Data Source=tanarok.database.windows.net;Initial Catalog=tanarokDB;Persist Security Info=True;User ID=veghbalazs;Password=Password12345;Trust Server Certificate=True.

##### Weboldal



Itt csak azok az elemek számíthatóak be, amelyeknek meg van a ZH alatt felépített API végpontja.

-   `1x1p` A weboldalnak van egy értelmezhető struktúrája
- Megvalósítva az index.html-ben és a main.css-ben.

-   `1x1p` A weboldal dinamikus tartalommal tölthető fel adatbázison keresztül
- Megvalósítva a vizsga.js-ben.

-   `1x1p` A weboldal használ legalább 20 sor értelmes css-t
- Megvalósítva a main.css-ben.

-   `1x1p` A weboldal javascriptje más funkciót is ellát, mint az adatok betöltése
- Megvalósítva a vizsga.js-ben.

### Egyéb, extra

-   `2x1p` `Scaffold-DbContext` használata (ajándék)
- Megvalóítva, létrehozta a TanarokdbContextet.az
    
