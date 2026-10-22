# Változásnapló

A projekt a [Semantic Versioning](https://semver.org/) verziózást követi. A dátumok `ÉÉÉÉ-HH-NN` formátumúak.

## [Kiadatlan]

### Hozzáadva

- Sorcerer PHB 2014 kasztképességek: Font of Magic, Flexible Casting, választható Metamagic lehetőségek és Sorcerous Restoration.
- A Combat mód automatikusan kezeli a Sorcerer varázserőpont-költségeit, a rekesz–pont átalakítást és a Quickened Spell bónuszakciós varázslását.
- Bárd PHB 2014 kasztképességek, automatikus Expertise, Song of Rest, Countercharm, Magical Secrets és College of Lore/Valor jellemzők.
- A Combat mód kezeli a Bardic Inspiration, Combat Inspiration, Cutting Words, Countercharm és Superior Inspiration erőforrásait.
- Tolvaj (Rogue) PHB 2014 kasztképességek, automatikus Expertise, Sneak Attack, Cunning Action és a Thief, Assassin, valamint Arcane Trickster alosztályok jellemzői.
- A Combat mód kezeli a Fast Hands, Uncanny Dodge, Evasion, Assassinate, Versatile Trickster, Thief’s Reflexes és Stroke of Luck használatát.
- Cleric PHB 2014 kasztképességek, automatikus varázslási keret, Turn/Destroy Undead, Divine Intervention és mind a hét PHB domain jellemzői.
- A Combat mód külön kezeli a domainenkénti Channel Divinity lehetőségeket, reakciókat, bónuszakciókat és használatszámlálókat.
- Fighter PHB 2014 kasztképességek, Fighting Style, Extra Attack, Second Wind, Action Surge és Indomitable erőforrások.
- Champion, Battle Master és Eldritch Knight jellemzők, automatikus kritikus tartomány, manőverkockák, War Magic és Fighter Combat műveletek.
- Monk PHB 2014 kasztképességek, automatikus harcművészeti kocka, páncél nélküli AC, mozgásbónusz, Ki-mentő DC és Diamond Soul mentődobások.
- Way of the Open Hand, Way of Shadow és Way of the Four Elements jellemzők, Ki-költségek és Combat műveletek.
- Paladin PHB 2014 kasztképességek, automatikus Aura of Protection, Fighting Style, Divine Smite, Lay on Hands és esküerőforrások.
- Oath of Devotion, Oath of the Ancients és Oath of Vengeance jellemzők, Isteni Energia lehetőségek, reakciók és magasabb szintű Combat műveletek.

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

- Egységes panelmegjelenés mobil- és asztali nézetben.
- Automatikus AC-, kezdeményezés-, mentődobás- és varázslási számítások.
- A szabad szöveges adatok két fő mezőbe rendezve: **Felszerelés**, illetve **Egyéb jártasságok és nyelvek**.
- A varázslatok aktív és inaktív állapotának kezelése a rendelkezésre álló erőforrások alapján.

### Javítva

- Combat visszalépés, saját fegyver választása és állati támadások folytató eseményei.
- Mobil és asztali elrendezési elcsúszások.
- Dinamikusan megjelenő kasztpanelek rendezhetősége.

