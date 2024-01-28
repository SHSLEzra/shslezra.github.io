---
layout: post
title: "Aegisub beállítások"
categories: [fansub, formazas]
chapter: 1
author: Ezra
---
Ahhoz, hogy rendesen tudj formázni (esetleg ellenőrzini, időzíteni, karaoket készíteni stb.), szükséged lesz egy rendesen beállított Aegire. Egyrészt az általa nyújtott funkciók, másrészt a kényelem és gyorsaság miatt.

Nem fogom az egész beállítások fület végigmutatni, csak néhány fontosabbat.

**Beállítások megnyitása: Alt+O (alapból), vagy View > Options.**


## Színek (“dark mode”)
Az Aegisubban nincs sötét mód (legalábbis *jelenleg* a legtöbb verzióban nincs; ez változhat). Ez van, ezzel kell együtt élnünk.  
Azért addig sem kell kiégetnünk a szemünket, ugyanis a színeket, bár egyesével, de át tudjuk állítani. Ez persze jól jöhet azoknak is, akik más logika alapján akarnak dolgozni, esetleg színvakoknak (bár nekik a formázás valószínűleg kiesik).

![A színek beállítása](https://files.catbox.moe/cwa8ce.png "(Az ablak sötét módjáért a Linux téma felelős)")

Ezek az alap beállítások. Hát most na, nem szeretek nagyon variálni. 

(Tényleges) sötét módhoz az összes feketét valami világos színre, az összes fehéret pedig valami neked tetsző sötét színre kell színezni. Ha másra nem is, arra jó ez, hogy mondjuk ki tudd emelni a megjegyzéseket.


## Gyorsgombok
Evezzünk fontosabb vizekre. Hotkeyek, gyorsgombok beállítása.

![A hotkey menü alapból](https://files.catbox.moe/d774fm.png)

Ahogy látjátok, különféle kategóriákba tudjátok besorolni a hotkeyeket.  
A “Default” és az “Always” gyakorlatilag ugyanazt jelenti: bárhol is vagy az Aegin belül, azt érzékeli.  
Személy szerint nem szívesen pakolok ide, mert alapvetően Ctrl+valami vagy Shift+valami hotkeyeim vannak, és a Shiftesek kellemetlenek tudnak lenni, ha akkor is aktiválódnak, amikor gépelek.

Az “Audio” csak az audiosávnál működik, a “Video” csak a videón állva, nyilván a többi is egyértelmű.

Új hotkey hozzáadásához válaszd ki, hova szeretnéd adni, majd nyomj a New gombra. Ezek után nyomd le a (maximum három gombból álló) billentyűkombinációdat, majd kattints ki a keretből.
Ezek után kattints bele a “Command” alatti részbe, ahol beírhatod, mit akarsz vele előhozni.  
Törléshez a “Delete”, módosításhoz pedig az “Edit” gomb használandó, természetesen.

![Új hotkey hozzáadása](https://files.catbox.moe/9bv79i.png "A pan_reset Ctrl+Í alatt van nekem, ezt viszont sajnos valamiért nem jeleníti meg - ezért a Ctrl- kiírása")

**Fontos: nem csak beépített funkciókat tudsz beállítani (mondjuk `audio/play/selection/after`), hanem egyes scripteket is.** Ezeket úgy éred el, ha elkezded gépelni, hogy `automation/lua/`, és ki fogja dobni.


## Hangbeállítások
Tulajdonképpen az időzítés finomhangolására alkalmas fül.

![Az audiófül](https://files.catbox.moe/35p1sd.png "Többnyire szintén az alapbeállítások láthatók")

Mint ahogy az előzőek, ezek is tulajdonképpen egyéni preferencia kérdései. Két javaslat:
- A pirossal bekeretezett négyzet (kulcskockákhoz való snapelés) mindenképpen legyen benyomva.  
- A kékkel jelölt alapértelmezett lead-in/lead-out valami hasonló értéken legyen, de úgyis tudjátok állítani TPP-ben később *(vagy elfelejthetitek akár a használatát is)*.


## Renderer beállítása
Talán az egyik legfontosabb beállítás az Aegin belül.  
Advanced > Video alatt találod, Subtitles provider néven egy lenyíló menüben.

![Renderer beállítása](https://files.catbox.moe/eykfdx.png)

Ha újabb verziót használsz az Aegisubból (értsd: nem 3.2.2), valószínűleg már alapértelmezetten a libass van beállítva (sőt, az is előfordulhat, hogy más opció nincs is). De sosem árt ellenőrizni.



Talán mondanom sem kell, de érdemes lecsekkolni az összes többi beállítást, hogy minden úgy működjön, ahogy az számodra a legkényelmesebb, leghatékonyabb.
Érdemes tudni például az automata mentés helyét is (adott esetben meg is változtatni), nem egyszer mentett már meg.