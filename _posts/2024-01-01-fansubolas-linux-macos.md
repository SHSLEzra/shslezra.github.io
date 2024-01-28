---
layout: post
title: "Fansubolás Windowson kívül: mivel?"
categories: [fansub, fansub-tippek]
tags: [technikai]
chapter: 99
author: Ezra
---

Az elmúlt időben egyre több embert láttam, akik MacOS vagy Linux rendszeren szerettek volna fordításokat készíteni.


Korábban nem kifejezetten tudtam volna mit hozzászólni a témához, de nemrégiben én is váltottam, így pedig muszáj voltam megismerni, mégis milyen (alternatív) megoldások kínálkoznak. Ebben a cikkben ezeket fogom röviden ismertetni.


## Aegisub

Talán ezzel van a legkönnyebb dolgunk: az Aeginek Linuxra és MacOS-re is van elérhető változata.

Jelen állás szerint [arch1t3cht kiadását](https://github.com/arch1t3cht) érdemes telepíteni: ebben van többféle Windows változat mellett egy AppImage Linuxra és egy MacOS telepítő.
Fontos megjegyezni, hogy ezekben azonban **NINCS beépített DependencyControl**, mely a legtöbb scripthez manapság már szükséges: ezt [innen](https://github.com/TypesettingTools/DependencyControl) lehet beszerezni (telepítési útmutató szitén a linken).


## Mocha

A Mochának leggyakrabban használt alternatívája a [Blender](https://www.blender.org/) - sokan még Windowson is használják, mert a lekövetési technikája máshogy működik, ráadásul teljesen ingyenes.
PhosCity készített egy [újabb leírást](https://fansubbers.miraheze.org/wiki/User:PhosCity/Blender_Motion_Tracking_for_Fansubbing) a használatáról; de a "klasszikus" is megtalálható [ezen a linken](https://subarashii-no-fansub.github.io/Subbing-Tutorial/Tracking-Motion/).


## Adobe Illustrator

Általánosan az [Inkscape](https://inkscape.org/) alkalmazás az, amivel helyettesíteni szokás az Adobe Illustratort.
Jelen tudásom szerint némi kényelmetlenség itt is adódik, akárcsak az Aegisub esetében: az Illustrator scriptjével szemben itt ki kell mentenünk a képet .svg formátumba,
majd az [Svg2ass program](https://github.com/irrwahn/svg2ass) (webes változat [itt](https://qgustavor.github.io/svg2ass-gui/)) vagy az SVG2ASS script ([itt](https://phoscity.github.io/Aegisub-Scripts/svg2ass/) vagy DependencyControlban) segítségével átalakítani .ass formátumba.


*(Egy rövid kitérőt tennék: ahogy az SVG2ASS script után kutattam, feltűnt egy utalás egy bizonyos tophf által készített scriptre, ami alapján mintázták az Adobe Illustratorhoz készült scriptet.
Ezt CorelDRAW-hoz írták; azonban a scriptet magát nem találtam meg, és a program egyébként is csak MacOS-re és Windowsra érhető el, Adobe programhoz hasonló áron. De egy említést talán megérdemel.)*


## Adobe Photoshop

A Photoshop egyik gyakori alternatívája a [Gimp](https://www.gimp.org/), amely hasonlóan a Blenderhez, sok esetben még Windows felhasználók által is alkalmazott.


A szerintem legszimpatikusabb, azonban valamivel ritkább program a [Darktable](https://www.darktable.org/install/) – ritkaságának köszönhetően kevesebben használják, azonban ha valaki képek szerkesztésére is használni akarja, talán ezzel jobban jár.


Egy másik, azonban csak MacOS-re elérhető program a [MediBang Paint Pro](https://medibangpaint.com/en/app-download/).


## Egyéb programok

Ezek azok, amik nem kifejezetten jelentősek, de említést mindenképpen érdemelnek:

- Égető: [ffmpeg](https://ffmpeg.org/download.html) használatával nem lehet félrelőni
- Videólejátszó: [mpv](Fansubolás Windowson kívül: mivel?) is elérhető minden platformra
- Fontkezelő: én [ezt](https://github.com/FontManager/font-manager) használom; a [FontBase](https://fontba.se/) viszont talán jobb választás
- Fontszerkesztő: [FontForge](https://fontforge.org/en-US/downloads/) (egyelőre még nem próbáltam ki)
