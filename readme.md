# Vefforritun 1, 2025, hópverkefni 2

- [Fyrirlestur 10.3: Hópverkefni 2](https://youtu.be/zlwHg9kDPZs)

## Verkefnalýsing

Verkefnið felst í að útbúa vef sem leyfir að búa til/velja spurningar og birta þær í barsvar (pubquiz) formi.

Verkefninu er skipt upp í verkefni sem verður að útfæra og verkefni þar sem hægt er að velja mismunandi virkni til að útfæra. Útfrá stærð hóps þarf að útfæra ákveðið mörg af þessum verkefnum. Ekki er gefið að hvert af þessum verkefnum séu jafn flókin eða tímafrek.

Vefur skal vera prófaður og virka í nýjustu útgáfum af Firefox og Chrome.

### Gögn

Nota skal gögn frá [is-trivia-questions](https://github.com/sveinn-steinarsson/is-trivia-questions), búa til ykkar eigin eða finna annarsstaðar.

### Forsíða og heildar útlit

Útbúa skal einfalt útlit fyrir forsíðu (`index.html`) sem veitir aðgang að þeim aðgerðum sem ákveðið er að útfæra, í minnsta lagi að birta spurningar. Einnig skal vefur hafa:

- Haus með titli síðu.
- Valmynd með hlekkjum á forsíðu og þá virkni sem er útfærð (t.d. `Forsíða`, `Búa til spurningar`, `Birta spurningar`, o.s.frv.).
- Fótur með einhverjum upplýsingum um vefinn, t.d. hver bjó til.

Þetta útlit fylgir sér síðan í gegnum aðrar síður. Athugið að útlit er ekki aðalatriði í þessu verkefni og skal vera einfalt.

Útlit skal vera skalanlegt frá `450px` upp í að minnsta kost `1600px` breidd.

Allt efni skal útbúið í JavaScript við keyrslu.

### Síður fyrir hvert efni

Fyrir hvert efni skal hafa síðu þannig að ef notandi refreshar síðu skal hún birt aftur.

Allt það sama gildir um þessar síður og um forsíðu varðandi útlit og skalanleika.

Hægt er að útfæra sem nokkrar HTML síður eða sem eina og nota JavaScript til að breyta innihaldi síðu og vísa í hvað er sýnt með query string eða hash í slóð.

## Virkni

### Grunvirkni

Í grunninn skal útfæra virkni sem birtir spurningar, eina í einu ásamt möguleikum til að fara í næstu spurningu og til baka í fyrri spurningu. Virkni getur verið þannig að frá forsíðu er hægt að fara í „Spurningar“. Þar er takki eða álíka sem byrjar að birta spurningar. Þegar spurning er birt skal hafa takka til að fara í næstu spurningu og til baka í fyrri spurningu ef við á (á ekki við að fara til baka í fyrstu spurningu eða áfram í síðustu spurningu).

Spurningar skulu að minnsta kosti:

- Innihalda 10 spurningar.
- Spurning skal að minnsta kosti hafa spurningu og svar. Í grunnvirkni er ekki krafa að birta svar.

Ekki er skilgreint _hvernig_ spurning er nákvæmlega birt eða _hvar_ spurningar eru geymdar en það eru önnur virkni sem hægt er að útfæra í þessu verkefni sem fjallar um það.

### Önnur virkni

Eftirfarandi er listi af annari virkni sem hægt er að útfæra. Fjöldi verkefna sem þarf að útfæra fer eftir stærð hóps.

#### Flóknari birting spurninga

Nota [Fullscreen API](https://developer.mozilla.org/en-US/docs/Web/API/Fullscreen_API) til að birta spurningar á skjá ásamt því að hafa lykilaborðsstjórn á því að fara í næstu spurningu og fyrri spurningu. T.d. að örvar til hægri og vinstri geri það. Að ýta á `F` fari í og úr fullscreen. `Space` gæti farið áfram í næstu spurningu.

#### Vista stöðu í localStorage

Nota [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) til að vista hvaða spurning er sýnd og hvar notandi er staddur í spurningum. Þegar notandi kemur aftur á síðuna skal birta sömu spurningu og síðast var sýnd.

#### Búa til spurningar og vista í localStorage

Þetta verkefni telst til tveggja verkefna vegna umfangs.

Búa til form sem leyfir notanda að búa til spurningu með spurningu og svari. Þegar formi er vistað skal vista spurningu í localStorage ásamt öðrum spurningum. Þegar spurningar eru birtar skal birta þessar spurningar ásamt þeim sem fyrir eru.

#### Nánari gögn fyrir spurningu

Bæta við fleiri gögnum fyrir spurningu, t.d. mynd, vídeó (embed af YouTube), bakgrunnslitur, flokkur, erfiðleikastig o.s.frv. Þegar spurning er birt skal birta þessi gögn líka eins og við á.

#### Miklu fleiri spurningar

Vinna fleiri spurningar úr spurningalista, a.m.k. 100 spurningar. Hvernig þið gerið það er upp á ykkur komið en það er leyfilegt að forrita það sem þarf til að ná þessu markmiði.

#### Búa til spurningalista

Þetta verkefni telst til tveggja verkefna vegna umfangs.

Búa til virkni þar sem búinn er til spurningalisti þar sem valdar eru spurningar úr þeim sem til eru. Upp á ykkur komið hvernig valið fer fram en það gæti tengst annari virkni, t.d. að velja flokk, velja spurningu og spurningu. Birta allar spurningar og leyfa að fjarlægja spurningar.

Að lokum skal vera hægt að gefa listanum heiti og vista í localStorage og síðan birta spurningar úr þessum lista þegar spurningar eru birtar.

#### Keppnisviðmót

Þetta verkefni telst til tveggja verkefna vegna umfangs.

Geta búið til keppnisviðmót þar sem búin eru til lið með nöfnum. Síðan er keyrt í gegnum spurningar og lið svara á einhvern hátt (gerum ráð fyrir að það sé bara á blaði). Í lokinn eru svör birt fyrir hverja spurningu og á einhvern hátt eru stig talin (aftur, gerum ráð fyrir að það sé bara gert á blaði). Síðan eru stig sett inn fyrir hvert lið og þeim raðað í stigatöflu þannig að sigurveinn sé efstur.

#### Önnur virkni

Annað sem þið getið útfært og skilgreint sjálf. Hægt er að ræða við kennara um hugmyndir, t.d.:

- Leit að spurningum
- Flokkun spurninga með möguleika á að búa til flokka
- Annað sem ykkur dettur í hug!

## Hópavinna

Verkefnið skal unnið í hóp með 3-4 einstaklingum. Hafið samband við kennara ef ekki er mögulegt að vinna í hóp. Hægt er að leita að félögum á slack á rásinni `#vef1-2025-vantar-hop`. Ekki er krafa að vera í sama hóp og í hópverkefni 1.

Notast skal við Git og GitHub. Engar zip skrár með kóða ættu að ganga á milli í hópavinnu, heldur á að „committa“ allan kóða og vinna gegnum Git.

Sjást ætti á _commit history_ að allir meðlimir hóps hafi tekið þátt í verkefni.

Útbúa þarf a.m.k. fimm Pull Request (PR) þar sem búið er að fara yfir af öðrum meðlim í hóp og yfirferð ásamt gagnrýni sést á GitHub. Ef um einstaklingsverkefni þarf að útbúa a.m.k. tvær PR þar sem viðkomandi fer yfir eigin kóða.

## Lýsing á verkefni

`README.md` skrá skal vera í rót verkefnis og innihalda:

- Upplýsingar um hvernig keyra skuli verkefnið:
  - `npm run dev` eða `npm start`.
  - `npm run lint` skal vera til staðar og keyra eslint og stylelint.
- Létt lýsing á uppsetningu verkefnis, hvernig því er skipt í möppur, hvernig CSS/Sass er skipulagt og fleira sem á við.
- Nákvæm útlistun á því hvað er útfært.
- Upplýsingar um alla sem unnu verkefni, nöfn, HÍ notendanöfn og GitHub notendanöfn.

## Tæki og tól

Verkefnið skal innihalda `package.json` og `package-lock.json` sem innihalda öll notuð tól.

Þegar verkefnið er sótt verður `npm install` keyrt á undan öllum öðrum skipunum.

Setja skal upp stylelint og eslint.

Leyfilegt er að nota öll tól sem við höfum notað í haust.

## Hýsing

Setja skal verkefnið upp á Netlify, tengt GitHub.

## Mat

- 10% README eftir forskrift, tæki og tól uppsett, vefur keyrir á Netilfy. Lint fyrir CSS/Sass og JavaScript.
- 10% Git notað og PR eftir forskrift.
- 10% Almennt útlit og skalanleiki útfært fyrir forsíðu og efnissíður.
- 10% Slóðir og síður fyrir hvert efni.
- 10% Grunvirkni útfærð.
- 50% Valið efni útfært.

Fyrir valið efni er metið:

- Einstaklingsverkefni: tvö auka verkefni útfært.
- Tveggja manna hópverkefni: þrjú auka verkefni útfærð.
- Þriggja manna hópverkefni: fjögur auka verkefni útfærð.
- Fjögurra manna hópverkefni: fimm auka verkefni útfærð.

## Sett fyrir

Verkefni fyrst sett fyrir í fyrirlestri mánudaginn 20. október 2025.

## Skil

Tilnefna skal hópstjóra sem skráir sig í ákveðinn hóp undir „Hópverkefni 2“ í Canvas. Aðrir nemendur skrá sig í framhaldinu í sama hóp, hópstjóri getur líka skráð aðra nemendur í hópinn.

**Útbúa skal hóp jafnvel ef verkefnið er unnið sem einstaklingsverkefni**.

Hópstjóri skal skila fyrir hönd allra í Canvas í seinasta lagi þriðjudaginn 18. nóvember 2025.

**Mikilvægt er að öll skil séu gerð í hóp annars munu ekki allir nemendur fá einkunn.**

Skil skulu innihalda:

- GitHub notendanöfn allra (passa þarf að allir nemendur séu í hópnum!)
- Slóð á verkefnið keyrandi í hýsingu
- Slóð á GitHub repo fyrir verkefni. Dæmatímakennurum skal hafa verið boðið í repo. Notendanöfn þeirra eru:
  - `klingsterina`
  - `kristinfrida`
  - `osk`
  - `reynirjr`

## Einkunn

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.1

## Útgáfusaga

| Útgáfa | Lýsing                     |
| ------ | -------------------------- |
| 0.1    | Fyrsta útgáfa verkefnisins |
