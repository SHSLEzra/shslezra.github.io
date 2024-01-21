---
layout: post
title: "Aegisub használata - az alapok"
categories: [fansub_alapok]
---
Az Aegisub lesz a fő munkaeszközünk fordítás során. Kezdőként ugyanis ezzel fogjuk a forrásvideóból kinyerni a feliratfájlt, ebben fogjuk kicsit beállítani, majd természetesen a feliratot magát is ebben fogjuk lefordítani.

## Aegisub telepítése
Erre a haladóknak szóló útmutatómban egy [egész cikket szenteltem]({% link _posts/2022-10-07-aegisub-verziok.md %}), itt azonban rövidre fogom.  
Két úton indulhatsz el Aegi telepítésével: telepítheted a [hivatalos verziót](https://aegisub.org/) klasszikus módon - kezdőként (illetve fordítóként, lektorként) minden bizonnyal ez is megfelelő lesz.  
Azonban a későbbiekben talán hasznos lehet egy alternatív buildet alkalmazni - ha itt vagy, valószínűleg beszélsz angolul, így nem fog problémát jelenteni [erről az oldalról](https://www.goodjobmedia.com/fansubbing/) az "Aegisub Builds" fül alól
kibányászni az éppen aktuálisan használt verziót. Többnyire ezek is érkeznek telepítővel, de akár portable programként is megtalálhatod néhányukat.

Ha szerencsés vagy, az operációs rendszered magától fel fogja ismerni (esetleg ha telepítővel raktad fel az Aegisubot, akkor magától be fogja állítani, hogy a feliratokat, legyen szó .ass-ről vagy .srt-ről ez nyissa meg).  
Ha ez nem történt meg, akkor állítsd be, hogy így legyen, vagyis az .ass és .srt fájlok alapértelmezett alkalmazása az Aegisbu legyen - amúgy sem kell nagyon mással megnyitnod a feliratokat.

Ezzel meg is volnánk, jöhet a munka!


## Felirat megnyitása

Az általad nyaa-ról letöltött videók általában .mkv formátumban fognak érkezni: ez azt jelenti, hogy videó mellett társítva van egy (vagy több) feliratfájl, nincsenek külön.
Azonban ez nem fog gondot jelenteni nekünk, az Aegisubbal ugyanis könnyedén ki tudjuk nyerni. Menj a Fájl > Feliratfájl megnyítása (angolul: File > Open Subtitles) menüpontra, majd válaszd ki a letöltött .mkv fájlodat.
Ha csak egy feliratfájl van mellé csatolva, azonnal be is tölti. Ha nem, akkor fel fog dobni egy ablakot, hogy melyik verziót kéred: ezek általában elég egyértelműen vannak elnevezve - ahogy azt az alábbi képen is látod.

![Ha több hangsáv is van, ki tudod választani](https://files.catbox.moe/5f09uk.webp)

Ezek után legyen az az első dolgod, hogy a nyers feliratfájlt elmented valamilyen néven. Ez persze bármi lehet, de a kiadásra felkészülve érdemes a közmegegyezés szerint valami hasonló módon elnevezni:
`[csapatnév] Sorozat Címe - RészSzáma (felbontás).ass` - igaz, a felbontás többnyire elhagyható. Íme egy példa az egyik első kiadásomból:

![Az AnimeGun Sub Iwa Kakeru kiadásának fájljai](https://files.catbox.moe/ltvpgb.png)

Ha esetleg nem tudod, mi az az .ass: az Aegisub által használt feliratformátum. Animékhez elhelyezések miatt ezt használják, használd te is nyugodtan.

## A fordítás folyamata

Ezek után jöhet a munka komoly része: a fordítás.  
Ha szeretnéd lefordítani az animét, akkor nem lesz elég a felirat (még ha páran így is gondolják), szükséged van a videóra is.
Szerencsére nincsen semmi probléma - fájlkezelőből csak simán húzd rá az Aegisubra a videót, és be is fogja tölteni. Ezzel el is érkezett az ideje annak, hogy megtanuljuk a programot használni. Íme a néhány legfontosabb eszköz:

![Az Aegisub legfontosabb eszközei](https://files.catbox.moe/end9c3.webp)

Nézzük is sorrendben őket.
- Lila: különféle egyszerűbb szövegelhelyezésekre - hely, forgatás, láthatóság - alkalmas eszközök.
- Piros: videólejátszó gombjai. Az első egy sima stop/start, a másodikkal a kijelölt feliratsort játssza le, a harmadik a pause.
  A negyedik egy kapcsoló: ha be van nyomva, mindig annak a sornak az elejére ugrik, amelyiket kijelölöd (szubjektív vélemény: érdemes kikapcsolni).
- Kék: a felirat formázásának eszközei: stílusok és színek állítására vannak. Fölötte találod a sornak az időkódjait, melyet a mellette található Time / Frame kapcsolóval videó ideje vagy képkockájának száma szerint nézhetsz.
- Narancs: a feliratok időzítéséhez használt eszközök az alábbi sorrendben: előző/következő sorra való ugrás; adott szakasz és adott sor lejátszása (nincs jelentősége itt);
  sor előtti 500 ms, sor első 500 ms, sor utáni 500 ms és sor utolsó 500 ms lejátszása. A többire még nem lesz szükséged.
- Zöld: CPS, azaz character per second (egy másodpercre jutó karakterszám) indikátor. Később említeni fogom.

Alapvetően két módon fordíthatod a feliratot: beírhatod az angol (vagy adott esetben más nyelvű) eredeti szöveg helyére a fordításodat;
vagy ha szeretnéd később még ellenőrizni (esetleg mással dolgozol), akkor az angolt kapcsos zárójelek {} közé rakhatod, majd beírhatod utána a magyart. Ilyenkor az angol csak a feliratfájl megnyitásakor fog látszani.


## Az .ass formátum előnyei

Kezdőként (szerintem) a leghasznosabb funkciója az .ass-nek a megjegyzések írása.  
Ezt ugyan már említettem fentebb, de álljon itt is: a {kapcsos zárójelbe tett szöveg} **nem fog látszani** a nézőnek; csupán annak, aki azt megnyitja.  
Ennek két fő alkalmazási módja az eredeti felirat megtartása a fordításban, illetve különféle megjegyzések - alternatív fordítási lehetőség, kérdés, amire adott esetben szükséged van.

Itt egy példa a felirat felépítésére:

![Egy .ass felirat felépítésére példa](https://files.catbox.moe/b0qtiy.png)
A sárga résszel kiemelt rész egy úgynevezett "tag" (erről mindjárt beszélünk); a sötétzöld az eredeti szöveg, míg a cián egy megjegyzés - adott esetben alternatív fordítási javaslat.


Szóval, mik is ezek a tagek?  
Ezek segítségével tudod a feliratodat formázni. A legtöbb (alapot) a felső eszközök használatával rá tudod tenni a feliratra (és érdemes is inkább azokat használni), de álljanak itt a dialógusok formázásához szükségesek, ha a gépelést pártolnád:
- {\i1}*dőlt szöveg*{\i0}
- {\b1}**félkövér szöveg**{\b0}
- bár animékben nem használt, de: {\s1}~~áthúzott szöveg~~{\s0}
- szintén: {\u1}__aláhúzott szöveg__{\u0} (a markdown ezt sajnos nem jeleníti meg)
Természetesen több tag együttes alkalmazása is lehetséges: a {\b1}{\i1}***félkövér és dőlt szöveget***{\b0}{\i0} fog adni. A tagek sorrendje nem számít.  
Ahogy azt a megjegyzésekhez is írtam, lehetséges sorok közepére, akár szavak közé is tageket illeszteni, ha éppen így kívánná meg a szükség.

Ezen kívül amit mindenképpen tudni szükséges, azok a különféle tördelési formák.  
Fontos, hogy esetükben **nincs szükség {}-re**! Programozásból ismerős lehet, de álljanak itt:
- A legjelentősebb a \N - ez egy klasszikus sortörés
- Ezen kívül használjuk még a \h-t, ez egy hosszú szóköz (ha a font tartalmaz ilyet) - ne használd dialógusokban, inkább címeknél, elválasztásoknál

Hogy röviden illusztráljam az összes gyakran alkalmazott tag alkalmazását, íme egy rövid példa:

![Ami így jelenik meg...](https://files.catbox.moe/omypui.png)

![...az így néz ki a feliratkezelőben](https://files.catbox.moe/33k5x3.png)

### Mikor és hogyan használjuk ezeket?
Ezen eszközök ügyes használatáról majd egy későbbi cikk fog szólni, de néhány alapot megjegyeznék:
- Sortörést mindenképpen érdemes alkalmazni hosszabb soroknál; ha nincs ötleted, hol, akkor legalább ott, ahol azt a program alapból eltöri
- Dőlt szöveget általában belső gondolatokra vagy valamilyen szó/kifejezés *kiemelésére* használjuk
- Ez utóbbi célra elfogadható a félkövér is, ha jól néz ki
- Hacsak nem muszáj, ne használj aláhúzott és áthúzott szöveget - de párbeszédben ***semmiképpen!***


## Videó automatikus betöltése

Ha nem egyedül dolgozol, tovább kell majd küldened a fájlt valakinek. Ehhez (jobb esetben) nem szükséges a videót is társítani (hiszen a társad is le tudja tölteni nyaa.si-ról), hanem csupán egy néhány kilobájtos fájlt átdobhatsz neki.  
De ha csak te fordítasz, akkor is szükséged lehet arra, hogy ismételten megnyisd a feliratot.

Amikor megnyitsz Aegisubbal egy feliratot, akkor a legutóbbi videót megpróbálja automatikusan betölteni hozzá - ehhez fel is fog kínálni egy ablakot, valami ilyesmit:

![Automatikus videóbetöltés](https://files.catbox.moe/paln0k.png)

Alap esetben az Aegisub a munkakönyvtár segítségével tárolja el a videó helyét, ha van rá lehetősége. Ha máshol tárolod a videót, mint a feliratot, akkor teljes útvonalat fog elmenteni.  
Ez azért jelentős, mert áthelyezés esetén (vagy ha valaki más nyitja meg utoljára) rossz helyen fogja keresni, és a betöltés hibára fog kifutni.
Természetesen nem kell ilyenkor aggódni - okézd le a hibaüzenetet, majd húzd rá a videót, mintha mi sem történt volna.