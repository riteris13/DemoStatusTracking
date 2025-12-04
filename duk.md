# D.U.K.
## Sąvokos
**1. Kas yra metaduomenys?**  
A: Metaduomenys – tai duomenys apie duomenis, naudojami resursų aprašymui ir suradimui. Jie padeda suvokti savo ir kitų duomenis, palengvina duomenų kokybės vertinimą, palaiko duomenų bazių integraciją bei taikomųjų programų veikimą. Metaduomenys yra būtini sklandžiam duomenų apdorojimui, priežiūrai, integracijai, saugumui, auditui ir valdymui.  

**2. Kas yra duomenų agentas, kam jis skirtas ir kaip naudojamas?**  
A: Duomenų agentas („Spinta“) – tai programinis įrankis, skirtas duomenų teikimo paslaugų teikimui pagal UDTS (universalus duomenų teikimo standartas), ir ŠDSA (šaltinio duomenų struktūros aprašo) generavimui.  

**3. Kas yra metaduomenų katalogas? Kur jis saugomas?**  
A: Metaduomenų katalogas – gamybinėje aplinkoje veikiantis data.gov.lt portalas, čia saugomi Lietuvos valstybinių informacinių sistemų metaduomenys pagal DCAT-AP-LT specifikaciją. Katalogas yra administruojamas VSSA.  

**4. Kas yra duomenų struktūra (esybė)?**  
A: Duomenų struktūra (esybė) - tai loginis duomenų modelio elementas, apibūdinantis objektą ir jo savybes. Pavyzdžiui, jei IS tvarko duomenis apie pastatus, „Pastatas“ bus esybė, o jos savybės gali būti „adresas“, „aukštų skaičius“, „plotas“.  

**5. Kas yra IS objektai ir klasifikatoriai?**  
A: IS objektai – tai informacinės sistemos koncepcinio modelio esybės (pavyzdžiui, asmuo, adresas). Klasifikatoriai – tai pakartotinai naudojami referenciniai duomenys (pvz., valiutų kodai, šalių sąrašai), siekiant užtikrinti vienodą šių duomenų interpretaciją.  

**6. Kas yra kvalifikuotas ryšys tarp duomenų rinkinių ir kitų metaduomenų katalogo išteklių?**  
Kvalifikuotas ryšys - tai papildomas ryšys su kitais metaduomenų katalogo ištekliais, kurie nėra susieti per standartines savybes. DCAT-AP-LT formoje į savybę "Kvalifikuotas ryšys" nurodome duomenų rinkinio ryšį su kitais katalogo objektais, kai nėra galimybės tą ryšį priskirti per egzistuojančią savybę.  

**Kaip atpažinti kvalifikuotą ryšį?**  
 Kvalifikuotas ryšys egzistuoja, kai:  
* Jei duomenų rinkinys priklauso nuo kito ištekliaus (pvz., naudoja klasifikatorius, teisės aktus, semantinius ryšius), bet formoje nėra tam skirto lauko;  
* Jei ryšys yra semantinis ar kontekstinis, o ne techninis per API;  
* Jei ryšys duomenims suteikia papildomą informaciją, kuri svarbi duomenų naudotojams.  
Pavyzdžiui, duomenų rinkyje "Gyventojai" naudojami savivaldybių kodus iš duomenų rinkinio "Adresų registras", bet tai yra atskiros IS, tad per esybę susieti negalime.

**7. Kodėl pirminė metaduomenų versija yra svarbi? Kas nusprendžia, kuri versija yra pirminė?**  
A: Pirminė versija  - tai naujausia, pagrindinė, paskelbta IS metaduomenų versija, kurią rekomenduojama naudoti visoms integracijoms ir sutarčių sudarymui. Tai versija, kuri paskelbiama po patvirtinimo - kai kuriama arba atnaujinama IS pereina į eksploatacijos stadiją.  

**8. Kas yra duomenų paslauga? Kuo skiriasi IS paslauga nuo duomenų paslaugos?**  
A: Duomenų paslauga - tai operacijų rinkinys, suteikiantis prieigą prie vieno ar daugiau duomenų rinkinių, dažniausiai tai API.  Paprastai sakant, tai elektroninė paslauga, suteikianti prieigą prie duomenų.  

IS paslauga - bendresnė sąvoka, apibūdinanti IS teikiamas elektronines paslaugas (nebūtinai duomenų teikimui). Pavyzdžiui, elektroninė paslauga "Deklaruoti gyvenamąją vietą", arba "Registruoti transporto priemonę".  

