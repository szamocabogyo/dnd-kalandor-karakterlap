# Változásnapló

A projekt a [Semantic Versioning](https://semver.org/) verziózást követi. A dátumok `ÉÉÉÉ-HH-NN` formátumúak.

## [Kiadatlan]

### Hozzáadva

- Sorcerer PHB 2014 kasztképességek: Font of Magic, Flexible Casting, választható Metamagic lehetőségek és Sorcerous Restoration.
- A Combat mód automatikusan kezeli a Sorcerer varázserőpont-költségeit, a rekesz–pont átalakítást és a Quickened Spell bónuszakciós varázslását.

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

