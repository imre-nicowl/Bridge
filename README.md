# **BRIDGE SZABÁLYOK**

*(SAYC nyomán)*
**Szerzők:** Jánoki Imre és Uhrin Ákos
**Verzió:** r3.1
**Eredeti:** 2023.07.03. (r1.0)
**Utolsó revízió (r1.8)** 2025.09.17.
**Átszerkesztve, bővítve (r3.0):** 2026.05.12.
**Konvenció-bővítések (r3.1):** 2026.05.12.

> 💡 **Mi változott a r1.8 → r2.0 között?**
Struktúrális változás a Google Docsban, ami alapjául szolgált a jelen markdownnak.

> 💡 **Mi változott a r2.0 → r2.1 között?**
> - Ellentmondások, inkonzisztenciák fixálva: game prémium, negatív double nemes szín hossza kérdés, 1NT->4NT kvantitatív, Stayman kiegészítés (Garbage Stayman, Smolen), Kickback választva (vs minorwood), gyenge 2-es vs rule of 20
> - Kidolgozott részek: exclusion Blackwood szöveges magyarázat, 5NT királykérdés Kickbackkel, power double részletes ágak, újranyitó kontra leírás, Cappelletti viszontválaszok
> - Új tartalmak: Bergen raises (2/1 rendszer szerves része), Western Cue bid stopper, Unusual vs Unusual védekezés, 1NT semi-forcing, Drury (passzolt segítő), Reverse bidding fejezet (2/1)

