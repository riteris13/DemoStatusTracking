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
Pavyzdžiui, duomenų rinkyje "Gyventojai" naudojami savivaldybių kodus iš duomenų rinkinio "Adresų registras", bet tai yra atskiros IS duomenys, tad tieisogiai per esybę susieti negalime.

**7. Kodėl pirminė metaduomenų versija yra svarbi? Kas nusprendžia, kuri versija yra pirminė?**  
A: Pirminė versija  - tai naujausia, pagrindinė, paskelbta IS metaduomenų versija, kurią rekomenduojama naudoti visoms integracijoms ir sutarčių sudarymui. Tai versija, kuri paskelbiama po patvirtinimo - kai kuriama arba atnaujinama IS pereina į eksploatacijos stadiją.

**8. Kas yra duomenų paslauga? Kuo skiriasi IS paslauga nuo duomenų paslaugos?**
A: Duomenų paslauga - tai operacijų rinkinys, suteikiantis prieigą prie vieno ar daugiau duomenų rinkinių, dažniausiai tai API.  Paprastai sakant, tai elektroninė paslauga, suteikianti prieigą prie duomenų.

IS paslauga - bendresnė sąvoka, apibūdinanti IS teikiamas elektronines paslaugas (nebūtinai duomenų teikimui). Pavyzdžiui, elektroninė paslauga "Deklaruoti gyvenamąją vietą", arba "Registruoti transporto priemonę".

**9. Kodėl reikia naudoti kontroliuojamus žodynus?**  
A: Kontroliuojami žodynai - tai standartizuoti, institucijų tvirtinami sąrašai, kuriuose pateikiamos leidžiamos reikšmės tam tikroms metaduomenų savybėms. Naudojant kontroliuojamus žodynus yra užtikrinama, kad visos institucijos naudotų tas pačias, semantiškai suderintas reikšmes, kurios būtų suprantamos visų, tiek Lietuvos, tiek Europos, ar jei naudojami globalūs žodynai, Pasaulio lygmeniu.  

**10. Kas yra koncepcinis modelis ir kam jis reikalingas?**  
A: Koncepcinis modelis - tai semantinis IS duomenų modelis, apibrėžiantis aukšto lygio koncepcijas, daiktus, esybes ir ryšius tarp jų, nepriklausomai nuo technologinio realizavimo. Dažnai vaizduojamas diagramomis arba vaizdinėmis priemonėmis. Šio projekto kontekste yra kuriami UML koncepciniai nodeliai. Pavyzdžiui, aukšto lygio elementai (esybės), kurie gali būti atvaizduojami koncepciniame modelyje - asmuo, juridinis asmuo, apdraustasis, santuoka, nekilnojamo turto objektas.

**11. Kas yra pirminis duomenų šaltinis (*Master data*)?**  
A: Pirminis duomenų šaltinis - tai vienintelis, autoritetingas duomenų šaltinis. Jame pirmą kartą registruojami esybės objektai ir suteikiami globalūs identifikatoriai. Tai patikimas tiesos šaltinis (ang. *single source of truth*).

**12. Kas yra repozitorius?**  
A: Repozitorius - tai duomenų saugykla, DVMS metaduomenų kontekste tai GitHub platformos kodo saugykla, kurioje institucijos teikia metaduomenų failus ir gali sekti veiklų statusą DVMS projekto lentoje. Tai saugus ir patikimas būdas saugoti ir atnaujinti informaciją, kadangi yra palaikoma versijų istorija, tai yra, bet kada galima atkurti senesnę versiją, peržiūrėti pokyčius tarp versijų.  
  

## Rolės ir atsakomybės
**1. Kas yra duomenų tvarkytojas, duomenų valdytojas, duomenų valdymo įgaliotinis, duomenų administratorius ir duomenų architektas? Kuo jie skiriasi?**  
A: Duomenų tvarkytojas - tai subjektas, kuris tvarko duomenis techniniame lygmenyje, duomenų valdytojo vardu. Pavyzdžiui, IS administratorius.

Duomenų valdytojas - tai institucija, kuri valdo IS.  

