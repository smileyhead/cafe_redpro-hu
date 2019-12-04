# New Super Mario Bros. U magyarítás
2016. május 11.

## Kompatibilis a magyarítás a Switch-verzóval (New Super Mario Bros. Deluxe)?
**Nem**, és valószínűleg nem is lesz, tekintettel arra, hogy ennek az írásakor (2019.12.04) még nincs Switch-em és egyrészt a Switch-es modolás még babacipőkben jár, másrészt Nintendo bácsi felettébb nehézkessé tette a konzol akármilyen feltörését (ha észrevesznek akármilyen módosítást, legyen az ártatlan homebrew-futtatás, vagy rendes kalózkodás, repülsz).
A magyarítás jelenlegi állapotában a Switch-verzió újításai miatt biztosan nem kompatibilis, és a fent említett okok miatt nem tervezek Deluxe-támogatást (legalábbis egyenlőre).

## Telepítési útmutató
**Megjegyzés:** Mivel csak most, 2019 végén jöttem rá, hogy anno milyen pocsék útmutatót írtam ehhez, és mivel már egy jó ideje nem foglalkoztam Wii U modolással, „kölcsönveszek” és átírok egy másik, frissebb, a Breath of the Wild-hoz írt [útmutatót](https://botw-modding-database.fandom.com/wiki/Mod_Installation_Instructions).

### Mindenekelőtt
Ahhoz, hogy játékokat modolhass egy Wii U-n, először fel kell ahhoz törnöd. Lásd: [Az Útmutatót](https://wiiu.hacks.guide/).

### A szoftverazonosítókról
Mivel a Wii U egy régiózárral rendelkező konzol, a játékok minden régióban különböző szoftverazonosítókkal (Title ID) jelennek meg. Mivel ezt olvasod, valószínűleg magyar vagy, így valószínüleg európai régiújú konzolod és játékod van. Ha mégis bizonytalan lennél, nézd meg a játék lemezét. A képes felén alul van három csoport szöveg. A középső így fog kinézni: `MODEL NO. WUP-006(EUR)`. Ha a zárójelben lévő szöveg **EUR**, akkor európai játékod van, ha **USA** akkor amerikai, illetve ha **JAP**, akkor japán.
A New Super Mario Bros. U szoftverazonosítója `10101x00`, ahol az `x`
- Japánban `C`
- Amerikában `D`
- Európában `E`
**Megjegyzés:** Az SDCafiine-es módszerhez a hosszabb formátumú szoftverazonosítóra lesz szükséged, ami a következő: `0005000010101x00`

### Modok telepítése Wii U-n
Wii U-n három lehezőséged van, ha egy modot akarsz telepíteni. FTPiiU Everywhere, Loadiine GX2, és SDCafiine.
- Használj **FTPiiU Everywhere**-t, ha a játékod a konzolra van telepítve és nem sajnálod felülírni az eredeti fájlokat.
- Használj **Loadiine GX2**-t, ha inkább lemásolnád a játékod, ~~vagy ha Loadiine-os kalóz verziót használsz.~~
- Használj **SDCafiine**-t, ha nem akarod módosítani az eredeti fájlokat és nem sajnálsz mindig futtatni egy programot játék előtt.

### 1. lehetőség: FTPiiU Everywhere
**Figyelmeztetés:** Készíts biztonsági mentést minden fájlról, amit felülírni kívánsz.
**Megjegyzés:** Az FTPiiU Everywhere nem ugyanaz, mint az FTPiiU. Amíg az FTPiiU csak az SD kártyához biztosít hozzáférést, az FTPiiU Everywhere-rel a konzol belső memóriáját is szerkesztheted és erre szükséged is lesz.
**Másik megjegyzés:** Ehhez a módszerhez telepítve kell, hogy legyen a játék a rendszer belső memóriájára.

1. Navigálj ide: `/storage_mlc/usr/title/`
   - Itt három felé ágazik az utunk.
     - A `00050000` mappában a játékok eredeti verzióját találod
	 - A `0005000c` mappában a telepített DLC-ket
	 - A `0005000e` mappában pedig a frissítéseket. A modot frissítésként fogjuk telepíteni, hogy könnyen eltávolítható legyen.
2. Navigálj tovább és másold be az MSBT fájlokat ide: `.../0005000e/10101x00/content/EU/English`
   - **Megjegyzés:** Ha ez a mappaszerkezet nem létezik, hozd létre magad.
   - **Másik megjegyzés:** Ha a Wii U-d nem angolra van állítva, akkor az `English` mappa helyett a rendszered nyelvének megfelelő mappába másold a fájlokat.
3. Kész! Ha jól csináltad, akkor a HOME Menüből indítva a játék magyar nyelven fog elindulni!

### 2. lehetőség: Loadiine GX2
**Megjegyzés:** Ugyan a Loadiine továbbra is kiválóan működik, 2017 óta nem volt új verziója, és manapság kissé elavultnak számít. Csak akkor válaszd ezt a megoldást, ha biztosan így akarsz játszani.
**Másik megjegyzés:** Ehhez a módszerhez szükséged lesz egy Loadiine-formátumú (kicsomagolt) játékra. Vagy másold le a játékot magadnak, vagy szerezd be „ultra-legális módon.”

1. Nyisd meg a játék mappáját és másold be az MSBT fájlokat ide: `/content/EU/English`
   - **Megjegyzés:** Ha a Wii U-d nem angolra van állítva, akkor az `English` mappa helyett a rendszered nyelvének megfelelő mappába másold a fájlokat.
2. Kész! Ha jól csináltad, akkor a Loadiine GX2-ből indítva a játék magyar nyelven fog elindulni!

### 3. lehetőség: SDCafiine
**Megjegyzés:** Ezt a módszert lemezes és telepített játékkal is használhatod.

1. Nyisd meg az SD kártyát és másold be az MSBT fájlokat ide: `sdcafiine/0005000010101x00/content/EU/English`
   - **Megjegyzés:** Ha a Wii U-d nem angolra van állítva, akkor az `English` mappa helyett a rendszered nyelvének megfelelő mappába másold a fájlokat.
2. Kész! Ha jól csináltad, akkor a HOME Menüből indítva a játék magyar nyelven fog elindulni!