> 💡 **Mi változott a r2.1 → r3.0 között?**
> - Konzisztens belső linkek a teljes dokumentumban a könnyebb navigációhoz.
> - Új [**Gyorskereső táblázat**](#gyorskereső-játék-közben) játék közbeni döntéstámogatáshoz.
> - Új nagy fejezet: [**Lejátszási taktikák**](#lejátszási-taktikák) – endplay, squeeze családok (strip squeeze-szel együtt), coup-ok, avoidance, safety play, hold-up, communication, counting – részletes példákkal.
> - Bedolgozva: [LTC és Zar Points](#lapérték-finomítás--ltc-és-zar-points), [Cuebid kontrollok](#cuebid--első--és-másodkörös-kontrollok), [Gyakori licitálási hibák](#gyakori-licitálási-hibák--anti-pattern-szekció), [Példa licitsorozatok](#példa-licitsorozatok-minden-főbb-konvencióhoz).
> - Pótolva a hiányzó pontozási sorok (kontrázott / rekontrázott bukás).
> - A hivatkozott, de korábban üres szekciók kapnak vagy magyarázó szöveget, vagy explicit ábra-placeholdert.

> 💡 **Mi változott a r3.0 → r3.1 között?**
> - **Erős 2♣ feltételek pontosítása:** 22+ HCP balanced **vagy** 19+ HCP + 9+ playing trick (eloszlásos). A korábbi „17 HCP" küszöb javítva minden helyen (induló-táblázat, részletes szekció, Gyorskereső).
> - Új: [Crawling (Creeping) Stayman](#crawling-creeping-stayman-konvenció) — gyenge kézzel 1NT-ből menekülés 4-4 nemes-fittel.
> - Új: [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) — 4+ adu + 10+ HCP take-out double után.
> - Új: [Az ellenfél kontrázott — ez **is** közbeszólás](#ellenfél-kontrázott--ez-is-közbeszólás) — explicit struktúra (direct raise / jump raise / Jordan 2NT / XX) takeout double után.
> - Bergen Raises vs. Mixed Raise distinkció kifejtve a Mixed Raise szekcióban.

## Tartalomjegyzék

- [**BRIDGE SZABÁLYOK**](#bridge-szabályok)
  - [Tartalomjegyzék](#tartalomjegyzék)
  - [Bridge alapok](#bridge-alapok)
    - [Pontok (HCP – High Card Points)](#pontok-hcp--high-card-points)
    - [Eloszlási (többlet) pontok](#eloszlási-többlet-pontok)
    - [Lapérték-finomítás – LTC és Zar Points](#lapérték-finomítás--ltc-és-zar-points)
      - [**Losing Trick Count (LTC) – Veszítendő ütések száma**](#losing-trick-count-ltc--veszítendő-ütések-száma)
      - [**Zar Points (Zar Petkov rendszere)**](#zar-points-zar-petkov-rendszere)
    - [Színek rangsora](#színek-rangsora)
    - [Nemes szín preferencia (segítőként)](#nemes-szín-preferencia-segítőként)
    - [Licitálási szintek (a partnerség két kezében összesen)](#licitálási-szintek-a-partnerség-két-kezében-összesen)
  - [Az Induló szabályai (az első, aki nem passzol)](#az-induló-szabályai-az-első-aki-nem-passzol)
    - [Első licit](#első-licit)
    - [Általános irányelvek](#általános-irányelvek)
    - [Induló licitek – részletes táblázat](#induló-licitek--részletes-táblázat)
    - [The Rule of 20](#the-rule-of-20)
    - [The Rule of 44](#the-rule-of-44)
    - [Az induló viszontválasza (miután a partner válaszolt – nem passzal)](#az-induló-viszontválasza-miután-a-partner-válaszolt--nem-passzal)
  - [A Segítő szabályai (miután az Induló megnyitotta a licitet)](#a-segítő-szabályai-miután-az-induló-megnyitotta-a-licitet)
    - [Semi-forcing 1NT (1M – 1NT)](#semi-forcing-1nt-1m--1nt)
    - [A) Első válasz – ha az ellenfél NEM szólt közbe](#a-első-válasz--ha-az-ellenfél-nem-szólt-közbe)
      - [Áttekintő táblázat](#áttekintő-táblázat)
      - [Inverted minor (csak nem nemes nyitásra)](#inverted-minor-csak-nem-nemes-nyitásra)
      - [Az induló viszontválaszai inverted minor sima emelés után](#az-induló-viszontválaszai-inverted-minor-sima-emelés-után)
      - [Jacoby 2NT (segítőként, csak nemes nyitásra)](#jacoby-2nt-segítőként-csak-nemes-nyitásra)
      - [Bergen Raises](#bergen-raises)
    - [B) Első válasz – ha az ellenfél KÖZBESZÓLT](#b-első-válasz--ha-az-ellenfél-közbeszólt)
      - [Az ellenfél kontrázott — ez **is** közbeszólás](#ellenfél-kontrázott--ez-is-közbeszólás)
      - [Negatív kontra – a Standard SAYC (B konvenció)](#negatív-kontra--a-standard-sayc-b-konvenció)
      - [Kevert emelés (Mixed Raise)](#kevert-emelés-mixed-raise)
      - [Jordan 2NT (4+ fit + 10+ HCP take-out double után)](#jordan-2nt-4-fit--10-hcp-take-out-double-után)
  - [Válaszok az 1NT vagy 2NT indulásra](#válaszok-az-1nt-vagy-2nt-indulásra)
    - [A) Segítő válaszai 1NT indulásra (közbeszólás nélkül)](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül)
      - [Stayman, Smolen és Garbage Stayman konvenciók (1NT → 2♣)](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2)
      - [Crawling (Creeping) Stayman konvenció](#crawling-creeping-stayman-konvenció)
      - [Puppet Stayman konvenció (1NT → 3♣ vagy 2NT → 3♣)](#puppet-stayman-konvenció-1nt--3-vagy-2nt--3)
      - [Jacoby transzfer I. és II. (1NT → 2♦ kőrre, 1NT → 2♥ pikkre)](#jacoby-transzfer-i-és-ii-1nt--2-kőrre-1nt--2-pikkre)
    - [B) Válaszok 1NT indulásra, ha az ellenfél közbeszólt](#b-válaszok-1nt-indulásra-ha-az-ellenfél-közbeszólt)
      - [Az ellenfél kettes szinten szólt közbe – kontra](#az-ellenfél-kettes-szinten-szólt-közbe--kontra)
      - [Lebensohl 1NT közbeszólás ellen](#lebensohl-1nt-közbeszólás-ellen)
  - [Válasz a gyenge 2-esre](#válasz-a-gyenge-2-esre)
    - [A) Válaszok közbeszólás nélkül](#a-válaszok-közbeszólás-nélkül)
      - [OGUST – válaszok az induló kérdésére (2♥ → 2NT → ?)](#ogust--válaszok-az-induló-kérdésére-2--2nt--)
    - [B) Válaszok közbeszólás esetén – Lebensohl gyenge 2-es ellen](#b-válaszok-közbeszólás-esetén--lebensohl-gyenge-2-es-ellen)
  - [Erős 2 treff indulás](#erős-2-treff-indulás)
    - [Válaszok a 2♣ indulásra (2♣ → ?)](#válaszok-a-2-indulásra-2--)
    - [Az induló viszontválaszai a 2♦ negatív válaszra (2♣ → 2♦ → ?)](#az-induló-viszontválaszai-a-2-negatív-válaszra-2--2--)
    - [Az induló viszontválaszai a 2♥ dupla negatív válaszra (2♣ → 2♥ → ?)](#az-induló-viszontválaszai-a-2-dupla-negatív-válaszra-2--2--)
    - [Egyéb megfontolások az erős 2 treff után](#egyéb-megfontolások-az-erős-2-treff-után)
  - [2/1 Game Forcing és Reverse Bidding](#21-game-forcing-és-reverse-bidding)
    - [2/1 Game Forcing (Kettő az egyre Game Force)](#21-game-forcing-kettő-az-egyre-game-force)
    - [Reverse Bidding (Fordított licit)](#reverse-bidding-fordított-licit)
  - [Slamkereső konvenciók](#slamkereső-konvenciók)
    - [Kickback (helyett 4NT!) – Roman Key Card Blackwood (RKC) ászkérdés – 1430](#kickback-helyett-4nt--roman-key-card-blackwood-rkc-ászkérdés--1430)
    - [Exclusion Blackwood](#exclusion-blackwood)
    - [Void válaszok 1430-ban](#void-válaszok-1430-ban)
    - [5NT Specific King Ask (Királykérdés Kickback után)](#5nt-specific-king-ask-királykérdés-kickback-után)
    - [Adu dáma megkérdezése RKC-ra érkezett válasz után](#adu-dáma-megkérdezése-rkc-ra-érkezett-válasz-után)
    - [Gerber (szanra adott) ász- és királykérdés](#gerber-szanra-adott-ász--és-királykérdés)
    - [Ha közbeszóltak az ászkérdésre – DEPO](#ha-közbeszóltak-az-ászkérdésre--depo)
    - [Cuebid – első- és másodkörös kontrollok](#cuebid--első--és-másodkörös-kontrollok)
  - [Overcallok és kompetitív licitek](#overcallok-és-kompetitív-licitek)
    - [Áttekintő pont-diagram](#áttekintő-pont-diagram)
    - [Szín bemondása (overcall)](#szín-bemondása-overcall)
    - [Take-out Double](#take-out-double)
    - [1NT és 2NT overcall](#1nt-és-2nt-overcall)
    - [Power Double (Erős Kontra, 16+ HCP)](#power-double-erős-kontra-16-hcp)
    - [Take-out Double 4-es magasan](#take-out-double-4-es-magasan)
    - [Újranyitó kontra (Reopening Double)](#újranyitó-kontra-reopening-double)
    - [Support Double](#support-double)
    - [Two-suited Double](#two-suited-double)
    - [Negatív kontra (overcaller partnereként)](#negatív-kontra-overcaller-partnereként)
    - [Rekontra (erős)](#rekontra-erős)
    - [Gyenge 2-re adott takeout double után – Lebensohl relay](#gyenge-2-re-adott-takeout-double-után--lebensohl-relay)
    - [Michael's Cue bid + Unusual 2NT vs. Védekezés (Unusual vs Unusual)](#michaels-cue-bid--unusual-2nt-vs-védekezés-unusual-vs-unusual)
    - [Védekezés 1NT indulás ellen – Cappelletti](#védekezés-1nt-indulás-ellen--cappelletti)
  - [Egyebek – egyéb konvenciók](#egyebek--egyéb-konvenciók)
  - [Ellenjáték (jelzések)](#ellenjáték-jelzések)
    - [Attitude (upside-down)](#attitude-upside-down)
    - [Count (upside-down)](#count-upside-down)
    - [Suit-preference](#suit-preference)
  - [Slem- és game-erő megbeszélése](#slem--és-game-erő-megbeszélése)
    - [The Law of Total Tricks](#the-law-of-total-tricks)
    - [Drury Konvenció (Passzolt segítővel)](#drury-konvenció-passzolt-segítővel)
    - [Western Cue bid (Stopper-kérés)](#western-cue-bid-stopper-kérés)
    - [Splinter bids](#splinter-bids)
    - [Fourth suit forcing (Negyedik szín forcing)](#fourth-suit-forcing-negyedik-szín-forcing)
  - [Pontozás](#pontozás)
    - [Sebezhetőség (vulnerability) – licitkezdő szerint](#sebezhetőség-vulnerability--licitkezdő-szerint)
    - [Ütésenkénti pontok](#ütésenkénti-pontok)
    - [Bónuszok teljesítésért (mans / bell)](#bónuszok-teljesítésért-mans--bell)
    - [Bukás ütésenként](#bukás-ütésenként)
    - [Kontra hatása](#kontra-hatása)
    - [Rekontra hatása](#rekontra-hatása)
  - [Játékmenet alapok](#játékmenet-alapok)
    - [Impassz (finesse)](#impassz-finesse)
    - [Hogyan nyitunk](#hogyan-nyitunk)
    - [Osztás és lejátszás](#osztás-és-lejátszás)
- [🎴 Lejátszási taktikák](#-lejátszási-taktikák)
  - [Endplay (kényszerkijátszás)](#endplay-kényszerkijátszás)
    - [Példa endplay (egyszerű, klasszikus)](#példa-endplay-egyszerű-klasszikus)
  - [Squeeze – általános alapelvek](#squeeze--általános-alapelvek)
    - [Alapfeltételek (BLUE-CASH-szerű mnemonika)](#alapfeltételek-blue-cash-szerű-mnemonika)
  - [Simple squeeze](#simple-squeeze)
    - [Példa (positional squeeze – csak ha a védő a felvevő ELŐTT van)](#példa-positional-squeeze--csak-ha-a-védő-a-felvevő-előtt-van)
    - [Pozicionális vs. automatikus squeeze](#pozicionális-vs-automatikus-squeeze)
  - [Vienna coup](#vienna-coup)
    - [Klasszikus Vienna pozíció](#klasszikus-vienna-pozíció)
  - [Double squeeze](#double-squeeze)
    - [Pozíció (vázlatosan)](#pozíció-vázlatosan)
  - [Criss-cross squeeze](#criss-cross-squeeze)
  - [Trump squeeze](#trump-squeeze)
    - [Példa](#példa)
  - [Strip squeeze](#strip-squeeze)
    - [Lényeg](#lényeg)
    - [Példa](#példa-1)
  - [Compound squeeze](#compound-squeeze)
  - [Guard squeeze](#guard-squeeze)
    - [Példa](#példa-2)
  - [Trump coup](#trump-coup)
    - [Klasszikus példa](#klasszikus-példa)
  - [Coup en passant](#coup-en-passant)
  - [Loser-on-loser play](#loser-on-loser-play)
    - [Példa loser-on-loser](#példa-loser-on-loser)
  - [Dummy reversal](#dummy-reversal)
    - [Példa](#példa-3)
  - [Avoidance play](#avoidance-play)
    - [Tipikus avoidance helyzet](#tipikus-avoidance-helyzet)
  - [Safety play](#safety-play)
    - [Példa: AKxxx vs xxx (4 ütésért)](#példa-akxxx-vs-xxx-4-ütésért)
    - [Példa: AQTx vs xxx (3 ütésért)](#példa-aqtx-vs-xxx-3-ütésért)
  - [Hold-up play (várakozás)](#hold-up-play-várakozás)
  - [Communication play (átmenetek)](#communication-play-átmenetek)
    - [Klasszikus unblocking példa](#klasszikus-unblocking-példa)
    - [Entries számolása indulás után](#entries-számolása-indulás-után)
  - [Counting – a felvevő alapdiszciplínája](#counting--a-felvevő-alapdiszciplínája)
    - [Mnemonika a count-hoz: „**LFP-O**"](#mnemonika-a-count-hoz-lfp-o)
- [📋 Gyorskereső (játék közben)](#-gyorskereső-játék-közben)
  - [Indulóként – Első licit](#indulóként--első-licit)
  - [Segítőként – Partner 1-szintű színes nyitására (közbeszólás nélkül)](#segítőként--partner-1-szintű-színes-nyitására-közbeszólás-nélkül)
  - [Segítőként – Partner 1♣ / 1♦ nyitására (közbeszólás nélkül)](#segítőként--partner-1--1-nyitására-közbeszólás-nélkül)
  - [Segítőként – Partner 1NT nyitására (közbeszólás nélkül)](#segítőként--partner-1nt-nyitására-közbeszólás-nélkül)
  - [Ellenfél közbeszólt – mit jelent a kontrám?](#ellenfél-közbeszólt--mit-jelent-a-kontrám)
  - [Slamkereső szekvenciák – gyorsmenü](#slamkereső-szekvenciák--gyorsmenü)
  - [Védekezés – jelzések](#védekezés--jelzések)
  - [Példa licitsorozatok minden főbb konvencióhoz](#példa-licitsorozatok-minden-főbb-konvencióhoz)
    - [Stayman + 4-3 nemes felderítés](#stayman--4-3-nemes-felderítés)
    - [Jacoby transfer + szuper-elfogadás](#jacoby-transfer--szuper-elfogadás)
    - [Negative double + folytatás](#negative-double--folytatás)
    - [Splinter + Kickback slem](#splinter--kickback-slem)
    - [Lebensohl 1NT ellen + különböző folytatások](#lebensohl-1nt-ellen--különböző-folytatások)
    - [2/1 Game Forcing + lassú szerkezet-feltárás](#21-game-forcing--lassú-szerkezet-feltárás)
    - [Bergen mass-emelés példa](#bergen-mass-emelés-példa)
  - [Gyakori licitálási hibák – anti-pattern szekció](#gyakori-licitálási-hibák--anti-pattern-szekció)
    - [1. Stayman 4 lapos major trumf nélkül](#1-stayman-4-lapos-major-trumf-nélkül)
    - [2. Túl erős nemes-emelés gyenge kerettel](#2-túl-erős-nemes-emelés-gyenge-kerettel)
    - [3. Fourth-suit forcing helyett természetes 4. szín](#3-fourth-suit-forcing-helyett-természetes-4-szín)
    - [4. Splinter ász-szingli/színhiány esetén](#4-splinter-ász-szingliszínhiány-esetén)
    - [5. 1NT-re 4NT-vel ászkérdést indítani](#5-1nt-re-4nt-vel-ászkérdést-indítani)
    - [6. Gyenge 2-es Rule of 20-as kézzel](#6-gyenge-2-es-rule-of-20-as-kézzel)
    - [7. Reverse hiányában elveszett 17 HCP](#7-reverse-hiányában-elveszett-17-hcp)
  - [TODO – kidolgozandó és olvasnivalók](#todo--kidolgozandó-és-olvasnivalók)
    - [Alapok és értékelés](#alapok-és-értékelés)
    - [Lebensohl és kapcsolódó konvenciók](#lebensohl-és-kapcsolódó-konvenciók)
    - [Felvevő technikák (declarer play)](#felvevő-technikák-declarer-play)
    - [További olvasnivalók](#további-olvasnivalók)
    - [Cue bidek és slem-keresés](#cue-bidek-és-slem-keresés)
    - [BBO referencia (AdvGIB 2/1)](#bbo-referencia-advgib-21)
    - [Még kidolgozandó témák a következő iterációhoz](#még-kidolgozandó-témák-a-következő-iterációhoz)

---

## Bridge alapok

A bridge négy játékos kártyajátéka, ahol egymással szemben ülő játékosok együttműködnek párokban. Egy színből összesen 13 lap van.

### Pontok (HCP – High Card Points)

A figura pontok (HCP) az alapja a kéz erejének értékelésekor:

| Ász (A) | Király (K) | Dáma (D / Q) | Bubi (J / Jumbó) |
| :---- | :---- | :---- | :---- |
| 4 pont | 3 pont | 2 pont | 1 pont |

A pakli összes figura pontja: **40**.

### Eloszlási (többlet) pontok

- **Színhiány (void):** 3 pont (ha az ellenfél színéből: 5)
- **Egyke lap (singleton):** 2 pont (ha az ellenfél színéből: 3)
- **Doubleton (két lap egy színből):** 1 pont
- **Hosszú adu szín:** 8 lap fölött minden további lapért +1 pont
- **Hosszú nem adu szín:** értékelni kell, jó lehet benne eldobni a kiadókat. Az 5., 6., 7., stb. hosszért egy-egy többletpont, ha van hozzá honor.
- **Védtelen honorok:** −1 pont az önmagában álló K, Q vagy J esetében (pl. singleton király). A „bare honor" duplán számít: nincs hossz mögötte, ráadásul az ellenfél könnyen leveheti.

ℹ️ További olvasnivaló: [Hand evaluation – Wikipedia](https://en.wikipedia.org/wiki/Hand_evaluation)

### Lapérték-finomítás – LTC és Zar Points

A HCP + elosztási pont rendszer mellett két modern, finomabb értékelési módszer is használható (különösen, ha [fit](#nemes-szín-preferencia-segítőként) már megtalálva van):

#### **Losing Trick Count (LTC) – Veszítendő ütések száma**

Színenként megszámoljuk, hány **biztos vesztő ütés** van a kezünkben:

- Hosszúság szerint: max. **3 vesztő** egy 3+ lapos színben, max. **2 vesztő** 2 lapos színben, max. **1 vesztő** szingliben, **0 vesztő** voidban.
- Az A, K, Q minden hiányzó kártyára *–1 vesztő* (max. a szín hosszáig). Példa: 3 lapos színben Axx = 2 vesztő (a K és Q kiadó); AKx = 1 vesztő; AKQ = 0 vesztő.

**Klasszikus LTC szabály (fit megtalálva):**

| Saját + partner LTC összege | Javasolt vállalás |
| :---- | :---- |
| 14 | 4-es szint / game |
| 12 | Kis slem (6-os szint) |
| 10 | Nagy slem (7-es szint) |

> 💡 Az LTC kiváló kiegészítője a HCP-nek, mert érzékeny az **eloszlásra**. Egy 12 HCP-s, 1-5-4-3-as nyitókéz erősebb (8 vesztő), mint egy 13 HCP-s 4-3-3-3-as (9 vesztő).

#### **Zar Points (Zar Petkov rendszere)**

Egy átfogóbb értékelési mechanizmus, ami egyetlen számba sűríti a HCP-t, az elosztást és a kontrollokat:

```
Zar Pontok = HCP
           + Kontroll pontok (Ász=6, K=4, Q=2, J=1 — figyelem, NEM a klasszikus 4-3-2-1!)
           + Két leghosszabb szín hossza (összeadva)
           + (Leghosszabb szín − legrövidebb szín) különbsége
```

**Tipikus küszöbök:** Az 1-szintű nyitáshoz **26 Zar pont** kell. Game-hez kb. 52, kis slemhez 62, nagy slemhez 67. Erősen segít „határeseti" lapoknál (pl. „11 HCP, 6-3-3-1 — kell-e nyitni?").

### Színek rangsora

```
Nem nemes: ♣ Treff → ♦ Káró
   <
Nemes:     ♥ Kőr  → ♠ Pikk
   <
Szan (NT)
```

### Nemes szín preferencia (segítőként)

- 4 kőr és 4 pikk → **kőrt** mond
- 5 kőr és 5 pikk → **pikket** mond
- 4 kőr és 5 pikk → **pikket** mond (a hosszabbat)
- 5 kőr és 4 pikk → **kőrt** mond (a hosszabbat)

### Licitálási szintek (a partnerség két kezében összesen)

A két kéz együttes pontja és aduszámának függvényében:

| Vállalás | Pontok (összesen) | Egyéb feltétel |
| :---- | :---- | :---- |
| Színjáték (1, 2 vagy 3) | 18–23 pont | min. 8 adu (lehet 7, ha nincs fit) |
| Szan (1NT vagy 2NT) | 20–23 pont | lehetőleg nincs 8 a nemes színekből |
| Nemes gém (4♥, 4♠) | 24+ pont | min. 8 adu |
| Nem nemes gém (5♣, 5♦) | 26+ pont | min. 8 adu |
| Szan gém (3NT) | 24+ pont | lehetőleg nincs 8 egy színből sem |
| Kis slem (6 bármiből) | 32–33+ pont (NT: 33+) | min. 4 az 5 kulcslapból* |
| Nagy slem (7 bármiből) | 35–37+ pont (NT: 37+) | mind 4 ász + adu király + más király/hosszú szín |

*Kulcslapok (key cardok): a 4 ász és az adu király. Lásd: [Kickback RKC 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430).

> 💡 **Mindig értékeld a lapot!** Szokatlan eloszlás, sok adu, erős mellékszín vagy színhiány esetén kevesebb pont is elég lehet. Kombináld a HCP-t [LTC-vel](#lapérték-finomítás--ltc-és-zar-points), amint fit van.

---

## Az Induló szabályai (az első, aki nem passzol)

> 💡 Indulóként, ha 16 pontnál kevesebbed van, ne emelj második szintre, kivéve ha:
> - A partner színét emeled (1♦ → 1♠ → 2♠).
> - A saját extrahosszú (6+) színedet ismétled magasabb szinten.
> - Második, alacsonyabb rangú színt mutatsz be (4+ lappal): 1♦ → 1♠ → 2♣.
>
> Ha az első kéz felülmúlja ezt — pl. 17+ HCP-vel második szinten *magasabb* rangú új színt mondasz be → [reverse bid](#21-game-forcing-és-reverse-bidding)!

### Első licit

Mindig hívj 1-es színt, ha legalább 12 pontod van. Nyithatsz kevesebb pontból is (10–12), ha hosszú színed van vagy kedvező az eloszlás — alkalmazd [a Rule of 20-at](#the-rule-of-20)!

### Általános irányelvek

- Ha 5-ös nemes színed van, azzal indulsz.
- Ha 5+ van mindkét nemesből, **pikkel** indulsz (a második licitre kőr bemondásával jelzed).
- Ha 4-4 nem nemes, **káróval** indulsz (ha van 3 kárónál is több).
- Ha 3-3 nem nemes, **treffel** indulsz (convenient minor).

### Induló licitek – részletes táblázat

| Licit | Jelentés |
| :---- | :---- |
| 1♣ vagy 1♦ | 12–20 pont és minimum 3 lap a színben. A hosszabbal nyiss, ha azonosak, lásd fent. |
| 1♥ vagy 1♠ | 12–20 pont és minimum 5 lap a színben. A hosszabbal nyiss; azonos hossznál pikkel (kizárva az ellenfelet). |
| 1NT | Pontosan 15–17 pont és egyenletes eloszlás (min. 2 lap minden színből). Eloszlások: 4-3-3-3, 4-4-3-2, 5-3-3-2. |
| 1 valami → valami → 1NT (újrahívás) | 11–14 HCP. |
| 1 valami → valami → 2NT (ugrás) | 18–19 HCP, balanced. |
| Stop 2NT | 20–21 HCP, balanced. [Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) + [transfer](#jacoby-transzfer-i-és-ii-1nt--2-kőrre-1nt--2-pikkre) érvényben. |
| Stop 2♣ (!) | **22+ HCP balanced**, *vagy* **19+ HCP + 9+ playing trick** (eloszlásos kéz, „1 ütés hiányzik a gémhez"). A partnernek kötelező válaszolnia! Lásd: [Erős két treff indulás](#erős-2-treff-indulás). |
| Stop 2♣ → válasz → 2NT | 22–23 HCP, balanced. Stayman + transfer érvényben. |
| Stop 3NT | Pontosan 24–26 pont és egyenletes eloszlás. |
| Gyenge 2-es (Stop 2♦, 2♥, 2♠) | Pontosan 6-lapos adu színnel. Sebezhetőségtől függ: **Kedvezőtlen** (mi bellben, ők mansban) = **6–10 pont**, **Kedvező** (mi mansban, ők bellben) = **5–11 pont**, agresszívebb. |
| Gyenge 3-as (Stop 3♣, 3♦, 3♥, 3♠) | 6–11 pont, erős (min. 2 figura) pontosan 7-lapos adu színnel. |

**Fontos megjegyzés a gyenge 2-esről és a [Rule of 20](#the-rule-of-20)-ról:** A Rule of 20 (HCP + két leghosszabb szín hossza ≥ 20) kizárólag az **1-es szintű nyitásokra** vonatkozik! A gyenge 2-es tisztán preempt jellegű licit.

**Mikor NE nyiss gyenge 2-est:**

- Ha megvan a Rule of 20-ad! (Pl. 11 HCP, 6-os pikk, 3-as treff = 11+6+3=20. Ezzel **1♠**-t kell nyitni, nem 2♠-t!)
- Ha a kezedben van „két sima ász" (two bare aces), például ♠A és ♣A egy gyenge, 6 lapos kőr mellett.
- Ha van egy „erős holdingod" egy külső színben (pl. egy 4 lapos KQJx mellékszín). A gyenge 2-es erejének a saját, megnevezett hosszú színéből kell jönnie, hogy a partner megfelelően tudjon dönteni az áldozásról vagy a gémről.

### The Rule of 20

> **Szabály:** Számold össze a HCP pontjaidat, és add hozzá a két leghosszabb színed hosszát. Ha az összeg legalább 20, **és 1-es szintű nyitásról van szó**, indulj el.

**Példa (Rule of 20 érvényesül):** ♠AQxxx ♥xx ♦KJxx ♣Qx → 11 HCP + 5 (pikk) + 4 (káró) = 20 → **nyiss 1♠-t**.

**Példa (NEM elég):** ♠Axxx ♥Qxx ♦KJxx ♣Qx → 11 HCP + 4 + 4 = 19 → **passzolj** (nincs hosszú szín, nincs eloszlás).

> ⚠️ A Rule of 20 csak az 1-szintű színes nyitásokat indokolja, gyenge 2-est, gyenge 3-ast, 1NT-t NEM!

### The Rule of 44

Stop 2♣-vel akkor is lehet indulni, ha nincs 21 pont, de van:

- legalább **4 biztos ütés** (pl. 2 ász + 2 király egy színből), **ÉS**
- maximum **4 kiadó** ([LTC](#lapérték-finomítás--ltc-és-zar-points) ≤ 4).

Javasolt minimum: 18 HCP. Eszközként szolgál, hogy az „elosztásos, de nem klasszikusan 21 HCP-s erős kéz" se vesszen el.

### Az induló viszontválasza (miután a partner válaszolt – nem passzal)

| Licit | Jelentés |
| :---- | :---- |
| Új szín (1♣ → 1♥ → 1♠) | Legalább 4 lap és 13–20 pont. |
| Első szín emelése (1♣ → 1♥ → 2♣) | Hosszabb szín (nemes: 6+, nem nemes: 5+) és 12–16 pont. |
| Ugrás saját színben (1♣ → 1♥ → 3♣) | Erősebb kéz: 17–20 pont. |
| Partner színének emelése (1♣ → 1♥ → 2♥) | 4 lap a partner színéből és 13–16 pont. |
| Ugrás partner színében (1♣ → 1♥ → 3♥) | Erősebb kéz: 17–20 pont. |
| **Reverse** (1♦ → 1♠ → 2♥) | 17+ HCP, az első szín hosszabb, mint a második; **forcing** egy körig. Lásd: [Reverse Bidding](#21-game-forcing-és-reverse-bidding). |
| 1NT (1♣ → 1♥ → 1NT) | 12–14 pont, a partner színében nincs 4 lap, és nincs másik 4-lap színed az első szinten. |
| 2NT (újra) | Itt már tudjuk, hogy megvan a gémre a pont; kérdezzük, hogy a partnernek van-e stoppere (lásd: [Western Cue bid](#western-cue-bid-stopper-kérés)), vagy elkezdünk tapogatózni slem felé. |

---

## A Segítő szabályai (miután az Induló megnyitotta a licitet)

A Segítő (responder) az Induló partnere. Általában akkor válaszol, ha legalább 6 pontja van.

> 💡 **Általános irányelvek:**
> - Nem nemes nyitásra (1♣/1♦), ha 4+ lapod van nemes színből, mindig azzal válaszolj. Ha mindkét nemesből 4 lapod van, **kőrrel**.
> - Nemes nyitásra (1♥/1♠), ha 3+ lapod van a partner színéből, emelj egy szinttel (1♠ → 2♠), hogy megerősítsd a 8 lapos fitet. (De lásd: [Bergen raises](#bergen-raises)).
> - Ha 10 pontnál kevesebbed van, ne emelj 2-es szintre, kivéve ha a partner színét emeled, vagy a saját extrahosszú színedre licitálsz.
> - Egyes furcsa eloszlásnál 1NT-t kell mondani, hogy alacsony maradjon a licit.

### Semi-forcing 1NT (1M – 1NT)

Az 1♥ vagy 1♠ nyitásra adott **1NT** válaszunk (6–12 HCP) **Semi-forcing**. A nyitó elméletileg passzolhatja, de **csak és kizárólag** akkor, ha egy teljesen lapos (balanced), egyenletes minimuma van (12–13 HCP). Minden más, elosztásos vagy erősebb kézzel a nyitónak licitálnia kell.

> 💡 Ez különbözik a klasszikus „forcing 1NT" SAYC-tól, ahol a nyitó *mindig* köteles válaszolni. A semi-forcing kompromisszum: kényelmesebb, és a passzolt minimumokat (~2/3 esetében) sem viszik fel feleslegesen.

### A) Első válasz – ha az ellenfél NEM szólt közbe

Ezek a válaszok érvényesek tiszta licitsorozatban (Induló licitált, ellenfél passzolt vagy még nem volt szava).

#### Áttekintő táblázat

| Licit | Jelentés |
| :---- | :---- |
| 1. szinten új szín (1♣ → 1♥) | 4+ lap a színből és 6–16 pont. |
| 2. szinten új szín, ugrás nélkül (1♥ → 2♦) | 4+ lap a színből és 10–16 pont. *(Lásd: [2/1 Game Forcing](#21-game-forcing-és-reverse-bidding).)* |
| Ugrás új színben / Jump-shift (1♦ → 2♥) | Nagyon erős: 17+ pont és 4+ lap a színből. |
| Induló nemes színének emelése 2-es szinten (1♥ → 2♥) | 3+ lap a színből (nem 4!) és 6–9 pont. |
| Stop 3 nemes – Induló színének emelése (1♥ → 3♥) | Preemptív zárás! (Lásd: [Bergen Raises](#bergen-raises)). 0–5 pont, 4 lapos adu. |
| 1NT (1♠ → 1NT) | 6–12 pont (Semi-forcing). Nincs partner színében elég lap. |

#### Inverted minor (csak nem nemes nyitásra)

> ⚠️ Csak akkor érvényes, ha az ellenfél NEM szólt közbe!

Az „inverted" lényege, hogy a sima emelés **erős**, az ugró emelés **gyenge** (preempt) – fordítva a természetes logikával:

| Licit | Jelentés |
| :---- | :---- |
| Erős sima emelés (1♣ → 2♣ vagy 1♦ → 2♦) | 10+ pont, legalább 4 lap támogatás, nincs 4 lapos nemes szín. Egy körig forcing. |
| Gyenge ugró emelés (1♣ → 3♣ vagy 1♦ → 3♦) | 0–6 pont, legalább 5 lap támogatás, nincs 4 lapos nemes szín. Preemptív. |

#### Az induló viszontválaszai inverted minor sima emelés után

**1♣ → 2♣ után:**

![Induló viszontválaszai 1♣ – 2♣ után (inverted minor folytatás)](https://github.com/imre-nicowl/Bridge/blob/main/Pics/strong_clubs_raise_responses.png)
<!-- IMAGE PLACEHOLDER: 3. ábra – Induló viszontválaszai 1♣ – 2♣ után (inverted minor folytatás). -->

**1♦ → 2♦ után:**

![Induló viszontválaszai 1♣ – 2♣ után (inverted minor folytatás)](https://github.com/imre-nicowl/Bridge/blob/main/Pics/strong_diamonds_raise_responses.png)
<!-- IMAGE PLACEHOLDER: 4. ábra – Induló viszontválaszai 1♦ – 2♦ után (inverted minor folytatás). -->

#### Jacoby 2NT (segítőként, csak nemes nyitásra)

> ⚠️ Csak akkor érvényes, ha az ellenfél NEM szólt közbe!

Egy 1♥ vagy 1♠ nyitás után a segítő közvetlen 2NT licitje a **Jacoby 2NT** konvenció.

**Feltételek:**

- Segítőként, közvetlenül egy 1♥/1♠ nyitás után.
- 13+ pont és **4+ lap** támogatás az induló színéből (a [Bergen Raises](#bergen-raises) rendszerben a Jacoby 2NT 4 lapos fittel párosul!).
- Műlicit, Game Forcing. Slem érdeklődést jelez.

**Induló válaszai a 2NT-re:**

| Induló licitje | Jelentés |
| :---- | :---- |
| 3 szinten új szín | 0 vagy 1 a színből (splinter / shortness). |
| 4 szinten új szín | 4 vagy több lap a színből (erős mellékszín). |
| 3 a saját nemes színe (1♥ → 2NT → 3♥) | Ha kőrrel indult: 17–20 pont, slem-érdeklődés. Ha pikkel indult: a 3♥ a 3♣/♦-hoz hasonlóan egykét/színhiányt ígér. |
| 3♠ az induló pikkje (1♠ → 2NT → 3♠) | 17–20 pont, slem-érdeklődés. (Ha kőrrel indult, akkor 3♠ a 3♣/♦-hoz hasonlóan egykét/színhiányt ígér.) |
| 3NT | Csak 13–16 pont, nincs egyke vagy színhiány. |
| 4♣ / 4♦ | 5+ lap a jelzett színből. |
| 4♥ / 4♠ | Ha az indított nemes szín, akkor lezáró licit. (Sign-off, rossz kéz). |

**A válaszok prioritása (általánosan):**

1. Először: erős 5+ lapos mellékszín bemondása.
2. Aztán: egyke vagy színhiány jelzése.
3. Aztán: ugrás 4 nemesre 12–14 ponttal.
4. Végül: a megegyezett nemes 3-as szintű ismétlése 16+ ponttal és nincs más megfelelő licit.

**Példa licitsorozat (Jacoby 2NT + Kickback):**

| Induló | Segítő |
| :---- | :---- |
| 1♥ (5+ kőr, 13–20 pont) | 2NT (4+ kőr, 13+ pont) |
| 3♣ (egyke/színhiány treffből) | 3♦ (ász vagy színhiány káróból) |
| 4♣ (fixen színhiány treffből) | 4♠ (ász vagy színhiány pikkből) |
| 4NT ([Kickback 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430), adu: kőr) | ... |

#### Bergen Raises

Marty Bergen rendszere a **pontosan 4 lapos** nemes-supportot (fittet) fejezi ki, 1♥ vagy 1♠ nyitás után. Erősen épít a [Law of Total Tricks](#the-law-of-total-tricks)-re.

| Licit | Jelentés |
| :---- | :---- |
| 1M – 3♣ | Gyenge mass-emelés (6–9 HCP, **4 lapos adu**). Konstruktív, preemptív. |
| 1M – 3♦ | Invitáló mass-emelés (10–12 HCP, **4 lapos adu**). |
| 1M – 3M | Preempt zárás (0–5 HCP, **4 lapos adu**). Gyors szintemelés az ellenfél elnémítására. |
| 1M – 2NT ([Jacoby 2NT](#jacoby-2nt-segítőként-csak-nemes-nyitásra)) | Game Forcing (13+ HCP, **4+ lapos adu**). |

> 💡 A különbség a sima 2-es emeléshez (3 lapos!) képest: itt mindenhol 4 lapos a fit, így pontosabban tudjuk a Law of Total Tricks-szel a biztonságos szintet (9 adu → 3-as szint biztonságos).

### B) Első válasz – ha az ellenfél KÖZBESZÓLT

> ⚠️ Ha közbeszóltak, sok természetes licit jelentése megváltozik. Az [Inverted minor](#inverted-minor-csak-nem-nemes-nyitásra) és a [Jacoby 2NT](#jacoby-2nt-segítőként-csak-nemes-nyitásra) NEM játszik közbeszólás esetén!

<a id="ellenfél-kontrázott--ez-is-közbeszólás"></a>
#### Az ellenfél kontrázott — ez **is** közbeszólás

**Fontos elv:** A takeout double **közbeszólásnak számít** (interference). Minden konvenció, ami közbeszólásra „lekapcsol", X-re is lekapcsol:

| Konvenció | Uncontested | Takeout double után |
| :---- | :---- | :---- |
| Inverted Minor | ✅ aktív | ❌ NEM aktív |
| Jacoby 2NT | ✅ aktív | ❌ NEM aktív (helyette: [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után)) |
| Bergen Raises | ✅ aktív | ❌ NEM aktív (helyette: [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) + módosított raise-struktúra) |
| 2/1 Game Forcing | ✅ aktív | ⚠️ **NEM tisztán GF** — a 2-es szintű új szín 10+ HCP F-1, de nem automatikusan GF |
| Semi-forcing 1NT | ✅ aktív | ⚠️ 1NT inkább 7–10 HCP, NF |
| Stayman / Jacoby transfer (1NT után) | ✅ aktív | Lásd: [B) Válaszok 1NT-re, ha az ellenfél közbeszólt](#b-válaszok-1nt-indulásra-ha-az-ellenfél-közbeszólt) |

**A licit-konstrukció ilyenkor (1♥/♠ – (X) – ?):**

| Te licited | Erő | Jelentés |
| :---- | :---- | :---- |
| **PASSZ** | 0–5 | Nincs jó licit |
| **2 ugyanaz a szín** (2♥) | 6–9 | 3+ adu, **konstruktív** (NEM preemptív, mint közbeszólás nélkül!) |
| **3 ugyanaz a szín** (3♥) | 0–6 | 4+ adu, **preemptív** (defenzív) — *lényeg: 4+ lapos support, nem invitációs!* |
| **4 ugyanaz a szín** (4♥) | 0–7 | 5+ adu, shape-es, lezáró |
| **2NT** | **10+** | **Jordan 2NT** — 4+ adu, limit+, GF-irány. Lásd: [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után). |
| **XX (rekontra)** | **10+** | **NINCS 4+ adu** — penalty-irány, 1 körig F. Általában *deny*-eli a 4 lapos nemes-fit-et (ha lenne, Jordan 2NT vagy splinter lenne) |
| **Új szín 1-es szinten** (1♠) | 6+ | 4+ lap, NF |
| **Új szín 2-es szinten** (2♣) | 10+ | 4+ lap, F-1 (de nem automatikus GF) |

> 💡 **Memóriasegítő — a „double a duma":**
> - **Direct raise = 6-9 HCP** (konstruktív, mint partner-tájékoztatás)
> - **Jump raise = 0-6 HCP, 4+ adu** (preemptív, ellenfél megnehezítése)
> - **2NT = Jordan, 10+ HCP, 4+ adu** (slam-irány vagy biztos gém)
> - **XX = 10+ HCP, NINCS fit** (penalty / büntetés keresése)
>
> Vagyis a 4 lapos fit **AKÁR gyenge, AKÁR erős** kézzel rögtön kiderül — ami információs előnyt jelent a partnerünknek a kompetitív kontra-átmenetekben.

<a id="negatív-kontra-a-standard-sayc-b-konvenció"></a>
#### Negatív kontra – a Standard SAYC (B konvenció)

A negatív kontra 6+ pontot ígér, és kifejezetten a be nem mondott nemes szín(ek)et mutatja:

- **Ha az ellenfél nemessel szólt közbe (pl. 1♦ – 1♥ – X):** A kontra *pontosan 4 lapos* hosszúságot ígér a másik nemesből (itt pikkből). Ha 5 pikked lenne, azt licitálnád, hogy 1♠.
- **Ha az ellenfél nemessel, kettes szinten szólt közbe (pl. 1♦ – 2♥ – X):** Ez is *pontosan 4 lapos* pikket ígér. (Mivel a 2♠ licit legalább 5 lapot és 10+ pontot ígérne.)
- **Ha az ellenfél alsó színnel szólt közbe (pl. 1♣ – 1♦ – X):** A kontra mindkét nemesből *pontosan 4-4 lapot* ígér.

*Ebből következik a fontos inferencia:* Ha az ellenfél 1♥-t vagy 2♥-t mondott, és a segítő kontrázni tudna (hogy 4 pikket mutasson), de ehelyett mégis licitálja a pikket (pl. 1♠ vagy 2♠), akkor a licitje **kőbe vésetten 5+ lapos** pikket ígér!

#### Kevert emelés (Mixed Raise)

> 💡 **Miért nem Bergen?** A [Bergen Raises](#bergen-raises) (3♣ = 7–9 + 4-es fit, 3♦ = 10–11 + 4-es fit) **csak akkor működik, ha az ellenfél nem szólt közbe**. Amint közbeszóltak, a 3♣ / 3♦ már *cuebid* értelmezést kaphat (ha az volt az ellenfél színe), vagy a licittér más okból lefoglalt. Ezért **contested** helyzetben a **Mixed Raise** veszi át a Bergen szerepét — egyszerűsített, ütésszint-orientált struktúrával.
>
> **Memorizálási szabály:** *Bergen = uncontested, Mixed Raise = contested overcall, Jordan 2NT = contested by takeout double.*

Ha közbeszóltak az indulásra, a segítő kevert emeléssel válaszol.

**Példa:** Észak 1♥ — Kelet 2♣ — Dél ?

| Dél válasza | Jelentés |
| :---- | :---- |
| Passz | 0–5 pont és nincs 4-nél több kőr. |
| Szín ismétlése 2-es szinten (2♥) | 10–12 pont. |
| Szín ismétlése 3-as szinten (3♥) | 6–9 pont, preempt. |
| Szín ismétlése 4-es szinten (4♥) | 0–5 pont, minimum 5-ös szín. |
| Ellenfél színének licitálása (3♣ cue bid) | 13+ pont, támogatás, forcing. |

#### Jordan 2NT (4+ fit + 10+ HCP take-out double után)

**Helyzet:** Partnered nemest nyitott (1♥ vagy 1♠), és **a jobb ellenfeled take-out kontrázott**.

Eredeti SAYC-ben a 2NT itt 13+ HCP, balanced, nincs fit lett volna — de takeout double után ez a *közbeszólás minősége* miatt szinte sosem releváns (ha balanced 13+-od van, és nincs fit, általában rekontrázol). Ezért a 2NT-t **átfordítjuk** Jordan 2NT-re.

| Te válaszod 1♥/♠ – (X) – ? után | Jelentés |
| :---- | :---- |
| **Passz** | 0–5 HCP, nincs jó licit |
| **1NT** | 7–10 HCP, balanced, nincs adu-fit (NF) |
| **2 ugyanaz a szín** (2♥) | 6–9 HCP, 3+ adu — *konstruktív* sima emelés |
| **2NT (Jordan)** | **10+ HCP, 4+ adu, limit+** (GF irány) |
| **3 ugyanaz a szín** (3♥) | 4+ adu, 0–6 HCP, **preemptív** (defenzív emelés) |
| **4 ugyanaz a szín** (4♥) | 5+ adu, 0–7 HCP, shape-es, lezáró/preemptív |
| **Új szín 1-es szinten** (1♠) | 6+ HCP, 4+ lap, NF (mint közbeszólás nélkül) |
| **Új szín 2-es szinten** (2♣/2♦) | 10+ HCP, 4+ lap, F (a 2/1 GF nem feltétlenül érvényesül kontra alatt) |
| **2♠ ugró új szín** (1♥ után) | Splinter (4+ kőr + ♠ rövidség, 10–13) |
| **XX (rekontra)** | **10+ HCP, NINCS 4+ adu** — penalty-irány, forcing 1 körig |

**Példa:**

| Lap | Te kezed |
| :---- | :---- |
| ♠ Q 4 | 2 pikk |
| ♥ K J 8 2 | 4 kőr |
| ♦ Q J 7 6 | 4 káró |
| ♣ K 8 5 | 3 treff |

**HCP:** 11. Partner 1♥ nyitott, jobb ellenfél X (takeout).

**Helyes licit:** 2NT (Jordan) — 11 HCP, 4 fit kőrben, limit+ raise. A partner most már GF üzemmódban van, és slam felé tovább vihet.

> 💡 **Mire való a Jordan 2NT?** Egyszerre teszi nyilvánvalóvá a 4 lapos fit-et ÉS a limit+ erőt. Enélkül a 4 fitet 3♥ vagy 4♥ közvetlenül kellene mutatni — de azok preemptív stílusúak (gyenge). A 2NT az egyetlen „tiszta" konstruktív licit a 4 fittel.

> ⚠️ **Eredeti 2NT (balanced 13+, nincs fit)?** Erre most a **rekontrával + utólagos NT-vel** kell eljutni:
>
> ```
> 1♥ – (X) – XX – (Passz)
>  ?  – (Passz) – 2NT  →  balanced 13+, nincs 4 fit
> ```

---

## Válaszok az 1NT vagy 2NT indulásra

Az 1NT pontosan **15–17 pontot** és balanced eloszlást ígér. A 2NT **20–21 pontot**.

### A) Segítő válaszai 1NT indulásra (közbeszólás nélkül)

| Licit | Jelentés |
| :---- | :---- |
| Passz | 0–7 pont és nincs 5-ös nemes (→ [Jacoby](#jacoby-transzfer-i-és-ii-1nt--2-kőrre-1nt--2-pikkre)) vagy 6-os minor szín (→ 2♠). |
| 2♣ ([Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2)) | 8–9 pont, pontosan négy kőr és/vagy négy pikk (egyébként [Puppet Stayman](#puppet-stayman-konvenció-1nt--3-vagy-2nt--3)). VAGY [Garbage Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) / [Smolen](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2). |
| 2♦ (Jacoby transzfer kőrre) | 8+ pont, legalább 5 kőr, partner mondja be a 2♥-t. |
| 2♥ (Jacoby transzfer pikkre) | 8+ pont, legalább 5 pikk, partner mondja be a 2♠-t. |
| 2♠ (Minor suit transfer) | 8+ pont, hatos hosszúságú nem nemes (minor) szín. Erre kötelező 3♣-t mondani; gyenge partner 3♦-ra korrigál, ha káró volt. |
| 2NT | 8–9 pont, balanced eloszlás, invitál 3NT-re. |
| 3♣ ([Puppet Stayman](#puppet-stayman-konvenció-1nt--3-vagy-2nt--3)) | 10+ pont (game force), legalább egy 3-as hosszúságú nemes. |
| 3NT | 10–13 pont, biztos a gém, nincs slem. Lezáró licit. |
| 4♣ (Gerber) | Ászkérdés. Lásd: [Gerber](#gerber-szanra-adott-ász--és-királykérdés). |
| 4♦ (Texas transfer kőrre) | 6+ kőr, partner mondja be a 4♥-t. |
| 4♥ (Texas transfer pikkre) | 6+ pikk, partner mondja be a 4♠-t. |
| **4NT** | **Kvantitatív meghívás 6NT-re.** (16–17 HCP). A nyitó 15 ponttal passzol, 17-tel 6NT-re emel. **NEM ászkérdés!** 1NT után az ászkérdés a 4♣ Gerber! |

#### Stayman, Smolen és Garbage Stayman konvenciók (1NT → 2♣)

A Stayman feltétele általában 8+ pont, célja a 4-4 nemes fit megtalálása. Azonban az 1NT → 2♣ sorozat két speciális elágazással is kiegészül:

**1. A Garbage Stayman (Szemét Stayman – Menekülés)**

Ha a segítőnek **nagyon gyenge** keze van (0–7 pont), de „rövid" a treffje (pl. 4-4-4-1 vagy 4-4-5-0 eloszlás), az 1NT elbukna. A segítő elindítja a Staymant (2♣):

- Ha a nyitó nemest talál (2♥ vagy 2♠), a segítő boldogan **passzol**.
- Ha a nyitó tagadja a nemest (2♦), a segítő **2♥-t vagy 2♠-t** mond. Mivel a Staymant indító már nem lehet erős (különben ugrana), ez a licit **Sign-off**, azaz a nyitónak kötelező passzolnia!

**2. A Smolen Konvenció (Game Forcing 5-4 nemesek)**

Ha a segítőnek **Game Forcing** keze van (10+ pont) és **5-4 eloszlása** a nemesekben. (Nem indíthat Jacoby Transzfert, mert akkor a 4 lapos nemese elvész.)

- A segítő Staymant mond (2♣).
- Ha az induló bemond egy nemest (2♥/2♠) → Megvan a gém, emelünk.
- Ha az induló tagadja a nemest (**2♦**), a segítő **UGRIK a másik, RÖVIDEBB nemes színben** (3♥ vagy 3♠).
- *Jelentés:* A bemondott 3-as szintű színben 4 lapom van, a *másik* nemesben 5 lapom van, és Game Forcing vagyok! Az induló így tudni fogja a pontos 5-4 eloszlást, és ha van 3 lapos fitje az 5-ös színünkhöz, ő fogja azt bemondani, így az erős 1NT kéz lesz a rejtve maradó felvevő!

**Segítő válaszai – 1NT → 2♣ → 2♦ (Nincs 4-es nemes) után:**

| Segítő licitje | Jelentés |
| :---- | :---- |
| 2♥/2♠ | Garbage Stayman: 0–7 pont, gyenge kéz 5-ös nemessel (vagy menekülés). **Sign-off!** |
| 2NT | Nincs 5-ös nemes (csak egy vagy két 4-es), invitál 3NT-re. |
| 3♥/3♠ | **Smolen** konvenció: 4 lap a licitált nemesben, 5 lap a másikban. Game Forcing. |
| 3NT | Lezáró licit, nincs slem. |

<a id="crawling-creeping-stayman-konvenció"></a>
#### Crawling (Creeping) Stayman konvenció

**Mikor használjuk?** Ha 0–7 HCP-d van, és a kezed 4-4 (vagy 5-4 / 4-3) a nemesekben + rövid treff, de a partner 1NT nyitására adott Garbage Stayman válaszodra (2♣) a partner **2♦-ot vagy 2♥-t** mondott. Most „felkúszunk" a 2-es szinten a legjobb fit reményében.

**Crawling Stayman szekvencia:**

| Licit | Jelentés |
| :---- | :---- |
| 1NT – 2♣ – **2♦** – **2♥** | 4-4 nemes, gyenge (0–7). Partnernek: passz 4 kőrrel, **2♠** 4 pikkel. (Ez a klasszikus Garbage logika, *kúszás nélkül*.) |
| 1NT – 2♣ – **2♦** – **2♠** | 4 pikk + 5+ kőr, gyenge. Partner passzol 3-as pikkel, vagy **3♥**-re javít 2-es pikkel + 3-as kőrrel. |
| 1NT – 2♣ – **2♥** – **2♠** | **Crawling**: 4 pikk + 4-es kőr **vagy** 5+ pikk + 3-as kőr, gyenge. Partner most már **TUDJA**, hogy van 4 köröd, ezért választhat: passz 4 pikkel (4-4 fit pikkben) vagy **3♥** 5+ pikk + 3-as kőrre vissza. |
| 1NT – 2♣ – **2♠** – **PASSZ** | Garbage, 4 pikk, gyenge — nincs miért tovább kúszni. |

> 💡 **A Crawling Stayman kulcsa:** a 2♠ a partner 2♥ rebidje *után* nem 5+ pikket ígér — hanem azt mondja: *„4 pikkem van, és tudom, hogy 4+ köröd van. Te döntesz a 4-4 fit között."*

> ⚠️ **Konvenció-megegyezés szükséges!** A natural-Stayman játszók szerint 1NT – 2♣ – 2♥ – 2♠ az invitációs 5+ pikk lenne. A Crawling variánst **előre meg kell beszélni** partnerrel.

**Mire jó valójában?** Olyan helyzetekben, ahol 4-3-3-3 vagy 4-3-4-2 mellett gyenge kézzel mégis a nemes-fit a legjobb játszható szerződés (egy 4-3 fit jellemzően jobb, mint 1NT 0–7 HCP-vel).

**Példa:**

| Lap | Te kezed |
| :---- | :---- |
| ♠ K J 8 6 | 4 pikk |
| ♥ Q 7 5 2 | 4 kőr |
| ♦ J 7 3 | 3 káró |
| ♣ 6 4 | 2 treff |

**HCP:** 7. Sebezhetőség mindegy.

```
Partner: 1NT
Te:      2♣ (Garbage/Crawling Stayman, 0–7)
Partner: 2♥ (4 kőr van neki)
Te:      2♠ (Crawling — 4 pikk + 4 kőr, gyenge; te választasz)
Partner: PASSZ (4-4 pikk fit van, ez jobb mint 3♥)
```

#### Puppet Stayman konvenció (1NT → 3♣ vagy 2NT → 3♣)

Feltételek: 1NT-re 10+ HCP, 2NT-re 4–5 HCP, és legalább egy 3-as hosszú nemes.

**Konvenció lényege:** A Puppet Stayman *5-ös* és *4-es* nemest is keres a nyitónál (a sima Stayman csak 4-est). Hasznos, amikor 5-3 fit-et szeretnél megtalálni.

**Lépés 1 – A nyitó válasza a 3♣-re:**

| Nyitó licit | Jelentése |
|---|---|
| **3♦** | "Van *legalább* egy 4-es nemesem (de nincs 5-ösöm)." |
| **3♥** | "5 kőröm van." |
| **3♠** | "5 pikkem van." |
| **3NT** | "Nincs 4+ lapos nemesem." |

**Lépés 2 – Ha a nyitó 3♦-t mondott (van valamelyikből 4 lap), a kérdező folytatja:**

| Kérdező licit | Jelentése |
|---|---|
| **3♥** | "*Pikkem* van 4 lap (nem kőröm!) — kérdezem, van-e neked 4 pikked." → ha a nyitónak van 4 pikk: **4♠**, ha nincs: **3NT** |
| **3♠** | "*Köröm* van 4 lap (nem pikkem!) — kérdezem, van-e neked 4 köröd." → ha a nyitónak van 4 kőr: **4♥**, ha nincs: **3NT** |
| **3NT** | "4-4 nemesem van, vagy nem érdekel a fit." |

**Lépés 3 – Ha a nyitó 3♥/3♠-t mondott (5 lapos nemes), a kérdező folytatja:**

| Kérdező licit | Jelentése |
|---|---|
| **Egy szinttel emelés** (4♥/4♠) | 3+ lap fit, gémszint, nincs slam-érdeklődés |
| **3NT** | Nincs 3 lapos fit, NT-ben akarom játszani |
| **4-es szintű új szín** | Slam-cue (kontroll), fit van |
| **4NT** | Kickback indul (ha a fit megerősíthető) |

> 💡 **Mikor használd?** 1NT/2NT nyitásra GF + esetleges 5-3 nemes fit-keresés. **Feltétel:** legalább egy 3+ lapos nemes.

#### Jacoby transzfer I. és II. (1NT → 2♦ kőrre, 1NT → 2♥ pikkre)

Feltétel: 5 vagy több lap a színben. Az erős kéz (nyitó) fogadja a transzfert (2♥/2♠), így ő lesz a felvevő.

**Lépés 1 – 1NT → 2♦ (kőr transzfer) után a nyitó válasza:**

| Nyitó licit | Jelentése | Mikor? |
|---|---|---|
| **2♥** | Sima elfogadás | Alapeset, bármilyen erő (15–17 HCP) |
| **2♠** | "Big" elfogadás (ritkán használt) | Max + 4 kőr + 5+ pikk (kétszínű) |
| **2NT** | Szuper-elfogadás NT-ben | Max (17 HCP), pontosan 2 kőr (doubleton), kiegyensúlyozott — "ne menj tovább, ha gyenge vagy" |
| **3♣ / 3♦ / 3♠** | "Source of tricks" szuper | Max + 4 kőr + 5-ös ütésforrás a mondott színben (3♠ = vacuum/honor-doubleton-szín) |
| **3♥** | Klasszikus szuper-elfogadás | Max (17 HCP) + 4 kőr, kiegyensúlyozott |
| **4♥** | Megelőző / lezáró | Max + 4 kőr + nagyon offenzív (hosszú szín, kevés HCP de sok shape) |

**Lépés 2 – Ugyanez 1NT → 2♥ (pikk transzfer) után:**

| Nyitó licit | Jelentése |
|---|---|
| **2♠** | Sima elfogadás |
| **2NT** | Max + 2 pikk doubleton, kiegyensúlyozott |
| **3♣ / 3♦ / 3♥** | Max + 4 pikk + ütésforrás a megnevezett mellékszínben |
| **3♠** | Klasszikus szuper-elfogadás (max + 4 pikk) |
| **4♠** | Megelőző max + 4 pikk + nagyon offenzív |

**Lépés 3 – A válaszadó folytatása szuper-elfogadás után:**

| Válaszadó licit | Jelentése |
|---|---|
| Passz | "Az 5 lapom + a maxod elég a gémhez? Nem, kihagyom." (csak 3♥/3♠ után) |
| **3NT** / **4NT** | Kvantitatív választás: NT vagy színben (a partner választ) |
| **Új szín 4-es szinten** | Cue-bid → slam-érdeklődés |
| **4♥/4♠** | Lezáró gémben (signoff) |
| **4NT** | Kickback (a transzferelt nemes az adu) |

**Szuper-elfogadás:** Ha a nyitónak 4+ lapja van a segítő nemeséből és maximuma (16–17 HCP), nem 2-es, hanem **3-as szinten** fogadja a transzfert. Ez biztat a 4-es szintű gémre.

### B) Válaszok 1NT indulásra, ha az ellenfél közbeszólt

#### Az ellenfél kettes szinten szólt közbe – kontra

A kontra a Staymant jelenti.

**Példa:** 1NT – 2♦ – X (Stayman: 8+ pont, legalább egy 4-es nemes).

**Helyzet:** 1NT – (2X) – ? — ahol a 2X egy 2-szintű természetes közbeszólás (pl. 2♦, 2♥ vagy 2♠).

| A válaszadó licitje | Jelentése |
|---|---|
| **Passz** | 0–7 HCP, nincs jó megoldás |
| **X (kontra)** | **Stayman-kontra**: 8+ HCP, *legalább egy* 4-es nemes (a "Stayman a régi szerepben") — a nyitó a saját 4-eseit licitálja |
| **2-es szinten új szín** | 0–7 HCP, 5+ lap, lezáró (NF) |
| **2-es szinten cue** (a közbeszólt szín) | Nincs használatban (kontra van helyette) |
| **2NT** | Lebensohl relay → 3♣ átkérés (lásd 8. ábra) |
| **3-as szinten új szín** | 5+ lap, GF (Lebensohl nélkül) |
| **3-as szinten cue** | "Van stoppered?" — GF |
| **3NT** azonnal | GF, NINCS stopper a közbeszólt színben |

**Példa:**
```
1NT – (2♦) – X (Stayman, 8+ HCP, van 4-es nemes) – Passz
2♥ (nyitó: "van 4 köröm") – Passz – 4♥ (gém)
```

#### Lebensohl 1NT közbeszólás ellen

> 💡 **Slow shows, fast denies.**

Példa licit kiindulás: 1NT – (2♥) – ?

Pont szerint:

- **0–7 pont (gyenge):** 2NT → 3♣/3♦ Lebensohl, lezáró.
- **Invitálási kéz (8–9 pont):** Lebensohl (2NT) után olyan szín bemondása, amit azonnal is mondhattál volna (pl. 3♠). Ígér 5+ lapot, invitálás.
- **10+ pont (game force):**
  - 3-as szinten új szín azonnal (Lebensohl nélkül, pl. 3♠): 5 a színből, GF.
  - **Cue bid (3♥):** „Van stoppered? → 3NT = van, más = nincs."
  - Lebensohl → 3NT: **VAN** stopper, nincs 4 nemes.
  - Közvetlen 3NT: **NINCS** stopper, nincs 4 nemes.

**Helyzet:** 1NT – (2♥/2♠) – ?

**Alapszabály:** *Slow shows, fast denies* — a 2NT-en át menő (lassú) út stoppert mutat, a közvetlen (gyors) út tagadja.

**Az összes lehetséges licit:**

| A válaszadó licitje | Erő | Forcing? | Stopper? | Mit jelent? |
|---|---|---|---|---|
| **Passz** | 0–7 | NF | – | Nincs jó megoldás |
| **2-es új szín** (csak 2♥ után 2♠) | 0–7 | NF | – | 5+ lap, lezáró |
| **X (kontra)** | 8+ | Forcing 1 körig | – | Penalty-irányultságú / cooperative |
| **2NT** | 0–7 (gyenge) **vagy** 8–9 (inv) | Forcing 3♣-re | – | Lebensohl relay – a következő licit jelez |
| **3♣ / 3♦** (közvetlen) | 10+ | GF | – | 5+ lap, GF, **NINCS stopper** |
| **3♣ / 3♦ Lebensohl után** | 8–9 | NF | – | **Invitálás**, 5+ lap |
| **3-as cue** (a közbeszólt szín) | 10+ | GF | Kérdez | "Van stoppered? → 3NT igen, más nem" |
| **3-as cue Lebensohl után** | 10+ | GF | Kérdez | (Ritkábban használt) |
| **3♥/3♠** (ha másik nemes) | 10+ | GF | – | 5+ lap a másik nemesből, GF |
| **3NT közvetlen** | 10+ | – | **NINCS** | GF, nincs stopper, nincs 4-es másik nemes |
| **3NT Lebensohl után** | 10+ | – | **VAN** | GF, van stopper, nincs 4-es másik nemes |
| **4♣ / 4♦** | 10+ | GF | – | Texas-jellegű transzfer / két-színű |

**Memóriasegítő:**

```
                    1NT – (2♥) – ?
                         │
   ┌─────────────────────┼─────────────────────┐
  0–7                   8–9                    10+
   │                     │                       │
  Passz                 2NT → 3♣ → ?           Közvetlen
  vagy 2♠               (Lebensohl)               │
                         │                  ┌─────┴─────┐
                       3♣/3♦                Cue        3NT
                       (inv)              (Stoppert    (NINCS
                       3NT                 kérdez)      stopper)
                       (VAN stopper)        
```

---

## Válasz a gyenge 2-esre

A gyenge 2-es 6–10 pontot és pontosan 6-lapos erős színt mutat. (Lásd a [pontos tartományokat](#induló-licitek--részletes-táblázat) sebezhetőség szerint.)

### A) Válaszok közbeszólás nélkül

| Licit | Jelentés |
| :---- | :---- |
| Emelés ugrással (2♥ → 4♥) | 4-es support és 0–5 pont. Preempt. |
| Szín sima emelése (2♥ → 3♥) | 3-as vagy 4-es support, kb. 6–13 pont. Preempt. |
| Új szín (2♥ → 2♠) | 10–15 pont. Nincs supportod, legalább 5-ös hosszúság, egy körig forcing. |
| 2NT ([OGUST](#ogust--válaszok-az-induló-kérdésére-2--2nt--)) | 15+ pont, mesterséges királykérdés a partner színében. |

#### OGUST – válaszok az induló kérdésére (2♥ → 2NT → ?)

| Induló licitje | Jelentés |
| :---- | :---- |
| 3♣ | Gyenge kéz (5–7 pont), egy a top 3 honor közül a színében. |
| 3♦ | Gyenge kéz (5–7 pont), kettő a top 3 honor közül. |
| 3♥ | Jó kéz (8–10 pont), egy a top 3 honor közül. |
| 3♠ | Jó kéz (8–10 pont), kettő a top 3 honor közül. |
| 3NT | Jó kéz (8–10 pont), mindhárom top honor. |

### B) Válaszok közbeszólás esetén – Lebensohl gyenge 2-es ellen

Ha az ellenfelek közbeszóltak a gyenge 2-esre adott takeout double-re, akkor a Lebensohl relay-t használjuk.

**Helyzet:** **Ellenfél** gyenge 2-es nyitott → **partner** takeout-X → **ellenfél** passz → **te** válaszolsz, és pl. 8+ HCP-d van.

**Példa:** (2♥) – X – (Passz) – ?

| Te licited | Erő | Forcing? | Stopper? | Jelentése |
|---|---|---|---|---|
| **Passz** | – | – | – | Penalty pass (jó kőr-tartás) |
| **2♠** | 0–7 | NF | – | 4+ pikk, gyenge |
| **3♣ / 3♦** (közvetlen) | 8+ | F | – | 4+ lap, **konstruktív/inv+** |
| **2NT** | 0–7 | F | – | Lebensohl relay → 3♣ → kérdés/lezárás |
| **3♣ után gyenge folytatás** (passz / 3♦ lezárás) | 0–7 | NF | – | Gyenge kéz, menekülés |
| **3♥ (cue, közvetlen)** | 10+ | GF | Kérdez | "Stayman jellegű" — kérdezi a másik nemest / stoppert |
| **3♥ (cue, Lebensohl után)** | 10+ | GF | Kérdez | Ugyanaz, de van stopper-implikáció |
| **3NT** (közvetlen) | 10+ | – | NINCS | GF, nincs stopper |
| **3NT** (Lebensohl után) | 10+ | – | VAN | GF, van stopper |
| **3♠** | 10+ | GF | – | 5+ pikk, GF |

**Memorizálási szabály:** *„Cheap and fast = no stopper, slow via 2NT = stopper."*

---

## Erős 2 treff indulás

**Feltételek (legalább az egyik teljesüljön):**

- **22+ HCP**, balanced eloszlás (5-3-3-2 vagy lazább) — bár balanced kéznél 22–24 HCP-vel inkább 2♣ → 2NT a tisztább út, mint közvetlen 2NT (ami csak 20–21), VAGY
- **19+ HCP** + erős eloszlás (5+ lapos szín és/vagy 4-5 színhossz) + **9+ playing tricks** („1 ütés hiányzik a gémhez").
- A 2♦/2♥ válasz kivételével minden licit természetes és game forcing.

> 💡 **Mit jelent „1 ütés hiányzik a gémhez"?** Egy 4-major gémhez 10 ütés kell. Ha a saját kezedben (a partner segítsége nélkül!) látsz **9 biztos vagy szinte biztos ütést**, akkor a partnertől már csak **1 ütés** kell — ezt a kezet pedig veszélyes 1-es szinten megnyitni, mert a partner *passzolhatja* a sima 1-es nyitást. A 2♣ erős nyitás **kötelező válaszra szólít fel**, így biztosan nem maradsz 1-es szinten.

**Mi NEM erős 2♣ (gyakori tévedés):**

- ♠ AKQ54 ♥ AQ32 ♦ KQ ♣ 84 — **20 HCP, balanced**, de balanced kéznél 2NT (20–21) a helyes! Ez **2NT (Stop)**.
- ♠ AQ8543 ♥ AKQ ♦ Q72 ♣ 4 — **17 HCP, 6-os pikk, ~7 playing trick**. Ez **1♠** + reverse rebid (mert a kifelé 7 ütés *nem* 9). NEM 2♣.
- ♠ AKQ7654 ♥ AKJ ♦ 7 ♣ Q5 — **18 HCP, 7-es pikk, ~9 playing trick**. **EZ 2♣!** (A kéz önmagában szinte gémet játszik.)

### Válaszok a 2♣ indulásra (2♣ → ?)

| Licit | Jelentés |
| :---- | :---- |
| 2♦ | Negatív válasz, 4–7 pont, nem ígér kárót. Nem passzolható. |
| 2♥ | **Dupla negatív** válasz, 0–3 pont, nem ígér kőrt. Nem passzolható. |
| 2♠ | 8+ pont, 5-öt ígér a pikkből, game forcing. |
| 2NT | 8–11 pont, balanced, game forcing. |
| 3♣ / 3♦ | 8+ pont, 5-öt ígér a színből, game forcing. |
| 3♥ | 8+ pont, 5 kőrt ígér. |
| 3NT | 12–15 pont, balanced. |

### Az induló viszontválaszai a 2♦ negatív válaszra (2♣ → 2♦ → ?)

**Helyzet:** 2♣ (22+ HCP / 9+ ütés erős nyitás) – 2♦ (negatív/várakozó válasz) – ?

| Nyitó viszontválasz | Jelentés | Forcing? |
|---|---|---|
| **2♥** | 5+ kőr, 22+ HCP **vagy** ütésszám-nyitás | F-1 körig |
| **2♠** | 5+ pikk, 22+ HCP | F-1 körig |
| **2NT** | **22–24 HCP**, kiegyensúlyozott | NF (de a válaszadó folytathat) |
| **3♣** | 5+ treff, 22+ HCP | GF |
| **3♦** | 5+ káró, 22+ HCP | GF |
| **3♥ / 3♠** | Ugró nemes — 8+ lapos szín / nagyon erős színes kéz (ritkábban: solid suit) | GF |
| **3NT** | **25–27 HCP**, kiegyensúlyozott — `gamble` jellegű (válaszadó passzolhat) | NF |
| **4♣ / 4♦** | Splinter / kétszínű (ritkán; gyakran 5-5-ös) | GF |
| **4♥ / 4♠** | Lezáró gém — solid 8-9 lapos szín | NF |

**Folytatás 2NT (22–24 bal) után:** Pontosan úgy, mint egy 2NT nyitás után — Stayman (3♣), Jacoby transzfer (3♦/3♥), Puppet (?), stb. A 22–24-es tartomány gémszintet kényszerít, ha a válaszadónak 4+ HCP-je van.

**Folytatás 3NT (25–27 bal) után:** Hasonló rendszer, de még magasabb szintről. A válaszadó kvantitatív 4NT-vel slam-érdeklődést jelez (26+ kombinált).

### Az induló viszontválaszai a 2♥ dupla negatív válaszra (2♣ → 2♥ → ?)

**Helyzet:** 2♣ – 2♥ (**dupla negatív**: 0–3 HCP, **nincs ász és nincs király**) – ?

> ⚠️ Ez a válasz egyértelműen lerontja a slam-esélyt — a nyitónak nem szabad túlságosan optimistának lennie.

| Nyitó viszontválasz | Jelentés |
|---|---|
| **2♠** | 5+ pikk, GF (de slam már valószínűtlen) |
| **2NT** | 22–24 HCP balansz — a partner gyakorlatilag passzolja, hacsak nem nagyon shape-es |
| **3♣ / 3♦** | 6+ lap mellékszín, GF — partner egyszínű választ adhat |
| **3♥** | 6+ kőr, GF (kőr az adu — de óvatosan a slammal) |
| **3♠** | 6+ pikk, GF |
| **3NT** | 25–27 HCP balansz — passzolható |
| **4♣ / 4♦** | Splinter / kontroll-cue (ritkábban) |
| **4♥ / 4♠** | Lezáró gém — solid 8+ lapos szín, slam nem reális |
| **4NT** | Kvantitatív 6NT-meghívás (a partner passzol) |

**Gyakorlati tanács:** dupla negatív után gondolj a gémben-marasztalás stratégiájára — slam-vadászat csak akkor, ha a kezed önállóan 11+ ütésű (pl. solid 8+ lapos szín + 2-3 oldalütés).

### Egyéb megfontolások az erős 2 treff után

**2/3NT pontjelzés:** bármilyen válasz után az induló 2NT/3NT/4NT licitje pontot jelez (22–24 / 25–27 / 28–30, stb.).

---

## 2/1 Game Forcing és Reverse Bidding

Ezek a modern standard versenybridge alapvető rendszerei.

### 2/1 Game Forcing (Kettő az egyre Game Force)

Ha a partner 1-es szinten nyit (1♦, 1♥, 1♠), és te **ugrás nélkül, 2-es szinten egy alacsonyabb rangú új színt** mondasz be, az azonnali **Game Forcing (GF)**.

- **Példák:** 1♠ → 2♣, 1♥ → 2♦, 1♠ → 2♥.
- **Ígér:** Minimum 13+ HCP (Game érték).
- **Előnye:** Mivel már a 2-es szinten kiderült, hogy biztosan gémig (vagy slemig) fogtok licitálni, onnantól kezdve egyetlen licit sem passzolható el gém alatt! Lassan, kapkodás nélkül mutathatjátok be a színeket, egykéket, fogásokat.

> 💡 **Speciális kivétel:** Az 1♠ → 2♥ NEM 2/1 GF, mert a 2♥ a pikkre nézve magasabb rangú (reverse). Sok pár ezt mégis 2/1 GF-ként játssza – csapaton belül megegyezés kérdése.

### Reverse Bidding (Fordított licit)

Mikor a nyitó a második licitjével **magasabb rangú színt mond be, mint az első**, ráadásul kettes szinten.

- **Példa:** Nyitó 1♣ → Segítő 1♠ → Nyitó **2♦**. (A káró magasabb rangú a treffnél; ha „normális" sorrendben lett volna bemondva, azt 1♦ nyitással kellett volna kezdeni.)
- **Ígér:** Minimum **17+ HCP**.
- **Eloszlás:** Az első szín (treff) MINDIG hosszabb, mint a második (káró), tehát 5+ treff és pontosan 4 káró.
- **Szabály:** A Reverse licit a segítő számára legalább 1 körig **forcing, tilos elpasszolni!**

> 💡 **Tipp:** Ha 16–17 HCP-d van és reverse-ed lenne, gyakran jobb 1NT-vel rebid-elni (11–14 tartományba). 17+ HCP-vel viszont KÖTELEZŐ reverse-elni, hogy a partner ne álljon meg gém alatt.

---

## Slamkereső konvenciók

Ha megegyezett az adu szín, a slam-keresés célja megállapítani a kulcslapokat (4 ász + az ADU KIRÁLY = **5 kulcslap**).

<a id="kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430"></a>
### Kickback (helyett 4NT!) – Roman Key Card Blackwood (RKC) ászkérdés – 1430

Mi **Kickback**-et játszunk (a Minorwood helyett is ezt alkalmazzuk egységesen)!

- **Lényeg:** Az ászkérdés (RKC) a megegyezett aduszín fölötti **legolcsóbb, következő licit a 4-es szinten**. Nem a hagyományos 4NT.
  - Ha ♠ az adu → **4NT** az ászkérdés.
  - Ha ♥ az adu → **4♠** az ászkérdés.
  - Ha ♦ az adu → **4♥** az ászkérdés.
  - Ha ♣ az adu → **4♦** az ászkérdés.
- Ha még nem egyeztünk meg, akkor 4-es szintű ugrás → megegyezés ÉS ászkérdés egyben.

**Válaszok a Kickback ászkérdésre (1430 lépcsők):** A kérdő licittől számoljuk a „lépcsőket" felfelé.

| Lépcső | Jelentés (Kulcslapok száma) |
| :---- | :---- |
| 1. lépcső | **1** vagy **4** kulcslap (key card) |
| 2. lépcső | **0** vagy **3** kulcslap |
| 3. lépcső | **2** vagy **5** kulcslap, adu dáma NÉLKÜL |
| 4. lépcső | **2** vagy **5** kulcslap, adu DÁMÁVAL |

### Exclusion Blackwood

**Mikor használjuk?** Ha a partnerség megegyezett az aduban, de az egyik játékosnak **színhiánya (void)** van egy oldalszínben. Ilyenkor azt akarja megtudni: *„Hány kulcslapod van, NEM SZÁMÍTVA az én színhiányos színem ászát?"*

- **Hogyan licitáljuk:** Az adu megegyezése után egy **szokatlan, 5-ös szintű ugrás** egy új színben.
- **Példa (Egyszerű):** 1♠ – 3♠ (Limit emelés) – **5♣!** (Exclusion: „Pikk lesz az adu. Treff voidom van, mondd a kulcslapjaid a treff ász kivételével.")
- **Példa (Összetett):** 1♥ – 2NT (Jacoby) – 3♦ (Káró egyke/hiány) – 4♥ (Rossz, sign-off) – **5♣!** (Az erős nyitó treff Exclusiont mond; a 3♦ csak puhatolózás volt.)
- **Válaszok:** A válaszoló a sima [1430 lépcsőket](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430) használja, de úgy tesz, mintha az Exclusion szín ásza nem létezne a pakliban (ha mégis nála van, azt zérónak értékeli).

### Void válaszok 1430-ban

Ha a *segítőnek* van színhiánya (nem a kérdezőnek), az alábbi módon jelezheti a Kickbackre:

![Void-válaszok lépcsőszerkezete az RKC 1430-ra](https://github.com/imre-nicowl/Bridge/blob/main/Pics/void_RKCB.png)
<!-- IMAGE PLACEHOLDER: 12. ábra – Void-válaszok lépcsőszerkezete az RKC 1430-ra (5NT = páros void számú kulcslap, 6 új szín = void abban a színben, 6 adu = páratlan void). -->

### 5NT Specific King Ask (Királykérdés Kickback után)

Miután a Kickback-ből kiderült, hogy a partnerségnél megvan az összes kulcslap, a nagyslem lehetőségének vizsgálatára a kérdező **5NT**-t licitál (bármi is volt a Kickback szintje). Ez a **Specific King Ask**.

- **Válasz:** A segítő a 6-os szinten **bemondja azt a konkrét színt**, amelyikben a királya van (pl. 5NT → 6♦ = Káró királyom van).
- Ha több királya is van, a legolcsóbbat (legalacsonyabb rangút) mondja be.
- Ha *nincs* külső királya (az adu királyt már beszámoltuk a Kickback-be!), akkor egyszerűen visszatér az aduszín 6-os szintjére.

### Adu dáma megkérdezése RKC-ra érkezett válasz után

Az RKC-t licitáló megkérdezheti az adu dámát is a legolcsóbb új színnel. Válasz:

- **Adu szín visszahívása:** Nincs nálam.
- **5NT:** Itt a dáma ÉS nincs másik színből király.
- **Bármelyik nem adu szín:** Itt a dáma ÉS a licitált színből a király.

### Gerber (szanra adott) ász- és királykérdés

> 💡 **EZ GYAKORLATILAG KICKBACK SZAN UTÁN!**

Csak **1NT / 2NT nyitásra** lehet mondani. Cél: meg lehessen állni 4 vagy 5 szanon, ha nincs slem.

- A **4♣** a Gerber ászkérdés.
- Válaszok: 4♦ = 0 vagy 4, 4♥ = 1, 4♠ = 2, 4NT = 3.
- Az **5♣** a királykérdés (ugyanezzel a lépcsőszerkezettel).

> ⚠️ Ezért lett az [1NT – 4NT](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül) kvantitatív (nem ászkérdés)!

### Ha közbeszóltak az ászkérdésre – DEPO

**DEPO = Double = Even, Pass = Odd.**

- **Kontra (X):** 0, 2 vagy 4 ász (Páros – Even).
- **Passz:** 1 vagy 3 ász (Páratlan – Odd).

### Cuebid – első- és másodkörös kontrollok

A slamkeresés gyakran nem csak ászról és királyról szól, hanem szinkronizált **kontroll-mutogatásról**, ami az [Italian-style cuebid](https://en.wikipedia.org/wiki/Cue_bid) része:

- **1. körös kontroll** = ász vagy void (az első ütésből 0 megy el).
- **2. körös kontroll** = király vagy szingli (az első ütésből 1 megy el, a másodikból már 0).
- **Italian-style cuebid:** 1. és 2. körös kontroll keverten mutogatható; ez különbözik a klasszikus, „csak 1. körös kontroll" amerikai stílustól.
- **Sorrend:** Az ász-egyezés (vagy adu-egyezés) után a **legalacsonyabb, még meg nem mutatott** kontrollt mutatjuk. Ha átugrunk egy színt, az azt jelenti, hogy abban nincs kontrollunk!

**Példa licitsorozat:**

| Induló | Segítő | Megjegyzés |
| :---- | :---- | :---- |
| 1♠ | 3♠ (limit raise) | 10–12 HCP, 4 lapos pikk fit |
| 4♣ | | „Treff kontrollom van (ász vagy egyke)." |
| | 4♦ | „Káró kontrollom van; treffem nincs, vagy később mutatom." |
| 4♥ | | „Kőr kontrollom is van!" |
| | 4♠ | „Nincs több kontrollom, álljunk meg a gémnél." vagy 4NT (RKC, ha látom esélyét) |

> 💡 **Fontos:** Ha a partner cue-bid-et csinált egy színben, az implicit megegyezést jelent az aduban — onnan a folytatás bármilyen 4-es szintű cue-bid kontrollt ígér.

---

## Overcallok és kompetitív licitek

A cél, hogy kompetitív licit alakuljon ki: vagy nekünk érje meg játszani, vagy az ellenfelet rávenni magasabb szinten való megállásra.

### Áttekintő pont-diagram

![Áttekintő pont-diagram: overcall / takeout double / 1NT overcall / cue bid mátrix.](https://github.com/imre-nicowl/Bridge/blob/main/Pics/overcall.png)
<!-- IMAGE PLACEHOLDER: 13. ábra – Áttekintő pont-diagram: overcall / takeout double / 1NT overcall / cue bid mátrix. -->

### Szín bemondása (overcall)

| Helyzet | Pont | Hossz | Szín-minőség | Megjegyzés |
|---|---|---|---|---|
| **1-es szintű overcall** (pl. 1♣ – 1♠) | 8–17 HCP | 5+ lap | 2 honor: KQxxx, AJxxx, KJTxx | Legszélesebb tartomány |
| **2-es szintű overcall** (pl. 1♠ – 2♣) | 11–17 HCP | 5+ lap (általában 6) | 3 honor vagy 6+ lap: KQJxx(x), AKxxxx | Diszciplináltabb |
| **Ugró overcall** (1♣ – 2♠) **gyenge** | 6–10 HCP | 6+ lap | Jó szín (2 honor) | Modern stílus: **gyenge ugrás** = preemptív |
| **Ugró overcall (klasszikus erős)** | 16+ HCP | 6+ lap | – | Csak speciálisan megállapodva |
| **1NT overcall** (1♣ – 1NT) | **15–18 HCP** | balansz | Stopper a közbeszólt színben | A felső sáv ≈ erős 1NT nyitás |
| **2NT overcall** (1♣ – 2NT) | – | – | – | **Unusual NT**: kétszínű (a 2 alsó / 2 alsó nem-licitált) |
| **Cue-bid overcall** (1♣ – 2♣) | 16+ HCP | – | – | **Michaels**: kétszínű, lásd Michaels szakasz |
| **Take-out X** | 12+ HCP | rövid közbeszólt szín | – | A három másik szín támogatása |

**Példák:**

```
LHO: 1♣
Te: KQ954 / 73 / KQT2 / 94  → 1♠ overcall (✓ 5 lap, 2 honor, 11 HCP)
Te: AQ7 / KJ7 / KJ87 / Q97  → 1NT overcall (✓ 15 HCP, balansz, stopper)
Te: KQJT98 / 7 / Q3 / K842  → 2♠ ugró overcall, ha gyenge-ugrást játszotok (6 lap, 9 HCP)
```

**Általános feltételek:**

- **1-es szinten:** 8–17 HCP, jó 5+ lapos szín (általában 2 honor: pl. KQxxx vagy AJxxx).
- **2-es szinten:** 11–17 HCP, kiváló 5+ lapos szín (általában 3 honor vagy 6+ lap).
- **Ugró overcall (1♣ – 2♠):** „Erős, 1-szintű nyitást megelőző gyenge 2-es" — 6 lapos szín, 6–10 HCP (gyenge ugró overcall, ami a leggyakoribb modern stílus).

### Take-out Double

12–15 (11+) pont, 3-3 minden be nem mondott színből. A partnernek kötelező válaszolnia:

- **Passz:** 0–6 pont, az ellenfél színe nálunk hosszú, büntető szándék.
- **Alacsony szín:** 0–9 pont.
- **Ugrás színben:** 10–12 pont, invitáló.
- **Cue bid:** 13+ pont, Game Forcing.

### 1NT és 2NT overcall

| Licit | Jelentés |
| :---- | :---- |
| 1NT overcall (1♥ – 1NT) | 15–18 HCP, balanced, **biztos stopper** az ellenfél színében. Stayman + transfer érvényben (mint sima 1NT nyitás után). |
| 2NT overcall (1♥ – 2NT) | NEM természetes! [Unusual 2NT](#michaels-cue-bid--unusual-2nt-vs-védekezés-unusual-vs-unusual) – két alsó szín. |
| Ugró 2NT direkt nyitás után (passz után) | Természetes, 19–20 HCP. |

### Power Double (Erős Kontra, 16+ HCP)

A standard 12–15 pontos Take-out Double mellett létezik a „Power Double" (16+ HCP-vel). Ennek ereje a *második körben* derül ki.

**Licitsorozat:** 1♦ (Ellenfél) – **Kontra (Te)** – Passz – 1♠ (Partner, gyenge 0–9) – Passz – **?**

**Második licited:**

- **Új szín (pl. 2♥):** 16–18 pont, erős 5+ lapos kőr.
- **1NT:** 19–21 HCP, balanced eloszlás, biztos fogás a káróban (az ellenfél színében).
- **2NT ugrással:** 22–24 HCP, balanced, fogás a káróban.
- **Partner színének emelése (2♠ vagy 3♠):** 16+ pont és minimum 4 lapos fitt a partner (pikk) színében.

### Take-out Double 4-es magasan

Ha az ellenfél 4 nemest nyit közvetlenül (pl. 4♥), a kontra **általában takeout** (12+ HCP, 0–2 a kontrázott színben, 3+ a többi színben).

> ⚠️ Ez NEM tisztán büntető — a partnernek el kell tudni dönteni passz / 4♠ / 5♣ / 5♦ között. 4♠ közbeszólás esetén már jellemzően penalty doubleról beszélünk, mert a saját 4♠ licit túl drága lenne.

**Helyzet:** (4♥) – X – ? **vagy** (4♠) – X – ?

| A kontra jellemzői (kontrázó) | Érték |
|---|---|
| HCP | **12+** (általában 14+) |
| Hossz a kontrázott színben | 0–2 lap |
| Hossz a többi 3 színben | **3+ minden színben** (ideális: 4-3-3-3 vagy 4-4-3-2) |
| Erő | Cooperative — *nem* tisztán büntető |

| Partner válasza (X-er partnere) | Mikor? |
|---|---|
| **Passz** | 4+ jó lap a kontrázott színben (penalty conversion) |
| **4♠** (4♥ X után) | 4+ pikk, 0–8 HCP |
| **5♣ / 5♦** | 5+ lap, 0–8 HCP |
| **4NT** | Kétszínű mutatás vagy "válassz a két alsóból" |
| **5♥** (4♥ X után, cue) | Kérdez slam felé / két-színű kéz |

> ⚠️ **4♠ közbeszólás esetén** (vagyis (4♥) felett 4♠ overcall) a kontra már **penalty** — mert 4♠-t licitálni költséges lenne, így a kontra inkább büntető szándékú.

| Helyzet | A kontra értelme |
|---|---|
| (4♥) – X | **Take-out** (cooperative) |
| (4♠) – X | **Penalty** (gyengébb takeout, vagy "kártyák", a partner általában passzol) |
| (4♣) – X | **Take-out**, 3-3-3 a többi színben |
| (4♦) – X | **Take-out** |

---

### Újranyitó kontra (Reopening Double)

**Mikor használjuk?** A licit kezd „elhalni" az 1-es szinten.

**Példa:** 1♣ – Passz – Passz – **X!**

- **Lényege:** Az induló partnere passzolt, azaz neki alig van pontja (0–5). Ez azt jelenti, hogy a mi oldalunkon megvannak a pontok (gyakran 20–22 pont együttesen), csak a te partnerednek olyan lapja volt (csapda passz, vagy nagyon lapos rossz eloszlás), amivel nem tudott rögtön közbeszólni.
- **Követelmény:** 8–14 pont és **rövidség** az ellenfél által megnyitott színben, hogy a partner bármit mond, jó legyen neked.
- **Válaszok a passzoló partner részéről:**
  - *Legolcsóbb szín bemondása:* Gyenge, továbbra sincs sok pontja (0–8).
  - *Ugrás színben:* Invitáló (9–11 pont).
  - *Passz:* Ez az úgynevezett **Büntető Passz (Penalty Pass)**. Akkor húzza meg a partner, ha az ellenfél induló színéből rettentő hosszú, gyönyörű lapja van, amivel alacsony szinten, kontrázva akarja megbuktatni a felvevőt!

### Support Double

Akkor jön szóba, ha:

1. Te nyitottál nemest (pl. 1♠).
2. A partner új színt válaszolt (pl. 1NT → ez nem releváns; viszont egy 1♥ – 1♠ – 2♦ után a 2♦ szintén nem; ez a sorozat: 1♣ – Passz – 1♥ – 1♠ – ?)
3. Az ellenfél közbeszólt a saját partnered színe FÖLÉ.
4. **A te X kontrád ekkor pontosan 3 lapos fittet ígér** a partner színében (a 4 lapos fit ugyanis 2♥-re emelést jelent).

**Példa:** 1♣ (Én) – Passz – 1♥ (Partner) – 1♠ (Ellenfél) – **X** = pontosan 3 kőröm van.

**Helyzet:** Te nyitottál nemest / alsót → partner 1-szintű új színt válaszolt → ellenfél *közbeszólt a partner színe felé* → te döntesz.

**Példa-szekvencia:** 1♣ (én) – Passz – 1♥ (partner) – 1♠ (ellenfél) – **?**

| Lapok száma a partner színében | Helyes licit | Jelentés |
|---|---|---|
| **3 lap** | **X** (Support Double) | "Pontosan 3 köröm van" — semleges erő (12–17 HCP) |
| **4 lap** | **2♥** | "4 kőr fit, minimum (12–14 HCP)" |
| **4 lap, erős** | **3♥** (ugró raise) | "4 kőr fit + max (15–17), invitációs" |
| **4 lap, GF** | **4♥** | Lezáró gém |
| **4 lap, slam-érdeklődés** | **Splinter** (3♠ pl.) | Rövidség + 4 kőr |
| **Nincs 3+ kőr** | Természetes licit (1NT, 2♣, 2♦, X penalty, stb.) | Nincs fit |

> 📌 **Magyarázat:** Mivel a 2♥ emelés *garantáltan* 4 lapos fitet ígér (Support Double rendszerben), a X-kontra az egyetlen módja a 3 lapos fit közlésére. Enélkül a partner nem tudná megkülönböztetni a 3 és 4 lapos fit-et.

**Support Re-double (XX):** Ha az ellenfél *kontrázott* a partner válaszát (nem új színt mondott):
- **XX** = pontosan 3 lapos fit a partner színében
- **Raise (2♥)** = 4 lapos fit

### Two-suited Double

Olyan kontra, ami **két konkrét színt** ígér. Általában csak speciálisan megbeszélt szekvenciákban van értelme — pl. ellenfél [Cappelletti](#védekezés-1nt-indulás-ellen--cappelletti) 2♥ overcall-jára (kőr + alsó) a kontra büntető, vagy a Cappelletti 2♦ (nemesek) kontrázása nemes-bizonytalanságot jelez.

| Szekvencia | A X jelentése |
|---|---|
| **(1♣) – X – (XX) – ?** Te X-eltél = **takeout** (klasszikus) | Eredeti X: 12+, 3+ a többi színben |
| **(1NT) – X** | **Penalty / kártyák** (15+ HCP, főleg ász-király kombinációk) |
| **(1NT) – (2♣ Cappelletti, egyszínű) – X** | **Penalty** (ők egyszínűt jeleznek, te 4+ trefföt jelzel) |
| **(1NT) – (2♣ DONT, 5+ treff vagy 4-4 alsó-nemes) – X** | **Stayman/kártyák** (8+ HCP, 4-es nemes vagy büntetés) |
| **(1NT) – (2♦ Cappelletti, nemesek) – X** | **Penalty** (4+ káró) |
| **(1NT) – (2♥ Cappelletti, kőr+alsó) – X** | **Penalty kőrre** (4+ kőr — náluk valószínűleg shortness) |
| **(1NT) – (2♠ Cappelletti, pikk+alsó) – X** | **Penalty pikkre** (4+ pikk) |
| **1♥ – (2♥ Michaels, pikk+alsó) – X** | **Penalty** (4+ kőr, vagy ász-király az ellen-színekben) |
| **1♣ – (2♣ Michaels, nemesek) – X** | **"Karták"**, általában a kőr+pikk *ellen* |
| **1♥ – (X takeout) – XX** | Saját **erős XX**: 10+, nincs fit |
| **(1♥) – 1♠ – (2♥) – X** | **Cooperative / responsive** (8+, nem tudja mit, kérdezi a partnert) |

**A Two-suited double általános elve:** ha az ellenfél *kétszínű* konvenciót használ (Cappelletti, Michaels, DONT, Unusual NT), akkor a saját **X** és **cue-bid** specifikus üzeneteket kap:
- **X**: kártyák / penalty az egyik konkrét színre
- **Cue (alsó)**: gémforce, nincs stopper
- **Cue (felső)**: gémforce, van stopper

### Negatív kontra (overcaller partnereként)

Lásd: [A Segítő szabályai – Negatív kontra](#negatív-kontra-a-standard-sayc-b-konvenció). Pontosan 4 lapos másik nemest ígér.

### Rekontra (erős)

Ha az ellenfél takeout double-t mondott a te nyitásodra, és te a partnered helyzetében vagy:

- **Rekontra (XX):** 10+ HCP, *nincs* támogatás a partner színéből. Egy körig forcing; a következő licit pozitívan jellemző (büntető szándék, ha még egy alacsony lapot ki tudsz adni).
- Egy körig kötelező, hogy a partner megszólaljon — a partner *nem* mondhat passzot, hacsak nem kontrázni akarja a hamarosan rákövetkező ellenfél licitet.

**A) Azonnali XX – partner takeout double-jét követően**

**Helyzet:** Én 1♥ – (X takeout) – ?

| Válaszadó licit | Erő | Jelentés |
|---|---|---|
| **Passz** | 0–5 | Nincs jó licit |
| **1♠ / 1NT / 2♣ / 2♦** | 0–8 | Természetes, NF (a kontra "letörli" a megszokott jelentést) |
| **2♥** (sima emelés) | 6–9 | 3+ kőr fit, konstruktív |
| **3♥** (ugró emelés) | gyenge | 4+ kőr, preemptív (defenzív) |
| **2NT** (Jordan / Truscott) | 10+ | 4+ kőr fit, GF |
| **XX (rekontra)** | **10+ HCP** | **Nincs fit**, forcing 1 körig — büntető szándékkal "védjük meg" |
| **4♥** | gyenge, shape-es | 5+ kőr, preemptív |
| **Splinter (3♠, 4♣, 4♦)** | 10–13 | Rövidség + 4+ fit, GF |
| **Cuebid (2♣?? vagy közvetlen 3♣ stb.)** | – | Speciális megállapodás |

**Az XX (rekontra) utáni folytatás:**

```
1♥ – (X) – XX – (Passz / 1♠ / 1NT / 2♣ / 2♦)
                       ↓
                  Most a NYITÓ folytatja:
                   ├─ Passz: "kontrázni szándékozom"
                   ├─ Új színű licit: extra hossz, jelez
                   └─ Saját szín ismétlése: 6+ lap
```

**B) Második körös XX – ellenfél közbeszólta a partnered színét**

**Helyzet:** 1♥ – Passz – 1♠ – (2♥ közbeszólás) – ?

| Nyitó (én) licitje | Jelentés |
|---|---|
| **Passz** | Minimum, nincs leírnivaló |
| **X** | **Penalty** (4+ kőr a nyitónál — ritka, de erős) |
| **2♠** | 3 lapos pikk-fit, konstruktív |
| **3♠** | 4 lapos pikk-fit + max |
| **3♣ / 3♦** | Új szín, 4+ lap, F |

**C) Rekontra mint "kihívás" (SOS XX)**

**Helyzet:** Partnert *büntető-kontrázták*, és én *menekülni* akarok:

| Példa | Jelentés |
|---|---|
| 1NT – (X penalty) – ?? – (Passz) – **XX** | **SOS** (menekülés) — kérem a partnert, hogy válasszon szint |
| 4♠ – (X) – Passz – (Passz) – **XX** | **Konfidens** (extra erő, nincs ki kell mászni) |

**Memóriasegítő:**

- **Azonnali XX** (saját nyitásom után) = **10+ HCP, nincs fit, forcing 1 körig**.
- **Késleltetett XX / SOS XX** (3-as szint felett, vagy büntető-kontra után) = **menekülés** (gyenge, válassz színt!).

### Gyenge 2-re adott takeout double után – Lebensohl relay

**Helyzet:** Én 2♥ (saját gyenge 2-es nyitás) – (X takeout) – ?

| Válaszadó (partner) licitje | Erő | Forcing? | Jelentés |
|---|---|---|---|
| **Passz** | 0–5 | NF | Nincs jó licit, partner kicsi |
| **2♠** | 0–7 | NF | 5+ pikk, lezáró |
| **2NT** | 0–7 **vagy** 10+ | F-1 körig | **Lebensohl relay**: → 3♣ → ? |
| **3♣ / 3♦** (közvetlen) | 8–11 | F | Természetes, konstruktív |
| **3♥** (sima emelés) | 6–9 | NF | 3+ kőr fit, defenzív vagy konstruktív |
| **3♠** (ugró) | 10+ | F (GF) | 6+ pikk + kőr-fit (komplex jelentés) |
| **4♥** | gyenge | NF | Preemptív lezárás |
| **XX (rekontra)** | 10+ | F | Penalty-irány, nincs fit |
| **3NT** | 10+, balansz | – | Stoppert ígér, lezárás |

**A 2NT Lebensohl folytatása (kötelező 3♣):**

```
2♥ – (X) – 2NT – (Passz/3♣) – 3♣ kötelező – (Passz) – ?
                                              ↓
                       Most a VÁLASZADÓ folytatja:
                       ├─ Passz: gyenge, sign-off 3♣-ban
                       ├─ 3♦/3♠: 6+ lap, sign-off
                       ├─ 3♥ (cue): GF, fit-érdeklődés
                       ├─ 3NT: 10+, balansz, stopperrel
                       └─ 4♥: 4+ kőr fit, slam-irány
```

> 💡 **Magyarázat:** a saját gyenge 2-esünk ellen X esetén a partner gyakran *vakon* játszik. A 2NT relay megoldása lehetővé teszi, hogy a partner gyenge ÉS erős kézzel is jelezzen, anélkül hogy közvetlenül 3-as szintre menne.

### Michael's Cue bid + Unusual 2NT vs. Védekezés (Unusual vs Unusual)

**Michael's Cue bid (pl. 1♣ – 2♣):** 5-5 a nemesekben (ha minor volt a nyitás), vagy 5-ös a másik nemes és 5-ös az egyik minor (ha nemes volt a nyitás). 10+ pont.

**Unusual 2NT (pl. 1♠ – 2NT):** A két leggyengébb be nem mondott szín (jellemzően a két minor) 5-5 lapos fittje. 10+ pont.

**Védekezés az Unusual 2NT ellen (Ha ők mondják ránk):**

**Példa:** Mi nyitunk 1♠-t, erre az ellenfél bemondja a 2NT-t (két alsó). A segítő válaszai:

- **Kontra (X):** Büntető szándék. 10+ HCP-je van, és meg tudja fogni az ellenfél alsóit. Az ellenfelek nagy zűrbe kerültek.
- **Alsó Cue-bid (3♣):** Invitáló emelés a mi nemesünkben (Limit raise in Spades). Ha a nyitónak nem tetszik, egyszerűen mond egy 3♠-t (Sign-off).
- **Magasabb alsó Cue-bid (3♦):** Game Forcing (GF) emelés a mi nemesünkben.

### Védekezés 1NT indulás ellen – Cappelletti

A Cappelletti (1NT nyitás elleni közbeszólás) válaszai és a megfelelő verseny-folytatás:

| Cappelletti overcall | Licit | Segítő válasza |
| :---- | :---- | :---- |
| Egyszínű kéz (11–14p) | **2♣** | A segítő kötelezően (Relay) **2♦**-t mond. Az overcaller erre bemondja az 5+/6+ lapos igazi színét. |
| Mindkét nemes (5-4 v. 4-5) | **2♦** | A segítő bemondja azt a nemest, amelyikből több van (Pass/Correct). Ha egyenlő (pl. 3-3), **2♥**-t mond. |
| Kőr és egy Alsó (5-5) | **2♥** | A segítő, ha szereti a kőrt, passzol. Ha gyűlöli (0-1 lap), **2NT**-vel megkérdezi, mi az alsó szín. |
| Pikk és egy Alsó (5-5) | **2♠** | Mint fent, pikk preferenciával. Gyűlölet esetén 2NT kérdezi az alsót. |

---

## Egyebek – egyéb konvenciók

Lásd:
- [The Rule of 20](#the-rule-of-20)
- [The Rule of 44](#the-rule-of-44)
- [LTC és Zar Points](#lapérték-finomítás--ltc-és-zar-points)
- [Gyakori licitálási hibák](#gyakori-licitálási-hibák--anti-pattern-szekció)

---

## Ellenjáték (jelzések)

Mi az **upside-down** konvenciókat használjuk.

### Attitude (upside-down)

- **Encourage (bátorítás):** kicsit dobok, majd nagyot.
- **Discourage (elbátortalanítás):** nagyot dobok, majd kicsit.

### Count (upside-down)

- **Páros:** kicsi lapot dobsz.
- **Páratlan:** nagy lapot dobsz.

*(Szannál az első nem honor ütésnél a kicsi lap countot, nem attitude-öt ad.)*

### Suit-preference

- **Kicsi lap** = olcsóbb színre válts.
- **Nagy lap** = drágább színre válts.

---

## Slem- és game-erő megbeszélése

### The Law of Total Tricks

Kompetitív licitnél az aduszám határozza meg a biztonságos szintet (8 adu = 2-es szint, 9 adu = 3-as szint, stb.). Segít a gyors preempt kizárásoknál és a [Bergen Raises](#bergen-raises) rendszerben.

> **Total Tricks ≈ Total Trumps** (mi + ők együtt). Pl. ha nálunk 9 pikk + náluk 8 kőr van, akkor összesen ~17 ütés lehet a két felvételen együtt. Ha mi viszünk 9-et, ők visznek 8-at; ha mi viszünk 8-at, ők 9-et — ennek megfelelően nem érdemes 3♠-nál fennebb védekezni 3♥ ellen, ha 9-9 a fit-eloszlás.

<a id="drury-konvenció-passzolt-segítő"></a>
### Drury Konvenció (Passzolt segítővel)

Ha 3. vagy 4. helyen ülsz, a partnered nyithat egy „könnyített" (10–11 pontos), taktikai 1♥ / 1♠ licittel. Ha te már passzoltál (tehát max 11 pontod van), de van **3+ lapos fited** a nemesében és invitáló (10–11) kezed, **nem emelhetsz rögtön 3-as szintre**, mert el fogtok bukni, ha a partner könnyített nyitást csinált!

**Megoldás: A Reverse Drury (2♣)**

- A passzolt segítő **2♣** válasza a nemesre: *„Partner, 10–11 pontom van és 3+ támogatásom."*
- A nyitó válasza a 2♣-re:
  - **2♦:** *„Igazi, teljes értékű nyitásom van (12+ pont), mehetünk Gémre!"*
  - **A saját nemesének megismétlése (2♥/2♠):** *„Bocs, ez csak könnyített nyitás volt, álljunk meg itt, nincs Gém."*

### Western Cue bid (Stopper-kérés)

Mikor a licit során egyértelmű, hogy **3NT** a célunk, de van egy „veszélyes" szín az ellenfélnél, amiben nincs fogásunk (stopperünk), a legokosabb, amit tehetünk: **Licitáljuk be az ellenfél színét!**

- **Példa:** Észak 1♠ – Kelet 2♣ – Dél 2♦ – Nyugat Passz – Észak **3♣!**
- **Jelentés:** *„Partner, a te káróddal és az én pikkemmel 3NT a gémünk, de NINCS treff stopperem. Neked van?"*
- **Válasz:** Ha van stoppere, mond 3NT-t. Ha nincs, folytatja a licitet (pl. bemondja Észak pikkjét).
- **Fontos különbségtétel:** A Western Cue mindig egy *későbbi, reagáló* fázisban történik. Ha *azonnal*, az első adandó alkalommal licitálod rá az ellenfél színére a saját licitjét (pl. 1♥ – 2♥), az a [Michael's Cue bid](#michaels-cue-bid--unusual-2nt-vs-védekezés-unusual-vs-unusual) (két színű 5-5).

### Splinter bids

**Dupla ugrás új színben:** egy van a licitált színből (singleton vagy void) és 12+ pontot ígér. Slem kutatás.

**Példa:** 1♠ → 4♦ = „4 pikkem van, 12+ HCP, és káróból egykém vagy színhiányom van."

> ⚠️ **Vigyázat:** A splinter ász szingli (pl. ♦A egyedül) gyakran *rossz* hír, nem jó: a duplikálódik az értékkel (az ász már a HCP-ben szerepel, a shortness pedig még +2 pont). Ilyen kéznél splinter HELYETT inkább szín bemondás, vagy direkt [Jacoby 2NT](#jacoby-2nt-segítőként-csak-nemes-nyitásra) érdemes.

### Fourth suit forcing (Negyedik szín forcing)

Cél: ne kelljen a negyedik szín ismerete nélkül 3NT-t játszani – mondj valami extrát a shape-edről. Feltétel: legalább 13 pont segítőként (GF).

---

## Pontozás

### Sebezhetőség (vulnerability) – licitkezdő szerint

| Licitkezdő | Sebezhetőség |
| :---- | :---- |
| North (N) | mindenki mans |
| East (E) | N/S mans, W/E bell |
| South (S) | N/S bell, W/E mans |
| West (W) | mindenki bell |

### Ütésenkénti pontok

| Vállalás | Ütésenkénti érték |
| :---- | :---- |
| Nem nemes (♣, ♦) | 20 pont/ütés |
| Nemes (♥, ♠) | 30 pont/ütés |
| Szan (NT) | Első ütés: 40 pont; további ütések: 30 pont |

### Bónuszok teljesítésért (mans / bell)

| Vállalás | mans (nem sebezhető) / bell (sebezhető) |
| :---- | :---- |
| Sima (nem game, azaz partial) | 50 / 50 pont (résrekord) |
| Game prémium (Mans / Bell) | **300 / 500 pont** |
| Kis slem prémium (a game bónuszon FELÜL) | **500 / 750 pont** |
| Nagy slem prémium (a game bónuszon FELÜL) | **1000 / 1500 pont** |

### Bukás ütésenként

**Kontra nélkül:** 50 (mans) / 100 (bell) pont/ütés.

**Kontrázott bukás:**

| Bukás (ütés) | Nem sebezhető (mans) | Sebezhető (bell) |
| :---- | :---- | :---- |
| 1. ütés | 100 | 200 |
| 2. ütés | 200 | 300 |
| 3. ütés | 200 | 300 |
| 4. és további | 300 / ütés | 300 / ütés |

**Rekontrázott bukás:** a fenti kontra-értékek **duplázódnak** (100 → 200, 200 → 400, 300 → 600).

### Kontra hatása

- Megduplázza az alap ütések és a bukások értékét. Teljesítéséért 50/100 pont jár (**insult bonus**).
- **Nem** duplázza a gém-, kis- és nagyszlem-prémiumokat.

### Rekontra hatása

- Négyszerezi az alap ütések és a bukások értékét. Teljesítésért 100/200 pont jár.
- **Nem** négyszerezi a gém-, kis- és nagyszlem-prémiumokat.

---

## Játékmenet alapok

### Impassz (finesse)

Tipikusan figura-lyuk kijátszása/kijátszatása.

**Direkt impassz:**
Az ellenfél indul alacsony, beleteszed a dámádat. Ha az ellenfél kijön a királyával, ásszal viszed → bukta a királyt. Ha nem jön ki a királlyal, akkor elviszed a dámával, és megmarad az ászod… vagy bukod, de versenyen ezt mindenki megjátssza, és mindenki elbukik, tehát nincs probléma.

**Indirekt impassz:**
A partnered színnel indul a királyod felé. A közöttetek lévő ellenfél vagy beleteszi az ászát (üt, és felnő a királyod), vagy nem teszi bele (és a királyod viszi az ütést). Így mindenképp győztesen hozod ki a királyod.

### Hogyan nyitunk

- **Szan ellen:** A leghosszabb színből a 4. legnagyobb lap, vagy honor sequence tetejéből (pl. KQJx).
- **Színjáték ellen:** Színhiányból próbálunk nyitni (amiből 1-2 van), általában előbb a nagyobb lap. Erre normál körülmények között illik visszahívni a partner színét.

### Osztás és lejátszás

- **Osztás:** óramutató járásával megegyezően, 1-1 laponként, 13-13-13-13 lapot.
- **Lejátszás:** aki a licitet nyerő párosból a nyertes színt (vagy szant) először játékba hozta, az lesz a felvevő. A partnere lesz a terítő (asztal). A felvevőtől balra ülő ellenfél hív először; az asztal lepakol, és onnan folytatja a felvevő.

---

<a id="lejátszási-taktikák"></a>
# 🎴 Lejátszási taktikák

> Ez a fejezet az új r3.0 verzió legnagyobb bővítése. A bridge lejátszási oldalának ismerete legalább annyira fontos, mint a licit. Az alábbi 11+ technika gyakorlatilag minden komolyabb szerződésnél felmerül.
>
> **Ajánlott források:**
> - [mapiano.com/coup.htm](https://www.mapiano.com/coup.htm) – Coup-ok és defenzív technika.
> - Hugh Kelsey: *Squeeze Play in Bridge* — a klasszikus.
> - Kelsey & Ottlik: *Adventures in Card Play* — haladó squeeze és coup tartalom.
> - Reese: *The Expert Game* — counting és inferencia.

## Endplay (kényszerkijátszás)

**Lényeg:** Az ellenfelet olyan helyzetbe kényszerítjük (throw-in), hogy bármit játszik, ütést ad nekünk – vagy az adusora tetejét, vagy a saját stopper-színünket vezeti (esetleg ruff-and-discard-ot ad).

**Tipikus elemek:**

- **Throw-in card:** az a lap, amellyel beadjuk az ellenfelet (pl. ász vagy király kihajítva neki).
- **Endplay-állás:** az ellenfélnek csak olyan színe maradt, amelyikbe vezetni neki *rossz*.
- **Eliminációs lejátszás:** a „semleges" színek (pl. dupla-dupla) kihúzása, hogy ne tudjon mibe „menekülni".

### Példa endplay (egyszerű, klasszikus)

**Szerződés:** 4♠ (mans), kiadó káró királya.

```
                  ♠ AKQJ          ← dummy
                  ♥ A4
                  ♦ AQ32
                  ♣ 432

♠ x          ♠ x
♥ KJxx       ♥ Qxxx
♦ Kxxx       ♦ Jxx
♣ Jxxx       ♣ Q98x

                  ♠ xxxxx         ← felvevő
                  ♥ xx
                  ♦ xx
                  ♣ AKx
```

Ha simán fineszelünk a káró dámával nyugat felé, a király alulról elviszi, és bukhatunk. Helyette **endplay**:

1. **Adut húzunk:** ♠AKQJ — minden ellenfél követ, 4 ütés.
2. **Eliminációs treff:** ♣ A, K, és a 3. treffet a kezünkben **bemegyünk a dummyhoz** (de itt nincs treff a dummyban — pontosabban: ruff-oljuk a dummy harmadik treffjét? Itt csak 3 treffes a dummy, 3 kis lap; a kezünkben 3 treff: AKx. Tehát: ♣A, ♣K, harmadik kis lap kiadása → de ezt az ellenfél viszi.)
3. **Második iteráció:** Inkább a kőrt elimináljuk: ♥A, majd kiadunk egy kőrt. A nyugat felüt a ♥K-val.
4. **Most jön az endplay:** Nyugatnak már csak ♦Kxxx és ♣J marad (mondjuk). Ha treffet játszik, ruff-and-discard (a dummyban egyik káró eldobható). Ha kárót játszik kicsivel, **mi finesszelünk a 2-es lap fölé** és a 9 helyett a dámát tesszük be, ami nyer (mert a király bal felől jön).

**Tanulság:** Az endplay azt csinálja, hogy az ellenfél *kényszer-fineszt játszik magától*, így a finesz nem 50%-os, hanem 100%-os lesz.

## Squeeze – általános alapelvek

Squeeze játéknál egy ellenfél két (vagy több) színt egyszerre nem tud védeni, és valamelyiket „elfelejteni" kényszerül.

### Alapfeltételek (BLUE-CASH-szerű mnemonika)

1. **Count rectification (ütésszám-igazítás):** Az ütésszám pontosan 1-gyel kevesebb legyen, mint a kívánt cél. Ha 12 ütés kell, az ellenfélnek pontosan 1 ütése maradjon (az ún. „one trick short" pozíció). Gyakran szándékosan kiadunk egy korai ütést erre.
2. **Two threats (két fenyegetés):** Két különböző színben olyan kártyánk legyen, amely ütést érne, ha a megfelelő ellenfél kiengedi (pl. egy nem-magas „bezárt" lap, ami pontosan akkor üt, ha a védő eldobja a stopperét).
3. **Communication (átmenet):** A fenyegetésekhez vezető átmenet végig megmaradjon — különben a fenyegetés akkor sem üt, ha a védő eldobta a védő kártyáját.
4. **Squeeze card:** Az a lap, amelyet játszva az ellenfél kénytelen valamit eldobni. Általában a legolcsóbb hosszú szín utolsó lapja, ami már senkit sem érint, csak az ellenfelet, akit szorítunk.

> 💡 **Egyetlen kulcsmondat:** „**Ha az ellenfélnek 1 ütése maradhat, és én 2 fenyegetést tartok két különböző színben, akkor a squeeze card lejátszása után az ellenfélnek dönteni kell — és minden döntése rossz.**"

## Simple squeeze

**Egy ellenfél, két szín, egy fenyegetés mindkét színben.** A legalapvetőbb squeeze típus.

### Példa (positional squeeze – csak ha a védő a felvevő ELŐTT van)

**Cél:** Az utolsó ütés. Te 12 ütést akarsz, már 11 megvan.

```
              ♥ Q
              ♦ K              ← dummy (fenyegetések)

♥ Kx       
♦ Ax        ← a kritikus védő (West)

              ♣ A              ← squeeze card (felvevő)
              ♥ 4
              ♦ 2              ← cső-fenyegetések „bezárva"
```

A ♣A lejátszásánál nyugat választani kénytelen:

- Ha **♥K-t** dob, a dummy ♥Q üt (és az utolsó ütésen mi visszük: 12. ütés).
- Ha **♦A-t** dob, a dummy ♦K üt (12. ütés).
- Bármit dob, **squeezed!**

### Pozicionális vs. automatikus squeeze

- **Positional:** Csak akkor működik, ha a védő egy konkrét irányból ül (általában a fenyegetés-szín kéz ELŐTT). A fenti példa is positional.
- **Automatikus:** Akármelyik védőnél van a stopper, működik. Ehhez két oldalon kell fenyegetés (mindkét védőre alkalmazható).

## Vienna coup

A Vienna coup **ELŐKÉSZÍTŐ technika**: amikor a fenyegetés-szín fő ütése (általában ász) a felvevő kezében van, és „blokkolja" a saját fenyegetését, kihúzzuk az ászt SZÁNDÉKOSAN, hogy a partner kezében (dummy) maradó kis lap legyen az igazi fenyegetés.

### Klasszikus Vienna pozíció

```
                  ♥ Q         ← fenyegetés (dummy)

♥ K (védő)
              
                  ♥ A 4       ← felvevő – Az ász "blokkolja" a Q-t!
```

Anélkül, hogy lehúzzuk az ♥A-t, a ♥Q soha nem üthet (mert a védő ♥K-val felülütheti). **Megoldás:**

1. Mielőtt a squeeze card-ot játsszuk, **lehívjuk a ♥A-t** (Vienna coup).
2. Most a ♥Q a dummyban a tényleges fenyegetés (a védőnek ♥K-t kell tartania, hogy védje).
3. **Ezután a squeeze card** (más színből) lejátszása már működik: az ellenfél nem tudja a ♥K-t megtartani úgy, hogy a másik szín fenyegetését is védje.

> 💡 **Mnemonika:** „**Cash the ace, blow the threat, then squeeze.**" Az ász kihúzása **„felszabadítja"** a fenyegetést, mert a védőnek immár nincs „önmagát védő" módja arra a színre.

## Double squeeze

**Mindkét ellenfél squeeze-elve.** Van egy közös szín, amelyet csak az egyik ellenfél tud védeni, és két másik szín, amelyek külön-külön a másik ellenfelet érintik.

### Pozíció (vázlatosan)

```
                  ♠ x         ← West-fenyegetés
                  ♦ x         ← közös fenyegetés (mindkét ellenfél védi)
                  ♣ —

♠ K              ♥ K          
♦ Q              ♦ J          
♣ —              ♣ —          

                  ♥ x         ← East-fenyegetés
                  ♦ x         
                  ♣ A         ← squeeze card
```

- A ♣A-t játsszuk.
- **Nyugat** kénytelen választani: ha ♠K-t dob, dummy ♠ ütés; ha ♦Q-t dob, dummy ♦ ütés ÉS ezzel keletet is „kibírja". Tegyük fel ♠K-t dobott (a saját ♠ fenyegetést védte).
- **Kelet** közben látta a nyugati dobást. Nyugat már nem védi a ♦-t, így keletnek kell. Tehát keletnek ♦J-t kell tartania. → Eldobja a ♥K-t.
- Felvevő ♥ ütését lehívja.

Tipikus 13 ütésért: 12 már „be van zsebelve", a dummyben + felvevő kézben pontosan 1+1+1 lap az utolsó ütésre + fenyegetések.

## Criss-cross squeeze

**Egyazon ellenfél, két fenyegetés, mindkét fenyegetés A-x-szel a felvevőnél vagy dummyban (azaz „blokkolt").** Mindkét oldalon szükség van [Vienna coup](#vienna-coup)-szerű előkészítésre, de **átlósan**: a kezünkben lévő ász a dummy fenyegetését szabadítja fel, és fordítva.

```
                  ♥ Ax
                  ♦ x

♥ K? (vagy ♦K?)  ← Az egyik védő mindkét stoppert tartja
                  
                  ♥ x
                  ♦ Ax
                  ♣ A     ← squeeze card
```

A nehézség a kommunikáció: meg kell tartanunk az átmenetet *mindkét* oldalra ahhoz a kézhez, ahol épp a felszabadított fenyegetés van. Néha ez a squeeze card kezében lévő alacsony lapnyi átmenet.

> 💡 Általánosabb tanulság: a criss-cross gyakran „könnyebbnek tűnik", mert csak 1 védőre kell figyelni, de **a játék sorrendje kritikus**.

## Trump squeeze

**Adujáték végén az aduszín maga az egyik fenyegetés / lehívó eszköz.** Általában akkor működik, ha:

- A felvevő kéz vagy dummy aduja még el tud venni egy oldalszínű ütést (ruff fenyegetés).
- Az ellenfél vagy az adut őrzi (nem dobja), vagy az oldalszín fenyegetést – egyszerre nem mehet.

### Példa

A felvevő szerződése 6♠. Az utolsó 4 ütés állása:

```
                  ♠ —
                  ♥ Q3
                  ♦ —
                  ♣ x

♠ —                
♥ KJx          ♥ xx
♦ —             ♦ Qx
                  
                  ♠ J             ← utolsó adu
                  ♥ A
                  ♦ x
                  ♣ —
```

A felvevő lehívja a ♥A-t (♥K eldobható csak Westnél, mert ezzel megmaradna a ♥Q a dummyban; ha West a ♥K-t tartja, akkor a ♥J kell hogy menjen → akkor a ♥Q üt). De ha West a ♥K-t megtartja, és ♦Q-t dob, akkor:

- Felvevő ♥A → ♥3 → ♦x → utolsó ♠J: a ♥Q üt vagy a ♠J ruff-ot ad.
- Squeeze: a védő kétfelé húzva nem tud sem ♥K-t, sem ♦Q-t megtartani, **mert az adu még ruff-fenyegetést jelent.**

## Strip squeeze

> 🆕 Új technika, korábban nem volt a dokumentumban.

A strip squeeze (más néven **squeeze-without-the-count**) az endplay és a squeeze hibridje. Akkor használjuk, amikor a count *nincs igazítva* (nem 1 ütés híján vagyunk), és nem tudunk count-rectification-t csinálni (pl. az ellenfél már mindenét lehívta volna), de a védő egyik tartózkodó lapja olyan, hogy ha eldobjuk neki, akkor neki kell beadnia magát egy endplay-jel.

### Lényeg

A védő egyszerre kénytelen:

1. **Egy fenyegetést védeni** (hagyományos squeeze fenyegetés), VAGY
2. **Egy „menekülő" lapot megtartani**, ami kvázi egy throw-in kard — mert ha eldobja, akkor a felvevő tudja őt egy endplay-jel megadóztatni.

Ha eldob 1-et → simán üt a fenyegetés. Ha megtart 1-et → endplay-be hajtjuk.

### Példa

Szerződés: 6NT. Az utolsó 4 ütés:

```
                  ♠ AQ
                  ♥ —
                  ♦ —
                  ♣ x

♠ Kx           ♠ J?
♥ —             ♥ —
♦ —             ♦ —
♣ Kx           ♣ Jx

                  ♠ x
                  ♥ A
                  ♦ —
                  ♣ A
```

Mi 11 ütést szereztünk, és a 12. kell. A ♥A-t játsszuk **squeeze card**-ként. Most:

- **Nyugatnak** tartania kell mind ♠K-t (a ♠AQ-val nézve), mind ♣K-t (a kezünkben lévő ♣A miatt).
- Ha eldobja a ♣K-t → a kezében lévő ♣A üt, és a 13. ütésért ♠ ász vagy ♠Q (50%-os finesz nyugat felé). Tippeljük szerencsésen.
- Ha eldobja a ♠K-t → ♠A → ♠Q a végén üt, viszont nincs is finesz.
- **Strip squeeze trükk:** ha mind ♠K-t, mind ♣K-t megtartja, akkor most a ♣A-t lehívva endplay-be hajtjuk: nyugatnak ♣K-val be kell ütnie, és aztán ♠K-ba kell kárózni → ♠A üti! Vagyis **3 forgatókönyv mindegyike vesztes** a nyugatnak — ezért „strip" + „squeeze".

> 💡 A strip squeeze rendkívül elegáns, mert nem kell elkölteni az „1 trick short" pozíciót — viszont az ellenfél tartózkodó kártyáit pontosan kell ismernünk.

## Compound squeeze

**Több (általában 3) fenyegetés egyetlen szekvenciában, ahol az első squeeze a védőt egyik oldalon kényszeríti dobásra, ami felszabadít egy második squeeze-t** ugyanazon (vagy másik) védő ellen. Ritka, de tankönyvi „kombinált" trükk.

Praktikusan: az első squeeze card lejátszása után a védő szorult helyzetbe kerül, és a kötelező dobás felfedi a kéz pontos struktúráját. A felvevő azonnal kihasználja egy második squeeze-szel.

## Guard squeeze

**Egy védő egyszerre kénytelen védeni egy fenyegetést ÉS megtartani egy „őr" lapot** (general-purpose guard), ami a partnerét óvja egy finesztől. Mindkettő nem fér el a kezében — squeeze!

### Példa

A felvevőnek szüksége van egy ♥ K-impasszra, de csak akkor merné megjátszani, ha biztosan tudná, hogy a ♥K nyugatnál van. Egy másik színben (♣) viszont fenyegetést képes építeni nyugatra. Ha nyugat dobja a ♣ stopperét → ♣ ütésünk lesz. Ha tartja → nem mer ♥K-t tartani „őrként" — és ♠ vagy ♦ finesz révén bukik.

## Trump coup

**A felvevőnek elfogyott az aduja, de az ellenfélnél még van magas adu.** A trump coup célja: az utolsó ütések olyan állásban érjék az ellenfelet, hogy az adu-ütését „át kelljen lépnie" oldalszínű lehívásra (mert ha be is üt, a felvevő alól lép).

**Tipikus elemek:**

- **Adusor egyenlőtlenné tétele:** a felvevőnek pontosan annyi adut kell hagynia magán + dummyban, ahány az ellenfélnek.
- **Megfelelő mennyiségű ruff előtt:** szándékosan ruff-olunk az adu-rövidülés érdekében (azaz „fogyatjuk" magunkat le).
- **Pozícionálás:** az ellenfelet úgy érje az utolsó adu-vezetés, hogy a felvevő mögötte üljön (második kéz a végén).

### Klasszikus példa

Az ellenfélnél (jobboldali védő) ♠J9 marad, a felvevőnél ♠KQ. Ha simán ♠K-t vagy ♠Q-t játszunk, a védő ♠J-t alá teszi, és a ♠9 az utolsó adu — büntetlenül vihet ütést. Trump coup: a felvevő úgy alakítja a kezét, hogy az utolsó 2 ütésben *csak adu marad mindkét kézben*, és a védőnek elsőként KELL adut húzni → a ♠J alulról jön, és ♠K + ♠Q végigviszi.

## Coup en passant

**A felvevő egy oldalszín lehívásával kvázi „elsétál" az ellenfél magas aduja mellett**: az ellenfél vagy felüt aduval (akkor a felvevő aduja érvényesül később), vagy nem üt fel (akkor az oldalszín ütést kapjuk).

Klasszikusan a [trump coup](#trump-coup) egy enyhébb változata. „Passzban" = mintegy elhalad.

## Loser-on-loser play

**Egy oldalszín kiadó ütésére saját kiadónk eldobása** – látszólag ostobaság, valójában taktikai okokból:

- **Endplay előkészítése:** a „rossz" ellenfelet kiválasztjuk, ki üssön; a kezét megfosztjuk biztonságos exit-kártyától.
- **Adusplit elkerülése:** ha a partner aduvágna ránk, és ezt elkerülnénk, kiadóval „helyettesítve" elveszítjük az ütést, de az adusort megtartjuk.
- **Communication megőrzése:** az ellenfél által nyitott színben elsült ütésünket nem akarjuk üríteni, mert utánna nem tudnánk visszamenni a saját kezünkre.

### Példa loser-on-loser

Szerződés 4♠. Felvevő kezében ♣KQx, dummyban ♣Axx. A védő ♣A-val indul (rossz hír!), majd ♣2-vel folytat. A felvevő nyilvánvalóan elveszítette a ♣A-t. Helyette **dummyban beüt** ♣K-val, és a kezében nem tesz be egy harmadik treffet: helyette egy ♥-kiadót dob el!

Most a felvevő látja: később, ha kiad egy kőrt, az endplay-be hajthatja a védőt, mert ♣Q csak addig fenyegetés, amíg lapot tud rajta levenni — és az áthelyezett ♥ kiadó már nem ott van, ahol baj lenne belőle.

## Dummy reversal

Az alap-stratégia szerint a HOSSZABB adu-kéz húzza az adut. A **dummy reversal** ellentétes: a hosszú adu-kéznél RUFF-olunk, és a rövid adu-kézzel lapátoljuk az aduslagot:

- Akkor érdemes, ha a hosszú kézben kevés a melléküt, és a rövid kéznél hosszú szín lehívható.
- A ruff-ok megnövelik az ütésszámot 1-2-vel a természetes „adu-húz, oldal lehív" képest.
- **Tipikus felállás:** 5-3 vagy 6-3-as adu, dummyban a hosszabb, és a felvevőnél hosszú oldalszín.

### Példa

```
              Dummy: ♠ AQJxx ♥ Axx ♦ xx ♣ xxx     ← hosszú adu
              Felvevő: ♠ Kx ♥ Kxx ♦ AKQJxx ♣ Ax   ← rövid adu, hosszú káró
```

Szerződés 6♠. Klasszikus: ♠AKQJxx után 5 pikk + ♦AKQJ + ♥A + 2 belevágás = problematikus.

**Dummy reversal:** A felvevő úgy döntsön, hogy a *kezében* a rövid pikkkel adutartást ad, és **a dummy hosszú pikkjeivel ruff-olja** a kezében lévő 3 kőrt + 1 treffet. Így a dummy aduja „kéznél" elfogy, viszont a kezében marad az aduszín – és a 6 lapos káró lefuthat 6 ütésért. Eredmény: 6+5+1 = 12 ütés. ✅

## Avoidance play

Az **„okos"** módja, hogy MINDIG ugyanazt a (veszélyes) ellenfelet tartsuk ütésen kívül. Tipikusan 3NT vagy NT-szlemnél, ahol az egyik ellenfél hosszú szín-fenyegetése aktív:

- Fineszelési irányokat választunk meg úgy, hogy a veszélyes ellenfél ne kerüljön be.
- Néha: szándékosan kiengedünk egy ütést a NEM veszélyes ellenfélnek, hogy a veszélyeshez ne kerüljön rá.
- **Példa:** ♣ AQx vs xx hosszú szín, a balszélen lévő ellenfél a veszélyes – fineszelést NEM finiseljük, hanem ász-kis felé játszunk és a kis lapot bedobjuk.

### Tipikus avoidance helyzet

A felvevő 3NT-ben, Nyugat indult ♥5-vel (negyedikkel), a felvevőnek ♥Axx van. A ♥A-t **nem** vesszük be azonnal (hold-up); kelet ♥J-vel követi. Tegyük fel, kétszer hold-up-olunk, és a 3. kőr ütésénél már ♥A kötelező.

Most a felvevő tudja: **nyugat a veszélyes**, mert még 2 magas kőrje van. Bármilyen finesz, ami nyugatot beengedi, halálos. Ezért:

- Ha ♦ KQJxx van a kezében és ♦ Axx a dummyban, a ♦ A-t (dummy) lehívja először (avoidance), és csak utána játszik kicsit. Ha a ♦ K nyugatnál van, ő üt — viszont a kőrt már nem tudja lehívni, mert nincs belépő.

## Safety play

**A maximális ütésszám helyett a SZERZŐDÉS biztosítása.** Lemondunk az „extra" ütésről egy rosszabb állásban a játékvitel garantálásáért:

### Példa: AKxxx vs xxx (4 ütésért)

Ha 4 ütésből biztosan kell, a **kis lap mindkét kézből** (és kis-felé játszás) **5 helyett 4-et garantál** (akkor is, ha JTxx van velünk szemben).

- A „mohó" játék: ♠A, majd ♠K, majd folytatás. Ha a szín 4-1 áll meg, csak 4 ütést kapunk; 3-2 esetén 5-öt.
- Safety: ♠ Az első kör kis-kis (mindkét kézből), a másik beüt ♠Q-val vagy ♠J-vel. Ezután ♠A és ♠K kihúzza a maradékot, és garantáltan 4 ütésünk lesz a szín bármilyen 4-1 vagy 3-2 állásánál.

### Példa: AQTx vs xxx (3 ütésért)

Ha 3 ütés kell, a kétszeres fineszt elkerülve **az ásszal indulunk, majd kicsi-felé játszunk a Q felé**. Ha a király bal felől jön, az nem kell — már megvan a 3 (A + Q + T = 3 valószínűleg). Sokkal biztosabb, mint a tisztaza kétszeres fineszre menni.

> 💡 **Általános elv:** Minden lehetséges színeloszlást vegyünk számba, és válasszuk azt a sorrendet, ami a LEGROSSZABB esetben is teljesít.

## Hold-up play (várakozás)

NT-játékban a stopperünket szándékosan visszatartjuk, hogy az ellenfél kommunikációját megszakítsuk.

**Klasszikus „Rule of 7":** Ha az ellenfeleknek (saját + dummy színemen kívül) X lap van egy színből, akkor (X − 7) körig húzzuk a hold-up-ot. Pl. 5 lapos kőrindítás esetén (5-2 nálunk + 11 az ellenfélnél) → 4 körig húzunk, vagy a természetes 2-szeres hold-up.

- Ha az ellenfél 5 lapos színt vezet, és nálunk Axx van: kétszer engedünk át (tartjuk az ász-t), majd a 3. ütésen vesszük be – a partner addigra már nem tud belépőt mutatni.
- **Veszély:** ha a fineszelési ellenfél a hold-up alatt belépőt nyer, akkor mégis átmehet → az [avoidance play](#avoidance-play)-jel kombinálva érdemes.

## Communication play (átmenetek)

A felvevő egyik fő erőforrása a két kéz közötti **„közlekedés"**. Tipikus témák:

- **Belépők megőrzése a hosszú szín lehívásához:** gyakran feláldozunk kis ütést a végén úgy, hogy a magas lapot eldobjuk a sajátunkból.
- **Unblocking:** szándékosan kidobunk egy magas lapot a rövid kézből, hogy a hosszú kéz lapja át tudjon menni.

### Klasszikus unblocking példa

```
Dummy: ♥ AKxxx
Felvevő: ♥ Q2
```

Ha a felvevő ♥Q-t és ♥2-t hagyja a végére, akkor a dummy 4. és 5. kőre nem érhető el (mert a felvevő kőr-ütései elfogytak). **Megoldás:** Mihelyt a dummyban ♥A-t és ♥K-t húzol, a kezedből **♥Q-t alaeresztsd** az ♥A vagy ♥K alá! Ezzel a 4. kőr nyer (♥xx), és a kommunikáció megmarad.

### Entries számolása indulás után

Mielőtt fineszelünk, mindig gondoljuk át: **hány belépőm van még a vágó-irányba?** Egy klasszikus 3NT-bukás kiváltó oka, hogy a felvevő 1 belépővel kevesebbet számol egy AQxx-finesz kétszeri ismétlésére. Pénz az életbiztosítás: 1-2 percet rászánni az átmenetek számolására *minden szerződés elején*.

## Counting – a felvevő alapdiszciplínája

Minden lejátszási taktika alapja, hogy folyamatosan számoljuk:

- **Lapok hosszát szín szerint** mindkét ellenfélnél (a kontrákból és kihagyásokból kikövetkeztetve).
- **HCP-t** a licit + a kihagyások / kontrák alapján.
- **Az ellenfelek jelzéseit** ([attitude](#attitude-upside-down), [count](#count-upside-down), [suit-preference](#suit-preference)) egész kontextusban.

Az endplay-ek és squeeze-ek 90%-ban azon múlnak, hogy a felvevő pontosan ismeri a megmaradt kártyák eloszlását az utolsó 3-4 ütés előtt.

### Mnemonika a count-hoz: „**LFP-O**"

- **L** – Licit alapján (közbeszólás → 5+ lap; passz a partnerre → max 5 HCP; stb.).
- **F** – Felüt és nem üt (ha egy ellenfél nem ad ütést egy számára nyerő lappal, az inferálható információ).
- **P** – Pakli zárt: minden szín 13 lap, az látható + asztal + általam játszott + szignálok pontosan kiadják.
- **O** – Olvasott szignálok (count + attitude, főleg az indító ütésnél).

---

<a id="gyorskereső-játék-közben"></a>
# 📋 Gyorskereső (játék közben)

> Az alábbi táblázat azt segíti, hogy menet közben gyorsan eldöntsd: **mit jelent a licit / mit kell mondanom?** Mindegyik sor linkkel mutat a részletes szabályra.

## Indulóként – Első licit

| Lapom | Licit | Hivatkozás |
| :---- | :---- | :---- |
| 15–17 HCP, balanced (4-3-3-3 / 4-4-3-2 / 5-3-3-2) | **1NT** | [Induló licitek](#induló-licitek--részletes-táblázat) |
| 20–21 HCP, balanced | **2NT (Stop)** | [Induló licitek](#induló-licitek--részletes-táblázat) |
| 24–26 HCP, balanced | **3NT (Stop)** | [Induló licitek](#induló-licitek--részletes-táblázat) |
| 22–23 HCP, balanced | **2♣** → válasz → **2NT** | [2♣ + rebid](#egyéb-megfontolások-az-erős-2-treff-után) |
| 22+ HCP balanced, *vagy* 19+ HCP + 9+ playing trick (eloszlásos) | **2♣ (Stop!)** | [Erős 2 treff](#erős-2-treff-indulás) |
| 12+ HCP + 5-ös nemes | **1♥** vagy **1♠** | [Általános irányelvek](#általános-irányelvek) |
| 12+ HCP, nincs 5-ös nemes, 4+ káró | **1♦** | [Általános irányelvek](#általános-irányelvek) |
| 12+ HCP, nincs 5-ös nemes, 3-3 nemnemes | **1♣** (convenient minor) | [Általános irányelvek](#általános-irányelvek) |
| Rule of 20 igazolja (≥ 20), 10–11 HCP, hosszú szín | **1 szín** (légy bátor!) | [Rule of 20](#the-rule-of-20) |
| 6–10 HCP (kedvezőtlen) / 5–11 (kedvező), 6-os szín, nincs „2 bare ace" | **Stop 2♦/♥/♠** | [Gyenge 2-es](#induló-licitek--részletes-táblázat) |
| 6–11 HCP, 7-os szín, 2+ honor | **Stop 3♣/♦/♥/♠** | [Gyenge 3-as](#induló-licitek--részletes-táblázat) |
| Nincs Rule of 20, nincs hosszú szín | **PASSZ** | — |

## Segítőként – Partner 1-szintű színes nyitására (közbeszólás nélkül)

| Lapom partner 1♥ / 1♠ nyitására | Licit | Hivatkozás |
| :---- | :---- | :---- |
| 6–9 HCP, 3+ adu (nem 4!) | **2 ugyanaz a szín** | [A) Első válasz](#áttekintő-táblázat) |
| 6–9 HCP, **4 lapos** fit | **3♣** (Bergen mass) | [Bergen Raises](#bergen-raises) |
| 10–12 HCP, **4 lapos** fit | **3♦** (Bergen mass) | [Bergen Raises](#bergen-raises) |
| 0–5 HCP, 4 lapos adu (preempt) | **3 ugyanaz** | [Bergen Raises](#bergen-raises) |
| 13+ HCP, 4+ lapos fit, slem-érdeklődés | **2NT** (Jacoby 2NT) | [Jacoby 2NT](#jacoby-2nt-segítőként-csak-nemes-nyitásra) |
| 12+ HCP, 4+ pikk, partner kőrt nyitott | **1♠** (új szín, GF lehet) | [A) Első válasz](#áttekintő-táblázat) |
| 13+ HCP, splinter értékelhető (egyke + 4 fit) | **Splinter** (dupla ugrás új színben) | [Splinter](#splinter-bids) |
| 6–12 HCP, nincs fit, nincs új színem | **1NT** (semi-forcing) | [Semi-forcing 1NT](#semi-forcing-1nt-1m--1nt) |
| Új szín, 2-es szinten, 13+ HCP | **2♣ / 2♦ / 2♥** (2/1 GF) | [2/1 Game Forcing](#21-game-forcing-és-reverse-bidding) |
| **Passzolt segítőként**, 10–11 HCP, 3+ adu | **2♣** (Reverse Drury) | [Drury](#drury-konvenció-passzolt-segítő) |

## Segítőként – Partner 1♣ / 1♦ nyitására (közbeszólás nélkül)

| Lapom | Licit | Hivatkozás |
| :---- | :---- | :---- |
| 6+ HCP + 4+ nemes | **1♥ / 1♠** | [Inverted minor jegyzet](#inverted-minor-csak-nem-nemes-nyitásra) |
| 10+ HCP, 4+ fit, nincs nemes | **2 ugyanaz** (Inverted minor, erős) | [Inverted minor](#inverted-minor-csak-nem-nemes-nyitásra) |
| 0–6 HCP, 5+ fit, nincs nemes | **3 ugyanaz** (Inverted minor, gyenge) | [Inverted minor](#inverted-minor-csak-nem-nemes-nyitásra) |
| 17+ HCP, 4+ új szín | **Jump-shift** | [A) Első válasz](#áttekintő-táblázat) |

## Segítőként – Partner 1NT nyitására (közbeszólás nélkül)

| Lapom | Licit | Hivatkozás |
| :---- | :---- | :---- |
| 0–7, nincs 5-ös nemes, nincs 6-os alsó | **PASSZ** | [A) Segítő válaszai](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül) |
| 8+ HCP, pontosan 4-4 nemes | **2♣** (Stayman) | [Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) |
| 0–7 HCP, 4-4-4-1 vagy hasonló rövid treffel | **2♣** (Garbage Stayman) | [Garbage Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) |
| 0–7 HCP, 4-4 nemes + rövid treff, partner 2♥/2♠-t mondott | **Crawling**: új nemes a 2-es szinten | [Crawling Stayman](#crawling-creeping-stayman-konvenció) |
| 10+ HCP, 5-4 nemes | **2♣** → ha 2♦, akkor **3♥/♠** (Smolen) | [Smolen](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) |
| 5+ kőr | **2♦** (Jacoby transfer) | [Jacoby transzfer](#jacoby-transzfer-i-és-ii-1nt--2-kőrre-1nt--2-pikkre) |
| 5+ pikk | **2♥** (Jacoby transfer) | [Jacoby transzfer](#jacoby-transzfer-i-és-ii-1nt--2-kőrre-1nt--2-pikkre) |
| 6+ alsó szín, gyenge | **2♠** (minor transfer) | [A) Segítő válaszai](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül) |
| 8–9 HCP, balanced | **2NT** | [A) Segítő válaszai](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül) |
| 10+ HCP, 3-as nemes garantálva | **3♣** (Puppet Stayman) | [Puppet Stayman](#puppet-stayman-konvenció-1nt--3-vagy-2nt--3) |
| 16–17 HCP, balanced, slem-meghívás | **4NT** (kvantitatív, NEM ászkérdés!) | [A) Segítő válaszai](#a-segítő-válaszai-1nt-indulásra-közbeszólás-nélkül) |
| Ászkérdés (slem-kontextus) | **4♣** (Gerber!) | [Gerber](#gerber-szanra-adott-ász--és-királykérdés) |

## Segítőként – Partner 1♥/1♠ nyitására, ellenfél X-elt (takeout double)

| Lapom | Licit | Hivatkozás |
| :---- | :---- | :---- |
| 0–5 HCP, nincs jó licit | **PASSZ** | — |
| 6–9 HCP, 3+ adu | **2 ugyanaz a szín** (konstruktív) | [Ellenfél kontrázott — közbeszólás](#ellenfél-kontrázott--ez-is-közbeszólás) |
| **10+ HCP, 4+ adu** | **2NT (Jordan)** | [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) |
| 0–6 HCP, 4+ adu, preempt | **3 ugyanaz a szín** | [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) |
| 0–7 HCP, 5+ adu, shape-es | **4 ugyanaz a szín** | [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) |
| 10+ HCP, **nincs** 4+ adu | **XX (rekontra)** | [Rekontra](#rekontra-erős) |
| Splinter értékelhető (4+ adu + egyke) | **Dupla ugrás új színben** | [Splinter](#splinter-bids) |
| 7–10 HCP, balanced, nincs fit | **1NT** | [Jordan 2NT](#jordan-2nt-4-fit--10-hcp-take-out-double-után) |

## Ellenfél közbeszólt – mit jelent a kontrám?

| Szekvencia | Kontra jelentése | Hivatkozás |
| :---- | :---- | :---- |
| Mi nyitottunk → ellenfél közbeszólt → partner kontra | **Negatív double**, 6+ HCP, pontosan 4 lapos nem-közbeszólt nemes | [Negatív kontra](#negatív-kontra-a-standard-sayc-b-konvenció) |
| Mi nyitottunk nemest → partner új színt válaszolt → ellenfél közbeszólt → mi kontra | **Support Double**, pontosan 3 lapos partner-fit | [Support Double](#support-double) |
| Ellenfél nyitott → kontra (közvetlen) | **Take-out double**, 12–15 HCP | [Take-out Double](#take-out-double) |
| Ellenfél nyitott → passz → passz → kontra | **Reopening double**, 8–14 HCP, rövidség | [Reopening Double](#újranyitó-kontra-reopening-double) |
| Mi nyitottunk → ellenfél kontra → mi rekontra | **Erős rekontra**, 10+ HCP, nincs fit | [Rekontra](#rekontra-erős) |
| Ellenfél nyitott → kontra → partner új szín → mi rebid → kontra második körben | **Power double**, 16+ HCP | [Power Double](#power-double-erős-kontra-16-hcp) |
| 1NT-re ellenfél közbeszólt (2-es szinten) → mi kontra | **Stayman** | [B) Válaszok 1NT-re](#az-ellenfél-kettes-szinten-szólt-közbe--kontra) |
| Ellenfél ászkérdésünkbe közbeszólt → kontra | **Páros** ász (DEPO) | [DEPO](#ha-közbeszóltak-az-ászkérdésre--depo) |

## Slamkereső szekvenciák – gyorsmenü

| Helyzet | Licit | Hivatkozás |
| :---- | :---- | :---- |
| Adu megegyezve (♠), kulcslapokat kérdezek | **4NT** (Kickback) | [Kickback 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430) |
| Adu megegyezve (♥), kulcslapokat kérdezek | **4♠** (Kickback) | [Kickback 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430) |
| Adu megegyezve (♦), kulcslapokat kérdezek | **4♥** (Kickback) | [Kickback 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430) |
| Adu megegyezve (♣), kulcslapokat kérdezek | **4♦** (Kickback) | [Kickback 1430](#kickback-helyett-4nt-kickback-roman-key-card-blackwood-rkc-ászkérdés--1430) |
| NT nyitás után, slem-kontextus, ász kell | **4♣** (Gerber) | [Gerber](#gerber-szanra-adott-ász--és-királykérdés) |
| Adu OK, kulcslapok OK, király is kell | **5NT** (Specific King Ask) | [5NT](#5nt-specific-king-ask-királykérdés-kickback-után) |
| Adu OK, void van mellékszínben | **5 új szín** (Exclusion) | [Exclusion](#exclusion-blackwood) |
| Adu OK, kontroll-mutogatás | **4♣ / 4♦ / 4♥** (Cuebid) | [Cuebid](#cuebid--első--és-másodkörös-kontrollok) |

## Védekezés – jelzések

| Jelzés helyzete | Konvenció | Jelentés (upside-down) |
| :---- | :---- | :---- |
| Partner indított | **Attitude** | Kicsi = bátorítás, nagy = elbátortalanítás |
| 2. menet, követni kell | **Count** | Kicsi = páros, nagy = páratlan |
| Színváltást kell sugallnom | **Suit-preference** | Kicsi = olcsóbb szín, nagy = drágább szín |

---

## Példa licitsorozatok minden főbb konvencióhoz

> 💡 Minden példában a Nyitó balra, a Segítő jobbra van — a sorrend a nemzetközi licitlap szerinti olvasási irány.

### Stayman + 4-3 nemes felderítés

| Nyitó (15–17 NT) | Segítő (8 HCP, 4-3-3-3, 4 kőr) |
| :---- | :---- |
| 1NT | 2♣ (Stayman) |
| 2♥ („van 4 kőröm") | 4♥ (megvan a fit, 8+8+8=24) |

### Jacoby transfer + szuper-elfogadás

| Nyitó (17 NT, 4 pikk) | Segítő (10, 5 pikk) |
| :---- | :---- |
| 1NT | 2♥ (Jacoby transfer pikkre) |
| **3♠** (szuper-elfogadás: 4 pikk + 16–17 HCP) | 4♠ (van fit + jó pont, megyünk gémre) |

### Negative double + folytatás

| Nyitó (1♦) | Ellenfél (1♥) | Segítő (4 pikk, 8 HCP) | Ellenfél (passz) |
| :---- | :---- | :---- | :---- |
| 1♦ | 1♥ | **X** (negative: 4 pikk + 6+ HCP) | Passz |
| 1♠ (4 pikkem van) | passz | 3♠ (10–12 limit) | passz |
| 4♠ (van pont rá) | | | |

### Splinter + Kickback slem

| Nyitó (1♥) | Segítő (♥ KQxx, ♠ Axx, ♦ Axxx, ♣ x) |
| :---- | :---- |
| 1♥ | **4♣** (Splinter: 4+ kőr, 12+ HCP, ♣ egyke vagy void) |
| 4♠ (cue, ♠ kontroll) | 4NT (Kickback: ♥ az adu, hányad kulcslapod van?) |
| 5♥ (2 lépcső = 2 kulcslap, dáma nélkül) | 6♥ (van min. 4+2=6 kulcslap az 5-ből) |

### Lebensohl 1NT ellen + különböző folytatások

**Gyenge kéz (5 HCP, ♠ JTxxx):**

| Nyitó | Ellenfél | Segítő | |
| :---- | :---- | :---- | :---- |
| 1NT | 2♥ (overcall) | **2NT** (Lebensohl) | |
| 3♣ (kötelezően) | passz | 3♠ (sign-off, lezáró: gyenge!) | |

**Game force (12 HCP, ♠ AQxxx, stopper nélkül kőrben):**

| Nyitó | Ellenfél | Segítő | |
| :---- | :---- | :---- | :---- |
| 1NT | 2♥ | **3♥** (cue bid: GF, „van-e kőr stoppered?") | |
| 3♠ („van fit") | | 4♠ (game!) | |

**Game force (12 HCP, ♠ KQJxx, kőr stopper meg van):**

| Nyitó | Ellenfél | Segítő | |
| :---- | :---- | :---- | :---- |
| 1NT | 2♥ | **3♠** (közvetlen, nem Lebensohl: 5+ pikk, GF) | |
| 4♠ (fit + pontok) | | | |

### 2/1 Game Forcing + lassú szerkezet-feltárás

| Nyitó (♠ AKxxx, ♥ Kx, ♦ AQx, ♣ xxx) | Segítő (♠ xx, ♥ Axxx, ♦ Kxx, ♣ AKxx) |
| :---- | :---- |
| 1♠ | 2♣ (2/1 GF — már gémig megyünk) |
| 2♦ (új szín, kényelmesen) | 2♥ (4 lapos kőr) |
| 2NT (balanced rebid, 12–14) | 3NT (lezáró, megvan a 3NT-pont) |

### Bergen mass-emelés példa

| Nyitó (♠ Kxxx, ♥ AQxxx, ♦ Ax, ♣ Kx) | Segítő (♠ xx, ♥ Kxxx, ♦ KQxx, ♣ Axx) |
| :---- | :---- |
| 1♥ | **3♦** (Bergen: 4 lap kőr, 10–12 HCP) |
| 4♥ (megvan a 9 adu + pontok) | passz |

---

## Gyakori licitálási hibák – anti-pattern szekció

> ⚠️ Az alábbi „gyakori csapdákat" érdemes ismerni és aktívan kerülni.

### 1. Stayman 4 lapos major trumf nélkül

**Hiba:** 1NT → 2♣ ÉS nincs 4 lapos kőr/pikk a segítőnél.

A Stayman **kizárólag** akkor jó, ha a segítőnek van legalább egy 4-es nemese, vagy [Garbage Stayman](#stayman-smolen-és-garbage-stayman-konvenciók-1nt--2) helyzet áll fenn (gyenge kéz, rövid treff). Nem szabad „csak úgy, kíváncsiságból" Staymant licitálni.

### 2. Túl erős nemes-emelés gyenge kerettel

**Hiba:** 1♥ → 3♥, amikor a segítőnek 11 HCP-je és 3 lapos kőre van.

A 3♥ a Bergen rendszerben **preempt** (0–5 HCP, 4 lapos adu), nem invitáló. Helyette használj 2NT-t (Jacoby) vagy [Bergen 3♦](#bergen-raises)-t (4 lapos fit invitáló).

### 3. Fourth-suit forcing helyett természetes 4. szín

**Hiba:** 1♣ – 1♥ – 1♠ – **2♦** azzal a szándékkal, hogy *valódi* káró-színt mutass.

Ez **forcing**! Ha valódi káród van és sign-off-ot akarsz, először Stayman-szerű licitálás, vagy NT-re emelés érdemes. A 4. szín = „mondj még valamit, nem értek egyet a NT-vel".

### 4. Splinter ász-szingli/színhiány esetén

**Hiba:** 1♥ → 4♦, amikor a segítőnél ♦A egyedül van (és 4 kőre + 11 HCP-je).

A splinter „extra rövid színt" jelez (a 0–1 hossz „bónusz", mert nyitónak nem kell káró-üt elvesztenie). Ha az egyetlen káró épp az ász, akkor **nem nyertünk semmit** — ezt a felvevő nem tudja kihasználni (az ász akkor is ütött volna). Helyette: használj [Jacoby 2NT](#jacoby-2nt-segítőként-csak-nemes-nyitásra)-t.

### 5. 1NT-re 4NT-vel ászkérdést indítani

**Hiba:** 1NT → 4NT → Te elkezded számolni az ászokat.

A 4NT itt **kvantitatív** (16–17 HCP)! Ászkérdéshez **Gerber (4♣)**! Lásd: [Gerber](#gerber-szanra-adott-ász--és-királykérdés).

### 6. Gyenge 2-es Rule of 20-as kézzel

**Hiba:** 11 HCP + 6 ♠ + 3 ♣ → 11+6+3=20 → indítasz **2♠**-t.

**Helyette:** **1♠**! A Rule of 20-as kézzel az 1-szintű nyitás magasabb értékű — több licit-rugalmasság, magasabb pontosság, esetleg gém. A gyenge 2-es csak **gyenge** kézhez való.

### 7. Reverse hiányában elveszett 17 HCP

**Hiba:** 17 HCP + 5 treff + 4 káró → 1♣ → 1♠ → **2♣** (helyett 2♦ reverse).

A 2♣ rebid 12–16 HCP-t mutat — a partner most már soha nem fog tudni a 17-edik pontról. Ha 17+ van, **kötelező** reverse-elni (2♦) vagy 2NT ugorni (18–19 balanced).

---

## TODO – kidolgozandó és olvasnivalók

Az alábbi témák további elmélyítése javasolt; a hivatkozott források mindegyikét érdemes legalább egyszer átfutni.

### Alapok és értékelés

- Hand evaluation (length points, evaluation alapok): [en.wikipedia.org/wiki/Hand_evaluation](https://en.wikipedia.org/wiki/Hand_evaluation)
- Zar Petkov rendszere (Zar Points eredeti cikkek): keresett Bridge Bulletin archívum

### Lebensohl és kapcsolódó konvenciók

- Weak twos and Lebensohl: [sydneybridgecentre.com/wp/weak-twos-and-lebensohl/](https://sydneybridgecentre.com/wp/weak-twos-and-lebensohl/)
- Lebensohl over Weak Two: [bridgebum.com/lebensohl_over_weak_two.php](https://www.bridgebum.com/lebensohl_over_weak_two.php)
- Lebensohl after 1NT: [bridgebum.com/lebensohl_after_1nt.php](https://www.bridgebum.com/lebensohl_after_1nt.php)

### Felvevő technikák (declarer play)

- Trump coup és coup család (kiváló kiindulás): [mapiano.com/coup.htm](https://www.mapiano.com/coup.htm)
- Kelsey: *Squeeze Play in Bridge*
- Kelsey & Ottlik: *Adventures in Card Play* – haladó squeeze és coup
- Reese: *The Expert Game* – inferencia és counting

### További olvasnivalók

- WNT konvenciók: [bridgewinners.com/article/view/5431-convention-after-wnt/](https://bridgewinners.com/article/view/5431-convention-after-wnt/)
- Andrew Robson – Tips for Intermediates: [andrewrobson.co.uk/article/tips_for_intermediates/2783](https://www.andrewrobson.co.uk/article/tips_for_intermediates/2783)

### Cue bidek és slem-keresés

- Splinters (részletesen): [bridgebum.com/splinters.php](https://www.bridgebum.com/splinters.php)
- Slam-seeking conventions: [en.wikipedia.org/wiki/Slam-seeking_conventions](https://en.wikipedia.org/wiki/Slam-seeking_conventions)

### BBO referencia (AdvGIB 2/1)

- GIB system notes: [bridgebase.com/doc/gib_system_notes.php](https://www.bridgebase.com/doc/gib_system_notes.php)

### Még kidolgozandó témák a következő iterációhoz

- Forcing 1NT (mint a Semi-forcing alternatívája) — döntés a csapatban
- Minorwood (a Kickback alternatívája alsóknál) — döntés a csapatban
- Részletes „2♣ → 2♦ → ?" nyitói viszontválasz táblázat (most csak placeholder)
- Részletes „2♣ → 2♥ → ?" dupla negatív utáni folytatás (most csak placeholder)
- További squeeze családok: backwash squeeze, ekvivalens-stripping, suicide squeeze
- Defenzív coup-ok: Merrimac coup, Deschapelles coup, Crocodile coup
- Kvantitatív 4NT további szekvenciák (slem-tapogatózás után)