Duomenų valdymo įgaliotinis - paskirtas asmuo, atsakingas už duomenų valdymo politikos įgyvendinimą.  

Duomenų administratorius - duomenų tvarkytojo paskirtas asmuo, kuris pildo techninius duomenis apie pateiktis, duomenų paslaugas, duomenų elementus.  Atsakingas už prieigos prie duomenų valdymą, IS saugos užtikrinimą, metaduomenų katalogo techinių įrašų palaikymą.

Duomenų architektas - duomenų tvarkytojo paskirtas asmuo, kuris atsakingas už veiklos srities ir semantinės informacijos pildymą, IS duomenų kokybės, prieigų prie metaduomenų valdymą.  

**2. Kas atsakingas už metaduomenų pildymą ir tvirtinimą?**  
A: Metaduomenis pildo duomenų architektas, IS duomenų valdymo įgaliotinis ir VSSA architektų komandos nariai teikia šiems metaduomenims atgalinį ryšį. Metaduomenis tvirtina VSSA komanda.  

**3. Kaip VSSA dalyvauja metaduomenų pildymo procese?**  
A: VSSA valdo bendrą duomenų infrastruktūrą, padeda institucijoms duomenų architektūros klausimais, tikrina supildytus metaduomenis.

## Įrankiai ir procesai
**1. Kas yra DCAT-AP-LT?**  
A: DCAT-AP-LT - tai DCAT‑AP specifikacijos plėtinys, kuris apjungia BRegDCAT‑AP, DCAT‑AP‑HVD ir Lietuvos specifinius elementus, kad būtų galima struktūrizuoti Lietuvos valstybinių IS metaduomenis ir suderinti juos su ES standartais.  

**2. Kas yra KDA ir DSA, kuo jie skiriasi nuo ŠDSA?**  
A: Duomenų struktūros aprašas (DSA) - specifikacija, pagal kurią rengiami duomenų struktūrų aprašymai, reikalingi duomenų mainams tarp informacinių sistemų.

ŠDSA - Šaltinio duomenų struktūros aprašas, kuriame aprašoma IS duomenų šaltinio struktūra. Jis yra automatiškai generuojamas duomenų agento "Spinta" pagalba.

Trumpai, ŠDSA yra automatinis fizinės struktūros atvaizdas, o DSA - rankiniu būdu koreguotas ŠDSA, galutinai parengtas loginis-semantinis aprašas, kuris skelbiamas kataloge.

KDSA tai nuo ŠDSA ir duomenų šaltinio nepriklausomas, pagal senmantinį ir veiklos srities supratimą paruoštas struktūros aprašymas.

**3. Kaip metaduomenų katalogas susijęs su duomenų portalu? Kas juos administruoja**  
A: Duomenų portalas yra techninė metaduomenų katalogo realizacija, kuri kaupia metaduomenis apie IS, organizacijas, atstovus, teikiamas paslaugas.  


## Metaduomenų pildymo procesas
**1. Kaip pakeisti validavimo taisykles DCAT-AP-LT Excel formoje, norint praplėsti eilučių skaičių?**  
A: Atidarykite pildomą DCAT-AP-LT formą, pasirinkite langelį, kuriame rodomas pasirinkimų sąrašas. Tuomet įrankių juostoje pasirinkite Duomenys -> Duomenų tikrinimas (ang. *Data -> Data Validation*). Iššokusiame nustatymų lange pakeiskite šaltinio (ang. *Source*) diapazoną iki reikiamo dydžio (pvz. A1:A:20 į A1:A30).  

**2. Kokios taisyklės galioja identifikatoriaus pavadinimui?**  
A: Identifikatoriai kuriami rankiniu būdu naudojant tik lotyniškas raides be tarpų, atskirus žodžius atskiriant pabraukimo "_" simboliu.  

**3. Kas yra kardinalumas ir kam jo reikia?**  
A: Kadinalumas nurodo, kiek reikšmių galima pateikti vienai savybei:  
- [1] - galima nurodyti tik vieną reikšmę
- [n] - galima nurodyti kelias reikšmes (nereiškia, kad nurodyti kelias reikšmes būtina).  
Kardinalumas reikalingas, kad būtų aišku, ar savybė gali turėti kelis įrašus, ar tik vieną.

