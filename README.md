# D&D 5e kalandor karakterlap

Egyetlen HTML-fájlból futó, magyar nyelvű D&D 5e karakterlap. A karakteradatokat a böngésző helyi tárhelyén kezeli, ezért a lap internetkapcsolat nélkül is használható.

## Használat

1. Töltsd le a `DnD_kalandor_karakterlap.html` fájlt.
2. Nyisd meg egy korszerű böngészőben.
3. A **Beállítások → Export** paranccsal rendszeresen mentsd le a karaktert JSON-fájlba.
4. Másik böngészőben vagy eszközön a **Beállítások → Import** paranccsal töltsd vissza a mentést.

## Fő funkciók

- reszponzív asztali és mobil nézet;
- automatikus képesség-, mentődobás-, AC- és varázslási számítások;
- kaszt-, faj-, alfaj- és alosztályfüggő mezők;
- varázslatok forrás és szint szerinti kezelése;
- druida vad alak és ranger állati társ támogatása;
- körökre bontott Combat mód;
- rövid és hosszú pihenő kezelése;
- helyi mentés, JSON-export és import;
- átrendezhető és összecsukható mobil panelek.

## Adatvédelem

A karakteradatok alapértelmezés szerint a böngésző `localStorage` tárhelyére kerülnek. A projekt nem küldi el őket szerverre. A böngészőadatok törlése a karakter helyi mentését is eltávolíthatja, ezért ajánlott rendszeresen exportot készíteni.

## Fejlesztés

A projekt nem igényel fordítást vagy csomagtelepítést. A fő alkalmazásfájl közvetlenül megnyitható:

`DnD_kalandor_karakterlap.html`

A verziószám a `VERSION` fájlban található. A kiadások változásai a `CHANGELOG.md` dokumentumban szerepelnek. A kiadási és frissítési folyamatot az `UPDATE_MECHANISM.md` írja le.

## Szabályforrás és tartalom

A karakterlap több helyen D&D 5e 2014-es szabályokra, valamint külön megjelölt 2024-es ranger-megoldásokra épül. Publikálás előtt ellenőrizni kell, hogy minden terjesztett szöveg és adat megfelel-e az alkalmazandó licencfeltételeknek.

## Licenc

A projekthez még nincs kiválasztva nyílt forráskódú licenc. Nyilvános közzététel előtt a tulajdonosnak el kell döntenie, milyen feltételekkel engedélyezi a forrás használatát és módosítását.

