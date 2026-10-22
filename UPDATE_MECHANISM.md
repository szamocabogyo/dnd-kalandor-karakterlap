# Frissítési mechanizmus terve

## Cél

A karakterlap egyetlen helyi HTML-fájlként továbbra is offline használható maradjon, miközben biztonságosan jelezni tudja az új stabil kiadásokat. A böngésző biztonsági korlátozásai miatt a helyi fájl nem írhatja felül automatikusan saját magát.

## Verziózás

- A projekt a `MAJOR.MINOR.PATCH` formátumot használja.
- `PATCH`: hibajavítás, adatstruktúra-változás nélkül.
- `MINOR`: új, visszafelé kompatibilis funkció.
- `MAJOR`: importot, mentési formátumot vagy működést törően módosító kiadás.
- A forrás verziója a `VERSION` és a `version.json` fájlban egyezzen.

## Kiadási csatorna

1. A GitHub alapértelmezett ága tartalmazza a stabil forrást.
2. Minden kiadás kapjon Git taget, például `v0.1.0`.
3. A GitHub Release tartalmazza:
   - a verziózott HTML-fájlt;
   - a változásnaplót;
   - SHA-256 ellenőrzőösszeget;
   - rövid frissítési és adatmentési útmutatót.
4. A gyökérben lévő `version.json` mindig a legújabb stabil kiadást írja le.

## Alkalmazáson belüli frissítésellenőrzés

A GitHub-tárhely URL-jének beállítása után a karakterlap opcionálisan lekéri a nyers `version.json` fájlt.

- Az ellenőrzés csak felhasználói műveletre vagy ritkán, például 24 óránként történjen.
- Ha a távoli verzió újabb, jelenjen meg az új verzió, a változásnapló és a letöltési hivatkozás.
- A letöltés előtt ajánlja fel a karakter JSON-exportját.
- A frissítés kézi fájlcserével történjen; a régi HTML maradjon meg visszaállítási lehetőségként.
- Hálózati hiba esetén a karakterlap működjön tovább értesítés nélkül.
- A letöltött fájlhoz jelenjen meg a kiadáshoz tartozó SHA-256 érték.

## Mentési kompatibilitás

- Az exportált JSON kapjon külön `schemaVersion` mezőt.
- Import előtt készüljön automatikus biztonsági export a jelenlegi karakterről.
- Minden új séma mellé készüljön migráció az összes támogatott korábbi sémából.
- Ismeretlen, újabb séma importját a program utasítsa vissza érthető hibaüzenettel.
- A migráció soha ne törölje az eredeti importfájlt.

## Ajánlott megvalósítási sorrend

1. GitHub-tárhely létrehozása és végleges nyilvános URL meghatározása.
2. Licenc kiválasztása és jogi/tartalmi ellenőrzés.
3. `schemaVersion` hozzáadása az exporthoz és importmigrációk létrehozása.
4. Kiadási csomagoló szkript és GitHub Actions munkafolyamat.
5. Alkalmazáson belüli, kézzel indítható frissítésellenőrzés.
6. Frissítési értesítő, mentés, letöltés és visszaállítás teljes folyamatának ellenőrzése.

## GitHub Actions terv

Tag létrehozásakor a munkafolyamat:

1. ellenőrzi, hogy a tag, a `VERSION` és a `version.json` verziója egyezik;
2. elkészíti a verziózott HTML-másolatot;
3. kiszámítja a SHA-256 összeget;
4. feltölti a fájlokat a GitHub Release kiadáshoz;
5. hibával leáll, ha a verziók vagy az ellenőrzőösszegek nem következetesek.