**4. Ką reiškia DCAT Excel lapų spalvos žalia, geltona, rausva?**  
A: Žalia - privalomas pildyti lapas.  
Geltona - rekomenduojamas pildyti lapas.  
Rausva - pasirenkamai pildomas lapas.  

**5. Ką reiškia DCAT Excel langelių spalvos?**  
A: Tamsiai pilka - identifikatorius.  
Balta - pildoma laisvu tekstu, tiesiogiai suvedant reikšmes.  
Geltona - langelis turi pasirenkamas reikšmes iš jau sudarytų kontroliuojamų žodynų. Galima rinktis tik nurodytas reikšmes.  
Žalia - langelis turi pasirenkamas reikšmes iš kitų lapų. Norint juos užpildyti, turi būti sukurti reikiamos klasės egzemplioriai atitinkamuose lapuose, nurodytuose elemento paaiškinimuose.  

**6. Kam reikalingas `prepare` stulpelis DSA lentelėje?**  
A: "prepare" stulpelyje pildomos duomenų filtravimo ar paruošimo funkcijos. Tai leidžia aprašyti papildomas funkcijas, kaip filtravimas, konvertavimas. Taip pat modelių jungimui, papildomų savybių įtraukimui naudojamos agentui skirtos operacijos *include()*, *exclude()*, *expand()*.  

**7. Kuo skiriasi bazinis ir papildomas esybės modeliai?**  
A: Bazinis modelis aprašo pirminį duomenų šaltinį (vienintelis ir autoritetingas duomenų šaltinis, suteikiantis objektams globalius identifikatorius), kuriame pirmą kartą yra registruojami Esybės objektai. Jis DSA dokumente nurodomas be bazinio modelio (base stulpelio) reikšmės. Papildomi, arba išvestiniai modeliai nurodomi su bazinio modelio reikšme ir pakartotinai naudoja bazinio modelio duomenis, tai pat gali juos labiau išplėsti arba specializuoti.

**8. Kaip sužinoti esybės/modelio arba savybės/atributo brandos lygį?**  
A: Brandos lygis nurodomas "level" stulpelyje ir priklauso tiek nuo elemento metaduomenų tiek nuo tekiamų duomenų brandos. Priskiriami lygiai pagal tasykles DSA specifikacijoje. Aukščiausią brandą turi elementai, kurie yra susieti su semantiniais ištekliais, yra aiškiai aprašyti, yra žinomas teikiamų duomenų formatas, vienetai, tikslumas, jei tai modeliai(esybės) yra žinomi ir patikimi pirminiai raktai. 

**9. Kaip galima jungti modelius DSA lentelėse?**  
A: Modelių jungimas atliekamas per "property" reikšmę, kai "type" nurodoma *ref*. "ref" stulpelyje nurodomas kito modelio pavadinimas, arba pilnas URI.  
 Jeigu modelis jungiamas ne per pirminį raktą, savybės, per kurias jungiama nurodomos laužtiniuose skliaustuose po jungiamo modelio URI.   
Jeigu jungimui yra naudojamas kompleksinis raktas, jungimo savybės yra nurodomos laužtiniuose skliaustuose, jas atskiriant kableliu. Tokiu atveju "prepare" stulpelyje taip pat reikia nurodyti jungimui naudojamas savybes.   

**10. Kada DSA pildomas pagal šabloną, o kada pagal ŠDSA? Kas skiriasi?**  
A: Pagal ŠDSA pildome tada, kai turime agento sugeneruotą fizinės struktūros aprašą.   
Pagal šabloną pildome tada, kai fizinis modelis yra nežinomas, arba agentas nėra naudojamas.  

