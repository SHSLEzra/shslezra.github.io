---
layout: post
title: "Aegisub verziók: mi a különbség, és kinek fontos?"
categories: [fansub]
---

Kezdjük egyből az elején: *mégis milyen verziók lennének?*

A legfrissebb hivatalos verzió a [3.2.2](https://github.com/Aegisub/Aegisub), ami 2014 decemberében lett kiadva. Beláthatjuk, hogy talán vannak lemaradásai.


Szerencsénkre azonban az Aegisub nyílt forráskódú program - azaz gyakorlatilag bárki belenyúlhat, és csinálhat vele valamit.

A külföldi fansubberek egy része pedig pont ezt csinálta. Van egy csomó fajta, én most csak azt a kettőt emelném ki, amivel volt szerencsém dolgozni.


Az egyik [Plorkyeran buildje](http://plorkyeran.com/aegisub/), azonban pár éve ennek a fejlesztése is leállt.

~~A másik pedig a külföldön széles körben elterjedt [Daydream Café](https://github.com/Ristellise/AegisubDC), röviden AegisubDC.~~

~~(Itt szeretnék megemlíteni egy harmadikat is: [arch1t3cht buildjét](https://github.com/arch1t3cht/Aegisub), amelyik jelenleg aktívan fejlesztés alatt áll.)~~

Jelen állás szerint a fenti, arch1t3cht által készített változat a “legfrissebb”, azonban hogy a cikk némileg jövőálló legyen: a Good Job! Media oldalán a [Fansubbing](https://www.goodjobmedia.com/fansubbing/) részen megtalálható az éppen aktuálisan legelterjedtebb verzió.


Akkor térjünk vissza a címben feltett kérdésre.

## Mi a különbség ezek és a 3.2.2 között?

Egyrészt a fentiekben már benne van a libass (melyről a rendererekről szóló cikkben lesz részletesen szó). Egyelőre maradjunk annyiban, hogy fontos.

Másrészt pedig egy csomó apró újítás van, amik hasznosak lehetnek (ismét a formázóknak) - fontok betöltése, vektoros eszközök pontossága, beépített [Dependency Control](https://github.com/TypesettingTools/DependencyControl), video panning.


Persze nem akarom én megmondani, hogy ki milyen verziót használjon, de van pár dolog, amit mindenképpen érdemes figyelembe venni, akár saját buildet készítesz (franc tudja, minek), akár keresel valamit.
- ***legyen benne libass*** (lehetőleg a legfrissebb)
- legyen támogatott a DependencyControl (ugyanis sok script már alapból csak ennek segítségével működik)
- ezen kívül nem árt, ha vannak benne munkát megkönnyítő apróságok, de ez már személyes preferencia
- és szintén nem árt, ha aktívan frissített

Ez a cikk ennyi lenne. Azok, akik úgy döntöttek, hogy az újabb verziók közül választanak, de problémába ütköztek: a további rész nektek szól.


## Telepítési problémák

Külföldön (szinte) senki nem ütközik problémákba a telepítés során, a magyarok valahogy folyamatosan (főleg a Daydream Cafénál, de máshol is előfordulhat). Ilyenkor általában a Plorkyeran-féle buildeket használják, azok ugyanis telepítősek.
Ha mégis maradnál ezeknél, pár ötlet (visszatekerhetsz olvasni [MFK-n](https://discord.com/channels/939496117865943060/939497236998537246/940656798157914173) is, csak hogy lásd, milyen sok probléma adódik vele):
- Sok script és program nem szereti az ékezetes betűket (és a szóközöket sem igazán). Mivel ezek “hordozható” programok, gyakorlatilag bárhová telepítheted. Nekem például `D:\AegisubDC\` mappában van, ezzel nagy gond nem lehet.
- Ha a Windowsos felhasználónevedben van speciális karakter, a fenti lépés kifejezetten javallott.
- Ha a gép nevében van speciális karakter, az elvileg nem zavarja meg a programot. Gyakorlatilag pedig nem tudhatjuk. Ha van rá lehetőséged, próbáld ki egy virtuális gépen, vagy egy másikon, ahol nincs benne.
- Ha Program Filesba telepítetted, lehet, hogy valamihez nem fér hozzá.
- Ha korábban telepítettél bármilyen más Aegit (és valószínűleg megtetted), a kettő összeakadhat. Ha minden kötél szakad, egy biztonsági mentés után (scriptek, személyre szabások stb.) megpróbálhatod törölni mindkettőt, majd újratelepíteni az újat.
- Végül pedig maradnak más verziók és/vagy imádkozás az égiekhez, hogy mégis működjön. Más verzió választásához nézd a fenti rövid útmutatót.