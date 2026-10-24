# Változásnapló

A projekt a [Semantic Versioning](https://semver.org/) verziózást követi. A dátumok `ÉÉÉÉ-HH-NN` formátumúak.

## [Kiadatlan]

### Hozzáadva

- A Haladó alapadatok blokk új Kaland mezőt kapott az aktuálisan játszott kaland címéhez; az érték automatikusan mentődik, exportálható és importálható.

- A „Meghaltál” képernyőn külön jegyzetmező jelenik meg a mesélő utasításaihoz; ugyanaz a mentett jegyzet a Halálmentő dobások blokk lenyitható „Mesélő utasításai” részében is elérhető, és az Export/Import része.

- Ha valamelyik halálmentő eredményből összegyűlik mindhárom jelölés, az eredmény az aktuális körben még látható marad, a következő kör kezdetén pedig a siker- és kudarcjelölők automatikusan törlődnek.

- A halálmentőjelölők látható állapota most körváltáskor, Combat újranyitásakor, karakterbetöltéskor és importáláskor is a mentett értékekből áll helyre, így a korábbi sikerek és kudarcok a harmadik jelölésig megmaradnak.

- A halálmentő Combat nézet már csak negatív HP-nál aktiválódik; kézi gyógyítási értéket is elfogad, három siker esetén 0 HP-ra stabilizál, három kudarc esetén pedig „Meghaltál” jelzést jelenít meg.

- A Jegyzetek Cím gombja kapcsolóként működik: második kattintásra visszaállítja a címsort normál bekezdéssé.

- A Jegyzetek felsorolásai megfelelő belső behúzást és tördelést kaptak, így a listajelek keskeny képernyőn is a szerkesztőn belül maradnak.

- A Beállítások menü új Jegyzetek nézetet kapott formázható szöveggel, automatikus karaktermentéssel, Export/Import támogatással, Combat méretű desktop ablakkal és teljes képernyős mobilnézettel.

- A Fegyverek panel most belső görgetősáv nélkül, a tartalmához igazodó magassággal jelenik meg desktopon és keskeny képernyőn is.

- A desktop elrendezés ismét fix, háromoszlopos szerkezetet használ, az Elrendezés funkció pedig megszűnt. Mobilon a panelek rögzített sorrendje: Karakter adatok, Hit Points, Inspiráció, Tulajdonságok, Harci értékek, Skills, Fegyverek, Kasztjellemzők, kasztspecifikus panelek, Felszerelés, Pénz, Haladó alapadatok, Életerőkockák, Mentődobások, Egyéb jártasságok.
- Minden választható faj saját, semleges, árnyékban maradó arcú fantasy portrét kapott a `DnD portrék` mappa aranykeretes képei alapján. A képek optimalizálva és közvetlenül a HTML-be ágyazva működnek; a feltöltött egyéni portré továbbra is elsőbbséget élvez, eltávolításakor pedig automatikusan az aktuális faj alapképe jelenik meg.
- A Barbár sötét vérvörös, kovácsoltvas és bronz palettát, a Sorcerer pedig ametisztlila és cián kristályfényeket kapott, így mindkettő markánsan elkülönül a többi kaszttémától.
- A fajválasztó Aasimar, Genasi és Tabaxi lehetőségekkel bővült. Az Aasimar és Genasi alfajai is választhatók; a méret-, nyelv- és faji jellemző összefoglalók automatikusak, a Tabaxi pedig automatikusan megkapja az Észlelés és Lopakodás jártasságot.
- Prémium, kasztspecifikus fantasy vizuális rendszer mind a 12 alapkaszthoz: önálló színpaletta, beágyazott SVG-címer, háttérmotívum, panelornamentika és fényhatás.
- Kompakt heraldikai fejléc kasztnévvel és tematikus mottóval; desktopon részletes, mobilon egyszerűsített elrendezéssel.
- A tulajdonságmódosítók tematikus fantasy medálokat, a meglévő kaszterőforrások pedig díszített, az aktuális értékhez kapcsolt kijelzőket kaptak.
- A kaszttémák a sötét és pergamen megjelenéssel egymástól függetlenül működnek, támogatják a csökkentett animációt, és nem igényelnek külső erőforrást.
- Pergamen módban mind a 12 kaszt erősebb, külön hangolt tintaszínt kapott; a címer, heraldikai fejléc, panelkeretek, címsávok, sarokdíszek, tulajdonságmedálok és profi skill-sorok jobban őrzik az aktív kaszt vizuális karakterét.
- A Beállítások, Combat és pihenőgombok, valamint a mobil panelcímek az aktív kaszt színeit követik; a heraldikai fejléc explicit mobilnézetben is kompakt, teljes szélességű és túlcsordulásmentes.
- Az Elrendezés szerkesztő desktop és keskeny képernyőn egyaránt elérhető; a külön Desktop/Mobile kapcsolók megszűntek, a mobil elrendezés 768 px alatt automatikusan aktiválódik.
- Mobilnézetben a Tulajdonságok és Harci értékek külső kerete, háttere és sarokornamentikája megegyezik a Fegyverek és a többi kaszttémás panel kialakításával.
- A Háttér választó minden kasztnál és alosztálynál a teljes, 13 elemes PHB 2014 háttérlistát mutatja; a korábbi kasztonkénti ajánlási szűrés megszűnt.
- A Skills panel csak a kaszt, faj, alosztály és háttér alapján szabályosan választható jártasságokat engedi kijelölni, figyeli a választási kereteket, és letiltja az elérhetetlen vagy automatikusan járó sorokat.
- Az automatikusan járó skill-jártasságok ugyanazt az arany kiemelést és kitöltött jelölőt kapják, mint a kézzel választott jártasságok, miközben továbbra sem kapcsolhatók ki.
- A betöltött 2014-es varázslatok sebzésmezőt kaptak: 92 sebző varázslatnál automatikus alapérték és szintfüggő skálázás jelenik meg, az egyedi varázslatok értéke kézzel is szerkeszthető.
- A Combat varázslatválasztó megjeleníti a sebzésképletet, és a sebző varázslatok használata után felajánlja a kockánkénti sebzésdobást.
- Combat módban a varázslás dobása után külön „Sikeres találat” és „Sikertelen találat” döntés jelenik meg; sebzésdobásra kizárólag sikeres, sebző varázslat lép tovább.
- Sorcerer PHB 2014 kasztképességek: Font of Magic, Flexible Casting, választható Metamagic lehetőségek és Sorcerous Restoration.
- A Combat mód automatikusan kezeli a Sorcerer varázserőpont-költségeit, a rekesz–pont átalakítást és a Quickened Spell bónuszakciós varázslását.
- Bárd PHB 2014 kasztképességek, automatikus Expertise, Song of Rest, Countercharm, Magical Secrets és College of Lore/Valor jellemzők.
- A Combat mód kezeli a Bardic Inspiration, Combat Inspiration, Cutting Words, Countercharm és Superior Inspiration erőforrásait.
- Tolvaj (Rogue) PHB 2014 kasztképességek, automatikus Expertise, Sneak Attack, Cunning Action és a Thief, Assassin, valamint Arcane Trickster alosztályok jellemzői.
- A Tolvaj heraldikai fejléc sértetlen, belső geometrikus sarokdíszeket kapott; a Bárd és Tolvaj Expertise mezői kizárólag a Skills panelen már profi képességeket kínálják, kizárják a duplikációt, és az Expertise kiemelése azonnal megjelenik a skill soron.
- A Combat mód kezeli a Fast Hands, Uncanny Dodge, Evasion, Assassinate, Versatile Trickster, Thief’s Reflexes és Stroke of Luck használatát.
- Cleric PHB 2014 kasztképességek, automatikus varázslási keret, Turn/Destroy Undead, Divine Intervention és mind a hét PHB domain jellemzői.
- A Combat mód külön kezeli a domainenkénti Channel Divinity lehetőségeket, reakciókat, bónuszakciókat és használatszámlálókat.
- Fighter PHB 2014 kasztképességek, Fighting Style, Extra Attack, Second Wind, Action Surge és Indomitable erőforrások.
- Champion, Battle Master és Eldritch Knight jellemzők, automatikus kritikus tartomány, manőverkockák, War Magic és Fighter Combat műveletek.
- Monk PHB 2014 kasztképességek, automatikus harcművészeti kocka, páncél nélküli AC, mozgásbónusz, Ki-mentő DC és Diamond Soul mentődobások.
- Way of the Open Hand, Way of Shadow és Way of the Four Elements jellemzők, Ki-költségek és Combat műveletek.
- Paladin PHB 2014 kasztképességek, automatikus Aura of Protection, Fighting Style, Divine Smite, Lay on Hands és esküerőforrások.
- Oath of Devotion, Oath of the Ancients és Oath of Vengeance jellemzők, Isteni Energia lehetőségek, reakciók és magasabb szintű Combat műveletek.
- Warlock PHB 2014 Pact Magic, Pact Boon, Mystic Arcanum, Eldritch Master és követhető Eldritch Invocation képességek.
- Archfey, Fiend és Great Old One patrónusjellemzők, pihenőalapú erőforrások, reakciók és Combat műveletek.
- Wizard PHB 2014 varázskönyv, Arcane Recovery, Spell Mastery, Signature Spells és előkészítési összegzés.
- Mind a nyolc Arcane Tradition jellemzői, követhető erőforrásai, Combat műveletei, reakciói és Evocation sebzésmódosítója.
- Mobilnézetben balra igazított karakter-, kaszt- és alosztálycímkék, valamint ikonok a Tulajdonságok és Harci értékek címsorában.
- A Combat kör bármely szakaszban, külön áttekintés nélkül lezárható a „Befejeztem a körömet” megerősítés után.
- A kör befejezésének megerősítése a Combat mód megjelenéséhez igazodó, reszponzív párbeszédablakot kapott.
- A külön Combat „Áttekintés” lépés megszűnt; az aktuális és korábbi körök eseményei a Műveletek nézet naplójában maradnak elérhetők.
- A halálmentődobás ablaka üres aktuális HP mezőnél zárva marad, és csak ténylegesen megadott 0 vagy negatív értéknél nyílik meg.
- A halálmentő sikerek és kudarcok alapértelmezett pipái témába illő, arany csillag- és vörös keresztpecsétekre változtak.
- A halálmentők külön előugró ablaka megszűnt; Combat módban a kezdeményezés után 0 vagy negatív HP-nál a műveletek helyén jelenik meg a halálmentő felület.
- A Combat halálmentő felület kockatípusból, darabszámból és módosítóból számolt gyógyítást tud dobni, naplózni és automatikusan átvezetni az aktuális HP-ra.
- A Combat saját kör főképernyője tömörebb műveletválasztót és egyszerűbb állapotsort kapott; a duplikált következőlépés-gomb csak speciális támadásfolytatásnál jelenik meg.

### Tervezett

- GitHub-tárhely és kiadási URL-ek beállítása.
- Frissítésértesítő bekötése a stabil `version.json` végpontra.
- Automatikus kiadási csomag és ellenőrzőösszeg készítése.

## [0.1.0] – 2026-10-22

### Hozzáadva

- Asztali és mobil karakterlapnézet.
- Átrendezhető, összecsukható panelek és megjegyzett panelállapotok.
- Combat mód kör-, akció-, bónuszakció-, reakció-, támadás- és sebzéskezeléssel.
- Automatikus kaszt-, faj-, alfaj- és alosztályfüggő varázslatlista.
- Összecsukható, szint és forrás szerint csoportosított varázslatok.
- Druida vad alak, ranger állati társ és állati támadások támogatása.
- Érmék és drágakövek egységes nyilvántartása.
- Karakterportré, inspirációs kocka, pihenők és erőforrás-visszatöltés.
- JSON-export és import.
- Megerősítéssel és előzetes mentési lehetőséggel működő karakterlapürítés.

### Módosítva

- A közeli kasztpaletták erősebben elkülönülnek: Tolvaj indigó–ezüst, Boszorkánymester smaragd–ibolya, Sorcerer rubinvörös–borostyán, Druida élő mohazöld, Ranger olíva–réz megjelenést kapott, hozzájuk igazított fejlécmotívumokkal és fényekkel.
- A pergamen mód, annak beállításgombja, mentett állapota és teljes stílusrétege megszűnt; a karakterlap egységesen a kasztspecifikus sötét fantasy témát használja.
- Egységes panelmegjelenés mobil- és asztali nézetben.
- Automatikus AC-, kezdeményezés-, mentődobás- és varázslási számítások.
- A szabad szöveges adatok két fő mezőbe rendezve: **Felszerelés**, illetve **Egyéb jártasságok és nyelvek**.
- A varázslatok aktív és inaktív állapotának kezelése a rendelkezésre álló erőforrások alapján.

### Javítva

- Combat visszalépés, saját fegyver választása és állati támadások folytató eseményei.
- Mobil és asztali elrendezési elcsúszások.
- Dinamikusan megjelenő kasztpanelek rendezhetősége.