**11. Kaip patikrinti, ar pildomi duomenys atitinka kontroliuojamus žodynus?**  
A: 
- DCAT-AP-LT Excel formoje: geltonos spalvos langeliai yra automatiškai susieti su kontroliuojamais žodynais, reikia tik pasiirnkti tinkamą.
- DSA formoje: jei norite rankiniu būdu nurodyti žodyną savybei, "uri" stulpelyje įrašykite žodyno URI.
- Žodynų sąrašai pateikti DCAT-AP-LT specifikacijoje ir metaduomenų pildymo vadovo skyriuje "Kontroliuojami žodynai".
- Norėdami nustatyti, kokį žodyną naudoti, DCAT-AP-LT Excel formoje vadovaukitės savybės aprašymu, o pildant DSA - DSA specifikacija.   

**12. Kuo skiriasi pildymas pagal gyvavimo stadijas nuo pildymo DVMS projekto apimtyje?**  
A: Pagal gyvavimo stadijas - tai pagrindinis metaduomenų pildymo į metaduomenų katalogą procesas. Pildymas vykdomas pagal IS gyvavimo ciklą (steigimas, kūrimas, eksploatavimas, atnaujinimas, likvidavimas) ir Valstybės Informacinių Išteklių Valdymo Įstatymo reikalavimus.

Pildymas DVMS projekto apimtyje skiriasi nuo pildymo pagal gyvavimo stadijas, nes dauguma projekto apimtyje aprašomų IS jau yra eksploatuojamos, tad metaduomenys pildomi pagal įgyvendintą faktinę duomenų ir IS informaciją. Atliekamas pirminis metaduomenų užpildymas. Procesas skirstomas į tris pagrindinius etapus: 
- pagrindinės informacijos apie IS užpildymas ir DSA pildymas;
- duomenų rinkinių ir DSA apjungimas į bendrą modelį;
- veiklos terminijos gryninimas ir semantinis praturtinimas.  
Pasiekus reikiamą pilnumą bei kokybę, bei gavus patvirtinimą, metaduomenys skelbiami metaduomenų kataloge.  
 

## Metaduomenų versijavimas ir statusai
**1. Ar galima turėti kelias aktyvias metaduomenų versijas tuo pačiu metu?**  
A: Taip, kataloge gali būti kelios aktyvios versijos. Verta atkreipti dėmesį, jog aktyvi nuomatytoji versija gali būti tik viena, pagal nutylėjimą ji yra naujausia išlesta versija.  

**3. Kada reikia kurti naują metaduomenų versiją?**  
A: Nauja versija kuriama, kai:
- Įvyksta reikšmingi IS pokyčiai (pvz. nauji duomenų rinkiniai, naujos paslaugos),  
- Keičiami duomenų teikimo būdai ar semantika.


## DVMS projekto lenta
**1. Kaip teikti rezultatus per GitHub repozitorių?**  
A: Apibendrinta žingsnių seka pateikiama žemiau, išsamesni paaiškinimai pateikti Metaduomenų pildymo vadove.
- Pirmiausia reikia DVMS projekto lentoje sukurti naują IS užduotį.   
- Toliau, pasiruošus įkelti rezultataus, užduoties statusas pakeičiamas į "Ruošiama", sukuriama nauja šaka (ang. *branch*).   
- Sukūrus šaką, į jos *datasets/gov* aplanką sukuriami laikini failai pagal struktūrą:  
metadata/datasets/gov/<institucija>/<is>/DCAT-AP-LT-Meta.xlsx  
metadata/datasets/gov/<institucija>/<is>/<duomenų_rinkinys>/dsa.csv    
- Tikrieji failai įkeliami per "Add file" -> "Upload files", o juos įkelus atliekamas "Commit changes"
- Pasiruošus teikti rezultatus šakoje, kurioje yra teikiami rezultatai spaudžiame "Contribute", tada "Open pull request", tada "Create pull request"
- Perkeliame užduotį į "Pateikta tikrinimui" stulpelį DVMS projekto lentoje.

**2. Kaip sukurti IS užduotį?**  
A: DVMS projekto lentoje spaudžiama "Add Item", tada "Create new issue", pasirenkamas užduoties tipas "Informacinės sistemos užduotis". Sukūrus užduotį reikia supildyti projekto duomenų kortelę, pateikiant tokius duomenis, kaip: institucijos pavadinimas, IS kodinis pavadinimas, koordinatorius, įgyvendinimo būdas.

