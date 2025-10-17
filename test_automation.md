# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

## A tesztelés alapjai:
#### Mi a tesztelés célja? Mi nem az?
Nem az a célja, hogy bebizonyítsa, hogy a rendszert hibátlan, hanem éppen ellenkezőleg, hogy felfedje a hibákat, minél korábban, és csökkentse azok javításának költségeit
#### Mi a kapcsolat a tesztelés és a hibamegelőzés között?
A tesztelés nemcsak a hibák megtalálását, hanem azok megelőzését is szolgálja.
A hibák elemzése (pl. miért keletkeztek, hol fordulnak elő leggyakrabban) segíthet a folyamatokat javítani, így a jövőben kevesebb hiba keletkezik.
#### Miért fontos, hogy a tesztelők függetlenek legyenek a fejlesztőktől?
A független tesztelő objektívebben látja a rendszert.

Nem befolyásolja az a tény, hogy ő maga írta a kódot.

Könnyebben észreveszi azokat a hibákat, amiket a fejlesztő már „megszokott”.
#### Mi a veszélye annak, ha a fejlesztő maga teszteli a saját kódját?
Hajlamos elnézni a saját hibáit („ez biztosan jól működik”).

Olyan teszteket ír, amelyek a várt működést igazolják, nem pedig a hibás eseteket keresik.

Ez csökkenti a tesztelés hatékonyságát.
#### Mik a tesztelési alapelvek?
1. A tesztelés azt mutatja, hogy vannak hibák.
2. A kiterjedt tesztelés lehetetlen.
3. Korai tesztelés, a fejlesztési folyamat korai szakaszában.
4. Hiba a fürtözésben, keressen érzékeny helyeket.
5. Paradox peszticid, ne ismételje meg ugyanazt a tesztet.
6. A tesztelés kontextustól függ.
7. A hibák hiányának nem kell helyesnek lennie.

#### Mit jelent az „alapvető tesztelési elv”, hogy „a kimerítő tesztelés lehetetlen”?

#### Mit jelent az „alapvető tesztelési elv”, hogy „a hibák halmozódnak”?

#### Mit jelent az „alapvető tesztelési elv”, hogy „a tesztelés a kontextustól függ”?



## 2. Tesztelés a szoftverfejlesztés életciklusán át
#### Mik a tesztszintek, és mi a különbség köztük?
Egységteszt (Unit test): Kisebb kódrészletek (függvények, osztályok) tesztelése.

Integrációs teszt: A komponensek együttműködését ellenőrzi.

Rendszerteszt: Az egész rendszert egyben vizsgálja.

Felhasználói elfogadási teszt (UAT): Ellenőrzi, hogy a rendszer megfelel-e az üzleti igényeknek.
#### Miért nem érdemes mindig ugyanazokat a teszteseteket futtatni (regressziós torzítás)?
Ha mindig ugyanazokat a teszteket futtatjuk, új hibák rejtve maradnak – a tesztkészlet „elavul”.
Ez a peszticid paradoxon is: a tesztelés hatékonysága csökken, ha nem frissítjük a teszteseteket.
#### Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Az egységteszt a legkisebb programrészek (függvények, metódusok) automatikus tesztelése.

A fejlesztők írják és futtatják.

Cél: minél hamarabb kiszűrni a hibákat a kódban.
#### Mi a különbség a verifikáció és a validáció között?
Verifikáció: „Jól építjük?” – megfelel-e a rendszer a specifikációnak.

Validáció: „A jót építjük?” – megfelel-e a rendszer a felhasználói igényeknek.
Példa:
Verifikáció: A bejelentkezés működik jelszóval.
Validáció: A bejelentkezés folyamata tényleg a felhasználó számára kényelmes és érthető?
#### Mik a tesztelési típusok, és mi a különbség köztük?
Funkcionális teszt: Ellenőrzi, hogy a funkciók helyesen működnek.

Nem funkcionális teszt: Teljesítmény, biztonság, használhatóság stb.

Regressziós teszt: Megnézi, hogy a módosítások nem rontottak-e el más részeket.

Smoke teszt: Gyors alapellenőrzés, hogy a rendszer „él-e”.
#### Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
Fehér doboz:	Ismeri a tesztelő kódot	Belső logika, vezérlési ágak tesztelése
Fekete doboz	Nem ismeri a tesztelő a kódot	Csak bemenet–kimenet vizsgálat
Szürke doboz	Részben	Ismeri a belső működés egy részét, de a tesztelés kívülről történik
#### Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?

#### Mi a különbség a statikus és dinamikus tesztelés között?