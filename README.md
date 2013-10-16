Softverove-inzinierstvo1
========================

Projekt UML na predmet Softvérové inžinierstvo 1

Projekt sa nachadza a stiahnete si ho:

`git clone https://github.com/SvetlanaM/Softverove-inzinierstvo-1.git`


Zadanie projektu
========================

Car Rental System
--
Uvažujme společnost CarRental, český řetězec orientovaný na půjčování vozidel s pobočkami ve třech
českých městech (Praha, Brno, Ostrava) a plánovaným rozšířením do dalších měst. Nový informační systém
by měl podporovat následující funkcionalitu.

Registracia
--
Společnost CarRental nabízí možnost výpůjčky vozidel pouze registrovaným zákazníkům. Registrace může
proběhnout dvěma způsoby. Prvním je osobní registrace na pobočce. Druhým je dvoufázová registrace,
skládající se z online předregistrace (uživatelské jméno, heslo, kontaktní informace) a osobního dokončení
registrace na pobočce (naskenování dokladu totožnosti a řidičského průkazu).

Členství
--
Při registraci má zákazník možnost stát se členem CarRental klubu, což s sebou přináší zasílání informací o
novinkách a možnost využití nabízených slev (napr. prázdninová, Vánoční). Členové klubu s častým
využíváním služeb (dle útraty za posledních 12 měsíců) se navíc stávají Premium členy, kteří mají slevu 10%
na všechny služby. Rozlišujeme tak Members a Premium Members. Premium Members se v případě poklesu
využívání služeb stávají opět Members. Na tuto skutečnost jsou upozorněni emailem.

Vozidla
--
Společnost CarRental spravuje vozový park skládající se z osobních automobilů, dodávek a motorek různých
značek, typů a parametrů. Pro každý druh vozidla (značka, typ a parametry) je k dispozici více kusů, které
jsou dle potřeby obměňovány (nákup od smluvního partnera, prodej v aukci). Databáze vozidel je pro
všechny pobočky jednotná.

Výpůjčka
--
Proces začíná nejčastěji rezervací vozidla (dle druhu) ve zvoleném termínu online nebo na pobočce.
Specifikuje se pobočka, kde bude vozidlo vypůjčeno, i pobočka, kde bude navráceno (za příplatek, 
pokud se místa liší). Pokud není vozidlo zvoleného druhu na pobočce k dispozici, může zákazník požádat o
jeho převoz z jiné pobočky (za příplatek). Rezervaci může zadat pouze registrovaný nebo i předregistrovaný
zákazník. Rezervace se stává platnou po zaplacení zálohy (ve stanoveném termínu). Dokud není rezervace
platná, je možné ji zrušit bez storno poplatku. Při rušení platné rezervace se účtuje storno poplatek. Výpůjčka
začíná fyzickým vyzvednutím vozidla, které je možné pouze pro registrované zákazníky (nikoli jen
předregistrované). Výpůjčka je možná i bez předchozí rezervace - pokud je požadované vozidlo k dispozici.
Výpůjčka končí fyzickým navrácením vozidla, po kterém probíhá finanční dorovnání (se započítáním
případných škod na vozidle).

Převoz
--
Každé vozidlo má svou domovskou pobočku, kde stojí, pokud není vypůjčeno nebo připraveno k vypůjčení
na jiné pobočce. Pokud zákazník v rezervaci požádá o vypůjčení vozidla na jiné pobočce, musí být tento
požadavek nejprve schválen manažerem domovské pobočky vozidla. Po navrácení je vozidlo převezeno zpět
na domovskou pobočku. K převezení dochází také u vozidel vypůjčených na domovské pobočce, ale
navrácených na jiné pobočce.

Uživatelé
--
Mimo zákazníků a agentů na pobočkách k systému přistupují manažeři (každá pobočka má svého manažera,
jeden z nich je manažerem celé společnosti), kteří mají k dispozici řadu statistik o vytíženosti 
jednotlivých druhů vozidel, nákupní a prodejní ceně konkrétních vozidel, generovaném obratu. Manažeři
rozhodují o nákupu nových vozidel, prodeji starších vozidel, termínech aukcí a změnách v druzích
nabízených vozidel. Posledním typem uživatelů jsou technici, kteří udržují chod systému a na žádost
manažerů spravují přístupová práva ostatních uživatelů (např. v případě povýšení agenta na manažera).