**3. Kaip įkelti DCAT-AP-LT Excel failą į GitHub?**  
A: Apibendrinta žingsnių seka pateikiama žemiau, išsamesni paaiškinimai pateikti Metaduomenų pildymo vadove.
- Pirmiausia sukuriama nauja šaka (ang. *branch*). 
- Tada pasirenkame *datasets/gov* aplanką, jame spaudžiame "Add file", tada "Create new file".   
- Toliau pagal nurodymus sukuriamas laikinas failas su aplanko struktūra: "metadata/datasets/gov/<institucija>/<is>/DCAT-AP-LT-Meta.xlsx" (čia institucija ir is įrašomi institucijos ir IS kodiniai pavadinimai). 
- Spaudžiamas mygtukas "Commit changes". 
- Sekantis žingsnis yra įkelti tikrąją failo versiją: spaudžiamas "Upload files" mygtukas, įkeliama tikroji failo versija.
- Spaudžiama "Commit changes".  

**4. Kaip įkelti DSA failą į GitHub?**  
A: Apibendrinta žingsnių seka pateikiama žemiau, išsamesni paaiškinimai pateikti Metaduomenų pildymo vadove.  
- Pirmiausia sukuriama nauja šaka (ang. *branch*). 
- Tada pasirenkame *datasets/gov* aplanką, jame spaudžiame "Add file", tada "Create new file". 
- Toliau pagal nurodymus sukuriamas laikinas failas su aplanko struktūra: "metadata/datasets/gov/<institucija>/<is>/<duomenų rinkinys>/dsa.csv" (čia institucija ir is įrašomi institucijos ir IS kodiniai pavadinimai). 
- Spaudžiamas mygtukas "Commit changes". 
- Sekantis žingsnis yra įkelti tikrąją failo versiją: spaudžiamas "Upload files" mygtukas, įkeliama tikroji failo versija.
- Spaudžiama "Commit changes".  

**5. Kaip atlikti „Pull request“ ir pateikti rezultatus tikrinimui?**  
A: 
- Šakoje, kurioje yra teikiami rezultatai spaudžiame "Contribute", tada "Open pull request", tada "Create pull request"
- Perkeliame užduotį į "Pateikta tikrinimui" stulpelį DVMS projekto lentoje.

**6. Kaip peržiūrėti pokyčius GitHub platformoje?**  
A: Pokyčius peržiūrėti galima tuo atveju, jei GitHub platforma palaiko tų dokumentų tipo atvaizdavimą. Tokiu atveju:
- Pasirenkame sukurtą "Pull request", tada spaudžiame "Files changed" kortelę.
- Atsidariusiame lange matysime failo pakeitimus: raudonai žymimi šalinimai, o žaliai - pridėjimai.  

**7. Kaip teikti komentarus apie pakeitimus?**  
A: Apibendrinta žingsnių seka pateikiama žemiau, išsamesni paaiškinimai pateikti Metaduomenų pildymo vadove.  Komentarus galima teikti per pakeitimų peržiūros langą:  
- Pasirenkame sukurtą "Pull request", tada spaudžiame "Files changed" kortelę.  
- Atsidariusiame lange matysime failo pakeitimus.  
- Užvedus pelytę ant norimos komentuoti eilutės, paspaudus mėlyną "+" kairėje pusėje, atidaromas komentaro teikimo langas.  
- Spaudžiame "Start a review".  
- Surašius norimus komentarus, viršuje spaudžiame "Review changes".  
- Pasirodžiusiame lange paspaudus "Submit review" komentarai bus pateikti.  

**8. Kada rezultatai paskelbiami „main“ šakoje?**  
A: Rezultatus galima viešinti, juos pateikiant "main" šakoje, tik po VSSA komandos patikrinimo ir patvirtinimo. Siekiant rezultatus paskelbti, pasirenkame rezultatams sukurtą "Pull request", ir, jei pavyko automatiniai tikrinimai, pasirenkame "Merge pull request".
 