**9. Kodėl reikia naudoti kontroliuojamus žodynus?**  
A: Kontroliuojami žodynai - tai standartizuoti, institucijų tvirtinami sąrašai, kuriuose pateikiamos leidžiamos reikšmės tam tikroms metaduomenų savybėms. Naudojant kontroliuojamus žodynus yra užtikrinama, kad visos institucijos naudotų tas pačias, semantiškai suderintas reikšmes, kurios būtų suprantamos visų, tiek Lietuvos, tiek Europos, ar jei naudojami globalūs žodynai, Pasaulio lygmeniu.  

**10. Kas yra koncepcinis modelis ir kam jis reikalingas?**  
A: Koncepcinis modelis - tai semantinis IS duomenų modelis, apibrėžiantis aukšto lygio koncepcijas, daiktus, esybes ir ryšius tarp jų, nepriklausomai nuo technologinio realizavimo. Dažnai vaizduojamas diagramomis arba vaizdinėmis priemonėmis. Pavyzdžiui, aukšto lygio subjektai gali būti viešosios paslaugos, viešosios institucijos.  

**11. Kas yra pirminis duomenų šaltinis (*Master data*)?**  
A: Pirminis duomenų šaltinis - tai vienintelis, autoritetingas duomenų šaltinis. Jame pirmą kartą registruojami esybės objektai ir suteikiami globalūs identifikatoriai. Tai patikimas tiesos šaltinis (ang. *single source of truth*).  

**12. Kas yra repozitorius?**  
A: Repozitorius - tai GitHub saugykla, kurioje institucijos teikia metaduomenų failus ir gali sekti statusą DVMS projekto lentoje. Tai saugus ir patikimas būdas saugoti atnaujinti informaciją, kadangi yra palaikoma versijų istorija, tai yra, bet kada galima atkurti senesnę versiją, peržiūrėti pokyčius tarp versijų.  
  

## Rolės ir atsakomybės
**1. Kas yra duomenų tvarkytojas, duomenų valdytojas, duomenų valdymo įgaliotinis? Kuo jie skiriasi?**  
**2. Kas atsakingas už metaduomenų pildymą ir tvirtinimą?**  
**3. Kaip VSSA dalyvauja metaduomenų pildymo procese?**  

## Įrankiai ir procesai
**1. Kas yra DCAT-AP-LT?**  
**2. Kas yra DSA, kuo tai skiriasi nuo ŠDSA?**  
**3. Kaip metaduomenų katalogas susijęs su duomenų portalu? Kas juos administruoja?**  

## Pildymo procesas
**1. Kaip pakeisti validavimo taisykles Excel, norint praplėsti eilučių skaičių?**  
**2. Kokios taisyklės galioja identifikatoriaus pavadinimui?**  
**3. Kas yra kardinalumas ir kam jo reikia?**  
**4. Ką reiškia DCAT Excel lapų spalvos žalia, geltona, raudona?**  
**5. Ką reiškia DCAT Excel langelių spalvos?**  
**6. Kam reikalingas `prepare` stulpelis DSA lentelėje?**  
**7. Kuo skiriasi bazinis ir papildomas esybės modeliai?**  
**8. Kaip sužinoti esybės/modelio brandos lygį?**  
**9. Kaip galima jungti modelius DSA lentelėse?**  
**10. Kada DSA pildomas pagal šabloną, o kada pagal ŠDSA? Kas skiriasi?**  
**11. Kaip patikrinti, ar pildomi duomenys atitinka kontroliuojamus žodynus?**  
**12. Kuo skiriasi pildymas pagal gyvavimo stadijas nuo pildymo DVMS projekto apimtyje?**  

## Versijavimas ir statusai
**1. Kuo skiriasi statusai `Patvirtinta`, `Paskelbta [Aktyvi]`, `Paskelbta [Neaktyvi]`?**  
**2. Ar galima turėti kelias aktyvias versijas tuo pačiu metu?**  
**3. Kada reikia kurti naują metaduomenų versiją?**  

## DVMS projekto lenta
**1. Kaip teikti rezultatus per GitHub repozitorių?**  
**2. Kaip naudotis DVMS projekto lenta?**  
**3. Kaip sukurti IS užduotį?**  
**4. Kaip įkelti DCAT-AP-LT Excel failą į GitHub?**  
**5. Kaip įkelti DSA failą į GitHub?**  
**6. Kaip atlikti „Pull request“ ir pateikti rezultatus tikrinimui?**  
**7. Kaip peržiūrėti pokyčius GitHub platformoje?**  
**8. Kaip teikti komentarus apie pakeitimus?**  
**9. Kada rezultatai paskelbiami „main“ šakoje?**  
