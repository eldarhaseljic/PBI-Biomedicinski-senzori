# PBI-Biomedicinski-senzori
Fakultet elektrotehnike Tuzla - Principi biomedicinskog inzenjeringa
```
UNIVERZITET U TUZLI
FAKULTET ELEKTROTEHNIKE
```
# SEMINARSKI RAD

## Principi biomedicinskog inženjeringa

## BIOMEDICINSKI SENZORI

```
Student: Haseljić Eldar
```
```
Profesor:
Dr.sc. Damir Demirović
vanr.prof.
```
Tuzla, mart/ožujak 2020.


## Sažetak

_U ovom seminarskom radu ćemo_ govoriti o biomedicinskim senzorima, njihovoj upotrebi,
_podjeli te načinu njihovog rada i_ o senzorima _uopće. Senzor je uređaj koji mjeri fizički kvantitet i
konvertuje ga u signal kojeg može očitavati posmatrač ili instrument._

Sama podjela, _odnosno klasifikacija senzora je dosta složena, i vrši se u odnosu prema: izvoru
napajanja, načinu upotrebe, obliku signala koji daje na svom izlazu, prirodi izlazne veličine itd._

Ključne riječi: signal, senzor, hemijski, fizički, biomedicinski


## Abstract

In this seminar work we will talk about biomedical sensors, their use, partition, mode and
sensor mode at all. The sensor is a device that measures the physical quantity and converts it into a
signal that the reader or instrument can read.
The same division or classification of sensors is quite complex, and is related to: source of
power, mode of use, signal form at its output, nature of output size, etc.

Key words: signal, sensor, chemical, physical, biomedical


## Sadržaj



- 1. Uvod
- 2. Klasifikacija senzora
   - 2.1. Klasifikacija po obliku signala na izlazu senzora
   - 2.2. Klasifikacija prema izvoru napajanja
   - 2.3. Klasifikacija po tipu senzora
   - 2.4. Klasifikacija na osnovu biotransdukcije.....................................................................
   - 2.5. Biomedicinska klasifikacija
- 3. Biomedicinski senzori
   - 3.1. Specifikacije senzora
      - 3.1.1. Osjetljivost..........................................................................................................
      - 3.1.2. Opseg
      - 3.1.3. Tačnost
      - 3.1.4. Preciznost
      - 3.1.5. Rezolucija
      - 3.1.6. Reproducibilnost
      - 3.1.7. Ofset
      - 3.1.8. Linearnost
      - 3.1.9. Vrijeme odziva
      - 3.1.10. Pomak
      - 3.1.11. Histereza
   - 3.2. Bioanalitički senzori
   - 3.3. Biosenzori u praćenju okoliša
      - 3.3.1. Enzimski biosenzori
   - 3.4. Senzori krvnih gasova
      - 3.4.1. Senzori za mjerenje kisika
      - 3.4.2. Ph Elektorde
      - 3.4.3. Senzori karbon dioksida
- 4. Optički senzori
   - 4.1. Optička vlakna
   - 4.2. Senzorski mehanizmi
   - 4.3. Imunološki senzori
- 5. Fizička mjerenja
   - 5.1. Transduktor protoka zraka........................................................................................
   - 5.2. Senzori za mjerenje temperature
      - 5.2.1. Termistori
      - 5.2.2. Bubni termometar
      - 5.2.3. Trenutni arterijski termometar..........................................................................
- 6. EKG simulacija pomoću MATLAB-a
   - 6.1. Značajne osobine valnog oblika EKG-a.
   - 6.2. Matlab kod
      - 6.2.1. main.m
      - 6.2.2. p_wav.m
      - 6.2.3. q_wav.m
      - 6.2.4. qrs_wav.m
      - 6.2.5. s_wav.m
      - 6.2.6. t_wav.m
      - 6.2.7. u_wav.m
- 7. Literatura
- Slika 1. Senzori........................................................................................................................... Popis slika
- Slika 2. Infracrveni senzor..........................................................................................................
- Slika 3.Klasifikacija na osnovu biotransdukcije
- Slika 4.Kalibracijska krivulja ulaza prema izlaznom tipičnom senzoru.
- greškama pomaka. Slika 5.Promjene ulaza u odnosu na izlazni odziv uzrokovane (a) greškama osjetljivosti i (b)
- Slika 6.Ulaz u odnosu na izlazni odziv senzora sa histerezom.
- Slika 7.Šematski prikaz hemiskog senzora
- Slika 8.Generički bioanalitički sensor
- Slika 9.Biosenzori
- Slika 10. Princip rada senzora za glukozu.
- Slika 11.Princip rada polarografskog Clarkovog tipa pO2.
- Slika 12. Transkutani senzor pO2.
- Slika 13. (a) pulsna sonda za pulsni oksimetar prsta i (b) jednokratni senzor prsta.
- pokazuje učinak arterijske pulsacije. Slika 14.Vremenska ovisnost apsorpcije svjetlosti kroz sloj perifernog vaskularnog tkiva
- Slika 15.Princip rada pH elektrode...........................................................................................
- Slika 16. Princip rada pCO2 elektrode
- Slika 17.Građa optičkog vlakna
- Slika 18.Princip senzora temelenog na optičkim vlaknima
- Slika 19.Princip rada optickih imunoloških senzora
- Slika 20.Fleish pretvarač zraka
- Slika 21.Uobičajeni oblici termistora
- Slika 22. Otporno - temperaturna karakteristika tipičnog termistora
- Slika 23.Swan-Ganz-ov kateter sa termodilucijom.
- Slika 24. Infracrveni termometar za uši bez kontakta.
- Slika 25.Trenutni arterijski termometar
- Slika 26.EKG signal
- Slika 27.Prikaz EKG signala nakon pokretanja skripte


## 1. Uvod

Senzor (njem. Sensor, engl. sensor, prema lat. sensus: osjećanje; osjećaj; osjetilo) pretvornik
ili mjerno osjetilo je dio mjernoga sistema koji u izravnom dodiru s mjerenom veličinom daje izlazni
signal ovisan o njezinom iznosu. Zbog prevladavajuće
primjene električnih i elektroničkih sistema, većina
senzora pretvara mjerenu veličinu u električki mjerljiv
signal. Tako se na primjer mehaničko titranje
membrane koja čini jednu ploču električnoga
kondenzatora u mikrofonu, uzrokovan zvučnim
talasima, pretvara u promjenu električnoga kapaciteta.
Senzor dakle mjeri fizikalnu veličinu (na primjer
temperaturu, vlažnosti zraka, pritisak , broj okretaja
motora) i pretvara ju u signal pogodan za daljnju
obradu (najčešće u električni signal). Senzori se
koriste prilikom izrade svakodnevnih predmeta, kao
što su dugmad lifta (osjetilni senzor), lampa koja se
pali na dodir, uređaji za praćenje broja koraka i sl.
Senzor je uređaj koji prima signal i reaguje na
njega tj. na neki poticaj. Poticaj mora biti konvertovan u električnu formu. Signal tako konvertovan
može biti korišten dalje u elektroničkim uređajima.

## 2. Klasifikacija senzora

Postoji nekoliko klasifikacija senzora napravljenih od strane različitih autora i stručnjaka. Neki
su vrlo jednostavni, a neki složeni.
Klasifikacije se vrše u odnosu na:

- tip senzora
- oblik signala kojeg daju na izlazu
- na osnovu izvora napajanja
- na osnovu biotransdukcije
- biomedicinska klasifikacija
- i slicno.

### 2.1. Klasifikacija po obliku signala na izlazu senzora

- Analogni senzori

```
Na svom izlazu daju kontinualni, neprekidni niz vrijednosti. Izlazni signal je
proporcionalan veličini koja se mjeri, a informacija o vrijednosti veličine koja se mjeri je
sadržana u amplitudi izlaznog signala. Izlaz ovih senzora se obično preko analogno-digitalnog
(A/D) konvertera povezuje na određeni uređaj. Analogni signal se dalje prenosi do uređaja
daljinske obrade signala gdje se obavlja znatno složenija obrada i procesiranje signala tj
pretvaranje analognog oblika u digitalni.
```
### Slika 1. Senzori


- Digitalni senzori

```
Podrazumjeva mjerni uređaj koji konvertuje mjernu analognu veličinu u digitalni izlazni
signal. Gradi se na bazi mikrokontrolera, što omogućava visok metrološki kvalitet i značajnu
obradu mjerne informacije. Digitalni senzori su poznati po svojoj tačnosti i jednostavnim
povezivanjem na uređaj za obradu.
```
### 2.2. Klasifikacija prema izvoru napajanja

- Aktivni senzori

```
To je uređaj koji vrši pretvaranje neelektričnih mjernih
veličina u električne. Pretvarači koji rade na ovaj način zovu se
aktivni pretvarači. Aktivni pretvarači za svoj rad ne trebaju
dodatnu energiju, te se široko koriste u proizvodnji i umrežavanju
okruženja, kao na primjer za nadgledanje industrijskih mašina.
```
- Pasivni senzor

```
To je uređaj koji detektuje i odgovara na nadražaj iz fizičke okoline. Pasivni senzor
sakuplja podatke kroz detekciju radijacije, svjetla, toplote ili nekih drugih fenomena koji se
javljaju u okruženju subjekta. Primjer tehnologija koje su bazirane na pasivnim senzorima su:
fotografska, termalna, hemijska, infracrvena.
```
### 2.3. Klasifikacija po tipu senzora

- Mehanički
- Toplinski
- Radijacijski
- Magnetski
- Hemijski
- Biomedicinski senzori

### 2.4. Klasifikacija na osnovu biotransdukcije.....................................................................

- Elektrokemijski
- Optički
- Elektronski
- Piezoelektrični
- Gravimetrijski
- Piroelektrični

## Slika 2. Infracrveni senzor..........................................................................................................

## Slika 3.Klasifikacija na osnovu biotransdukcije


### 2.5. Biomedicinska klasifikacija

Biomedicinski senzori obično se klasificiraju **prema količini koja se mjeri** i obično se
kategoriziraju kao **fizička, električna ili kemijska** , ovisno o njihovoj konkretnoj primjeni. Biosenzori,
koji se mogu smatrati posebnom podklasifikacijom biomedicinskih senzora, skupina su senzora koji
imaju **elemente biološkog prepoznavanja** , poput pročišćenog enzima, antitijela ili receptora. Svrha
pretvornika je pretvoriti biokemijsku reakciju u oblik optičkog, električnog ili fizičkog signala koji je
proporcionalan koncentraciji određene hemikalije. Stoga se senzor pH krvi ne smatra biosenzorom
prema ovoj klasifikaciji, premda mjeri biološki važnu varijablu.

## 3. Biomedicinski senzori

Dijagnostička bioinstrumentacija koristi se rutinski u kliničkoj medicini i biološkim
istraživanjima za mjerenje širokog raspona fizioloških varijabli. Općenito, mjerenje se dobiva iz senzora
ili pretvarača, a instrument ih dalje obrađuje radi dobivanja vrijednih dijagnostičkih informacija.
Biomedicinski senzori ili pretvarači glavni su sastavni dijelovi dijagnostičke medicinske
instrumenatacije koja se nalazi u mnogim liječničkim ordinacijama, kliničkim laboratorijama i
bolnicama.
Uređaji se također koriste u i nemedicinskim primjenama kao što su nadzor nad okolišem,
poljoprivreda, bioprocesiranje, prerada hrane te petrokemijska i farmakološka industrija. Općenito,
medicinski dijagnostički instrumenti dobivaju svoje podatke od senzora, elektroda ili pretvarača.
Medicinska instrumentacija se oslanja na analogne električne signale koji se uzimaju za ulaz. Ti se
signali mogu dobiti izravno biopotencijalnim elektrodama - na primjer, nadgledanjem električnih
signala koje stvaraju srce, mišići ili mozak, ili posredno pomoću pretvarača koji pretvaraju neelektričnu
fizičku varijablu, poput tlaka, protoka ili temperature, ili biokemijsku varijable, kao što su djelomični
pritisci plinova ili ionske koncentracije, na električni signal.
Biomedicinski senzori igraju važnu ulogu u širokom rasponu dijagnostičkih medicinskih
primjena. Ovisno o specifičnim potrebama, neki se senzori koriste prvenstveno u kliničkim
laboratorijima za mjerenje fizioloških količina kao što su elektroliti, enzimi i drugi biokemijski
metaboliti u krvi. Ostali biomedicinski senzori za mjerenje tlaka, protoka i koncentracija plinova, poput
kisika i ugljičnog dioksida, koriste se za kontinuirano praćenje stanja pacijenta.

### 3.1. Specifikacije senzora

Potreba za točnim medicinskim dijagnostičkim postupcima postavlja stroge zahtjeve u dizajnu i
uporabi biomedicinskih senzora. Ovisno o planiranoj primjeni, performanse specifikacije
biomedicinskog senzora mogu se procijeniti, kako bi se osiguralo da mjerenje zadovoljava projektne
specifikacije. Da bismo razumjeli karakteristike performansi senzora, važno je najprije razumjeti neke
uobičajene terminologije povezane sa specifikacijama senzora. Sljedeće definicije obično se koriste za
opisivanje karakteristika senzora i odabir senzora za pojedine primjene.

#### 3.1.1. Osjetljivost..........................................................................................................

Osjetljivost se obično definira kao omjer promjene izlaza za
datu promjenu ulaza. Drugi način za definiranje osjetljivosti je
pronalaženje nagiba kalibracijske linije koji se odnosi na ulaz (izlaz,
tj. DOutput / DInput), kao što je prikazano na slici 4. Visoka
osjetljivost podrazumijeva da mala promjena ulazne količine
uzrokuje veliku promjenu u izlazu. S druge strane, osjetljivost se
također može definirati kao najmanja promjena ulazne količine koja
će rezultirati detektabilnom promjenom u izlazu senzora.

## Slika 4.Kalibracijska krivulja ulaza prema izlaznom tipičnom senzoru.


#### 3.1.2. Opseg

Raspon opsega senzora odgovara minimalnim i maksimalnim radnim granicama za koje se
očekuje da će senzor točno izmjeriti. Na primjer, temperaturni senzor može imati normalne performanse
u radnom rasponu od -200 do +500 ºC.

#### 3.1.3. Tačnost

Tačnost se odnosi na razliku između prave vrijednosti i stvarne vrijednosti koju mjeri senzor.
Tačnost se obično izražava kao omjer između prethodne razlike i prave vrijednosti i određuje se kao
postotak čitanja u cijeloj skali. Imajmo na umu da istinska vrijednost treba biti praćena do primarnog
referentnog standarda

#### 3.1.4. Preciznost

Preciznost se odnosi na stupanj obnovljivosti mjerenja. Vrlo ponovljiva očitanja ukazuju na
visoku preciznost. Preciznost se ne smije brkati s tačnošću. Na primjer, mjerenja mogu biti vrlo precizna,
ali nisu nužno točna.

#### 3.1.5. Rezolucija

Kada se ulazna količina poveća s neke proizvoljne nulte vrijednosti, izlaz senzora se možda neće
promijeniti dok se ne prekorači određeni ulazni priraštaj. Sukladno tome, rezolucija je definirana kao
najmanja uočljiva promjena ulaza koja se može sa sigurnošću otkriti.

#### 3.1.6. Reproducibilnost

Reproducibilnost opisuje koliko su blizu mjerenja kada se isti unos mjeri više puta tijekom
vremena. Kad je raspon mjerenja mali, obnovljivost je velika. Na primjer, temperaturni senzor može se
obnoviti od 0,1 ° C za raspon mjerenja od 20 ° C do 80 ° C. Obratit treba pažnju da obnovljivost može
varirati ovisno o rasponu mjerenja. Drugim riječima, očitanja mogu biti vrlo ponovljiva u jednom
rasponu i manje ponovljiva u drugom radnom opsegu.

#### 3.1.7. Ofset

Offset se odnosi na izlaznu vrijednost kada je ulaz nula, kao što je prikazano na slici 4.

#### 3.1.8. Linearnost

Linearnost je mjera maksimalnog odstupanja bilo kojeg očitanja od ravne kalibracijske linije.
Obično se linearnost senzora izražava ili kao postotak stvarnog očitanja ili kao postotak čitanja u punoj
skali. Pretvaranje nepoznate količine u skalirani izlazno očitavanje pomoću senzora je najprikladnije
ako jednadžba umjeravanja ulaza i izlaza slijedi linearni odnos. To pojednostavljuje mjerenje, jer
možemo pomnožiti mjerenje bilo koje ulazne vrijednosti sa konstantnim faktorom, a ne pomoću „tablice
pretraživanja“ kako bismo pronašli različiti faktor množenja koji ovisi o ulaznoj količini kada
kalibracijska jednadžba slijedi nelinearnu jednačinu. Imajmo na umu da je ponekad poželjan linearni
odziv, ali moguća su i tačna mjerenja čak i ako je odziv nelinearan sve dok je odnos ulaza i izlaza u
potpunosti karakteriziran.


#### 3.1.9. Vrijeme odziva

Vrijeme odziva označava vrijeme koje je potrebno da senzor dosegne određeni postotak (npr. 95
posto) svoje konačne ustaljene vrijednosti kada se ulaz promijeni. Na primjer, može biti potrebno 20
sekundi da senzor temperature dosegne 95 posto svoje maksimalne vrijednosti kada se izmjeri promjena
temperature od 1 ºC. U idealnom slučaju, kratko vrijeme reakcije ukazuje na sposobnost senzora da brzo
reagira na promjene unosa.

#### 3.1.10. Pomak

Drift(Pomak) se odnosi na promjenu očitavanja senzora kada ulaz ostaje konstantan. Pomak se
može kvantificirati izvođenjem višestrukih testova kalibracije tijekom vremena i određivanjem
odgovarajućih promjena u presjeku i nagibu linije za umjeravanje. Ponekad odnos ulaza i izlaza može
varirati s vremenom ili može
ovisiti o drugoj neovisnoj
varijabli koja također može
promijeniti očitavanje izlaza.
To može dovesti do nulte (ili
offset) pomaka ili pomaka
osjetljivosti, kao što je
prikazano na slici 5. Da bi se
odredio nulti pomak, ulaz se
drži na nuli dok se bilježi
izlazno očitanje. Na primjer,
izlaz pretvarača tlaka može
ovisiti ne samo o tlaku već i
o temperaturi. Stoga
varijacije u temperaturi
mogu proizvesti promjene u
očitavanjima na izlazu, čak i ako ulazni tlak ostane nula. Pomicanje osjetljivosti može se utvrditi
mjerenjem promjena u izlaznim očitanjima za različite ne-nule konstantne ulaze. Na primjer, za
pretvarač pritiska, ponavljanjem mjerenja u raznim temperaturama, otkrit će se koliko nagib linije za
umjeravanje ulaza i izlaza varira od temperature. U praksi i nula i osjetljivost nanošenja određuju ukupnu
pogrešku uslijed pomaka. Znajući vrijednosti ovih odrona mogu pomoći u kompenzaciji i ispravljanju
očitanja senzora.

#### 3.1.11. Histereza

U nekim senzorima ulazna i izlazna karakteristika slijedi
različit nelinearni trend, ovisno o tome povećava li se ili
smanjuje ulazna količina, kao što je prikazano na slici 6. Na
primjer, određeni manometar može proizvesti drugačiji izlazni
napon kada ulazni tlak varira od nule do pune skale, a zatim se
vraća na nulu. Kad mjerenje nije savršeno reverzibilno, kaže se
da senzor pokazuje histerezu. Ako senzor pokazuje histerezu,
odnos ulaza i izlaza nije jedinstven, ali ovisi o promjeni smjera
u ulaznoj količini.

## greškama pomaka. Slika 5.Promjene ulaza u odnosu na izlazni odziv uzrokovane (a) greškama osjetljivosti i (b)

```
greškama osjetljivosti i (b) greškama pomaka.
```
## Slika 6.Ulaz u odnosu na izlazni odziv senzora sa histerezom.


### 3.2. Bioanalitički senzori

Svi živi organizmi posjeduju biološke senzore. Većina
prirodnih senzora su specijalizovane ćelije koje su osjetljive
na: svjetlo, pokret, temperaturu, magnetno polje, gravitaciju,
vlažnost, vibracije, pritisak, električno polje, zvuk, i druge
fizičke pojave iz okruženja. Drugi biološki senzori koji se
nazivaju unutrašnjim, jesu osjetljivi na istezanje, pokret
organizma i nesvjesni osjećaj pokreta i prostorne pozicije.

Neki od bianalitičkih senzora su:

- senzori koji reaguju na toksine, feromone
- metabolički senzori za nivo glukoze ili kisika
- signalne molekule: hormoni, neurotransmiteri i citokini
- senzori koji razlikuju proteine samog organizma i vanjske ili strane proteine.

Budući da bioanalitički senzori rade na pricipu mjerenja materijalnih tj fizičkih veličina, oni
spadaju u skupinu pretvorbenih uređaja. Oni putem procesa prepoznavanja određenog materijalnog
uzorka na molekularno-fizičkoj razini i senzora koji omogućava pretvaranje istog u signal, mogu nam
dati veoma korisne informacije. Biomedicinski senzori se sastoje od vece skupine uređaja koji mogu
biti hemijski, fizički ili neka druga vrsta senzora.

Hemijski senzor definiran je kao mjerni uređaj koji pretvara hemijsku informaciju o uzorku u
analitički mjerljiv signal. Hemijska informacija može doći od hemijske reakcije analita ili od fizikalnih
svojstava ispitivanog sustava. Hemijski senzor sastoji se od dvije osnovne jedinice: receptora i
pretvornika. Receptor je odgovoran za selektivno i osjetljivo prepoznavanje analita. U pretvorniku
hemijskog senzora energija oslobođena tijekom interakcije analita i receptora prevodi se u električni
signal koji je pogodan za mjerenje što
je vidljivo na Slici 7.

Biosenzori su također i
hemijski senzori, ali oni koriste samo
određene klase biološkog
prepoznavanja i pretvaranja.
Biosenzor se prema IUPAC-u
(International Union of Pure and
Applied Chemistry) definira kao
samostalan integrirani uređaj koji je
sposoban davati specifične
kvantitativne ili semikvantitativne
informacije koristeći biološki element
za prepoznavanje.

Čisti fizički senzor generiše i pretvara parametre koji ne zavise od hemijskih osobina ali rezultat
ovog senzora je način reagiranja na naboje ili neke druge vrste tačkasih massa. Sve ovo kada se zajedno
koristi u biološkim sistemima moze rezultirati bioanalitičkim senzorom bez obzira na fizičke, hemijske
ili biohemijske osobine.Oni proizvode analitički signal za biološki sistem za buduća razmatranja.

## Slika 7.Šematski prikaz hemiskog senzora

## Slika 8.Generički bioanalitički sensor


Postupak hemijskog prepoznavanja je fokusiran na molekularnoj razini hemijskih entiteta,

često hemijskih struktura. U novije vrijeme biološki procesi prepoznavanja su bolji za razumjeti, a
opći koncept priznavanja receptom ili kemoreceptorom postao je moda. Iako su to često velike

molekule vezane za ćelijske membrane, one sadrže specifične strukture koje omogućuju širok raspon
različitih načina molekularnog prepoznavanja, uključujući prepoznavanje velikih i malih vrsta. Dakle,

kemoreceptor se pojavljuje u literaturi senzora kao generički izraz za glavnu osobu koja radi
prepoznavanje. Biološko prepoznavanje u biosenzorima posebno naglašavala "receptore" i njihove

kategorije.

Povijesno, funkcijareceptora nije nužno značila izravno mjerenje veličine sa receptora.
Odnosno, postojale su određene hemijske reakcije i pretvorbe koje su se koristile prilikom mjerenja:
promjena pH vrijednosti, promjena otopljenog O 2 , stvaranje H 2 O 2 , promjene optičke asorpcije i
promjena temperature.Glavni receptori su enzimi zbog njihove izvanredne selektivnosti. Drugi receptori
mogu biti neke druge supstance biohemije kao na primjer antitijela, organele, mikrobi i dr.

Glavna razlika između enzima i antitijela je ta što se antitijela čvrsto vežu za antigene pri čemu
dolazi do stvaranja kompleksa. Također postoje receptori razine praćenja koji usmjeravaju mrave , kao
što su feromoni. Skica generičkog bioanalitičkog senzora je prikazana na Slici 8.

### 3.3. Biosenzori u praćenju okoliša

Biosenzori nalaze primjenu u različitim područjima,
od agrikulture, kontrole kvalitete
namirnica, u medicini, vojsci i kontroli različitih procesa u
okolišu. Za kontrolu i praćenje okoliša biosenzori mogu
pružiti brzu informaciju o mjestu zagađenja. Osim toga,
prednost biosenzora nad drugim analitičkim metodama jest i
u prenosivosti što znanstvenicima omogućava mjerenje
koncentracije polutanata, te u mogućnosti mjerenja bez
dodatnih priprema uzoraka. Također, uz određivanje
specifičnih spojeva mogu dati informaciju o njihovom
biološkom učinku (npr. toksičnost nekog spoja).

Najčešće korišteni biosenzori u praćenju okoliša su enzimski biosenzori, imunosenzori i
senzori sa specifičnim reporter genima.

#### 3.3.1. Enzimski biosenzori

Enzimi su najčešće korišteni biološki senzorski element u proizvodnji različitih biosenzora.
Enzimi čine skupinu od preko 2.000 proteina koji imaju takozvana biokatalizna svojstva. Ova svojstva
daju enzimima jedinstvenu i snažnu sposobnost ubrzavanja hemijskih reakcija unutar bioloških stanica.
Većina enzima reagira samo na specifične supstrate, iako se mogu nalaziti u kompliciranoj smjesi s
drugim tvarima. Važno je, međutim, imati na umu da su topljivi enzimi osjetljivi i na temperaturne i na
pH vrijednosti te da ih mogu inaktivirati mnogi kemijski inhibitori. Za praktične primjene biosenzora,
ti se enzimi normalno imobiliziraju nesolubiranjem slobodnih enzima ugradnjom u inertnu i stabilnu
matricu kao što su škrobni gel, silikonski kaučuk ili poliakrilamid. Taj je postupak važan kako bi se
osiguralo da enzim zadrži svoja katalitička svojstva i može ih se ponovo upotrijebiti.

## Slika 9.Biosenzori


Djelovanje specifičnih enzima može se upotrijebiti za izgradnju niza različitih biomedicinskih
senzora. Tipičan primjer enzima koji se temelji na enzimima je senzor glukoze koji koristi enzim
glukozidu oksidazu. Glukoza igra važnu ulogu u metaboličkim procesima. U bolesnika koji pate od
dijabetes melitusa, gušterača ne proizvodi dovoljne količine inzulina da bi na odgovarajući način
kontrolirao nivo glukoze u krvi. Stoga, za upravljanje bolešću, ovi pacijenti moraju redovito nadzirati i
regulirati razinu glukoze u krvi lijekovima i injekcijama inzulina. Trenutno dostupni senzori glukoze
temelje se na imobiliziranom enzimu, poput glukozida oksidaze, koji djeluje kao katalizator. Glukoza
se otkriva elektrokemijskim mjerenjem ili količine proizvedene glukonske kiseline ili vodikovog
peroksida (H2O2) ili mjerenjem količine potrošenog kisika u skladu sa sljedećim hemijskim reakcijama:

##### 퐺푙푢푐표푠푒+푂 2 + 퐻 2 푂

```
푔푙푢푐표푠푒 표푥푖푑푎푠푒
→ 푔푙푢푐표푛푖푐 푎푐푖푑+ 퐻 2 푂 2
```
Senzor glukoze sličan je senzoru pO2 i
prikazan je na slici 10. Glukoza i kisik ulaze kroz
vanjsku membranu kako bi glukoza omogućila
interakciju s enzimom glukoza oksidaza. Preostali
kisik prodire kroz drugu membranu propusnu za
kisik i mjeri se kisikovom elektrodom.

Senzori utemeljeni na biokatalizima obično se
sastoje od elektrokemijskog pretvarača osjetljivog na
plin ili ionsko selektivne elektrode s enzimom
imobiliziranim u ili na membrani koja služi kao
biološki posrednik. Analit difundira iz rastvorenog
uzorka u biokatalitički sloj, gdje se odvija enzimska
reakcija. Elektroaktivni proizvod koji nastaje (ili se
konzumira) obično se detektuje pomoću ionsko
selektivne elektrode. Membrana razdvaja osnovni
senzor od enzima ako se troši plin (kao što je O2) ili
stvara (kao što je CO2 ili NH3).

Iako je koncentracija osnovnog supstrata
kontinuirano u padu, potrošnja je obično
zanemariva. Smanjenje se otkriva samo kad je testni
volumen vrlo mali ili kada je površina enzimske membrane dovoljno velika. Stoga je ova
elektrokemijska analiza nerazorna, a uzorak se može ponovno upotrijebiti. Mjerenja se obično izvode
pri konstantnom pH i temperaturi bilo u otopini miješanog medija ili u otopini koja teče.

### 3.4. Senzori krvnih gasova

Mjerenja arterijskih plinova u krvi (pO2, pCO2 i pH) često se provode na kritično bolesnim
pacijentima u operacijskoj sali i na odjelu intenzivne njege. Liječnik ih koristi za podešavanje mehaničke
ventilacije ili za primjenu farmakoloških sredstava. Ova mjerenja daju informacije o respiratornim i
metaboličkim neravnotežama u tijelu i odražavaju adekvatnost oksigenacije krvi i eliminacije CO2.
Tradicionalno se provodi analiza plinova arterijske krvi izvlačenjem krvi iz periferne arterije.
Uzorak krvi se zatim transportira u klinički laboratorij na analizu. Potreba brzih rezultata ispitivanja u
liječenju nestabilnih, kritično bolesnih pacijenata dovela je do razvoja novijih metoda kontinuiranog
praćenja neinvazivnog plina u krvi. To omogućava liječniku da prati trendove u pacijentovom stanju
kao i da odmah dobije povratne informacije o adekvatnosti određenih terapijskih intervencija.
Neinvazivni senzori za mjerenje O2 i CO2 u arterijskoj krvi temelje se na otkriću da plinovi poput
O2 i CO2 mogu lako difundirati kroz kožu. Do difuzije dolazi zbog djelomične razlike tlaka između

## Slika 10. Princip rada senzora za glukozu.


krvi u površinskim slojevima kože i na vanjskoj površini kože. Ovaj koncept korišten je za razvoj dvije
vrste neinvazivnih elektrokemijskih senzora za transkutano nadgledanje pO2 i pCO2. Nadalje, otkriće
da krv mijenja boju ovisno o količini kisika kemijski vezanog na hemoglobin u eritrocitima dovelo je
do razvoja nekoliko optičkih metoda za mjerenje zasićenosti kisikom u krvi.

#### 3.4.1. Senzori za mjerenje kisika

Kvantitativna metoda za mjerenje oksigenacije u krvi je od velikog značaja za procjenu
krvožilnog i respiratornog stanja pacijenta. Kisik se prenosi krvlju iz pluća u tkiva u dva različita stanja.
U normalnim fiziološkim uvjetima, oko 2 posto ukupne količine kisika koju krv prenosi u vodi se otapa
u plazmi. Ta je količina linearno proporcionalna pO2 u krvi. Preostalih 98 posto nalazi se unutar
eritrocita u labavoj, reverzibilnoj hemijskoj kombinaciji s hemoglobinom (Hb) kao oksihemoglobinom
(HbO2). Dakle, postoje dvije mogućnosti za mjerenje oksigenacije krvi: upotrebom polarografskog
senzora pO2 ili mjerenjem zasićenosti kisikom (relativna količina HbO2 u krvi) pomoću optičkog
oksimetra. pO2 senzor, također poznat kao Clarkova elektroda, koristi se za mjerenje parcijalnog tlaka
plina O2 u uzorku zraka ili krvi.
Ovaj je senzor kategoriziran kao amperometrijski (tj. Mjerenje se temelji na proizvodnji struje
kada se napon primjenjuje između dvije elektrode) i zahtijeva vanjski polarizirajući izvor napona
pristranosti. Mjerenje se temelji na principu polarografije, kao što je prikazano na slici 11. Elektrode
koriste sposobnost molekula O2 da hemijski reagiraju s H20 u prisutnosti elektrona za proizvodnju
hidroksilnih (OH) iona. Ova elektrokemijska reakcija, koja se naziva oksidacija / redukcija ili redoks
reakcija, stvara malu struju i zahtijeva vanjski napon stalnog polarizirajućih napona od oko 0,6 V.

```
Kisik se smanjuje (troši) na površini katode od
plemenitog metala (npr. Platine ili zlata) (elektroda spojena
na negativnu stranu izvora napona) u skladu sa sljedećom
kemijskom reakcijom:
```
```
푂 2 + 2 퐻 2 푂+ 4 푒−
↔ 40 퐻−
```
```
U ovoj redukcijskoj reakciji, molekula O2 uzima četiri
elektrona i reagira s dvije molekule vode, stvarajući četiri
hidroksilna iona. Rezultirajući OH ioni migriraju i reagiraju s
referentnom Ag / AgCl anodom (elektroda spojena na
pozitivnu stranu izvora napona), uzrokujući reakciju
oksidacije u dva koraka koja slijedi:
```
```
퐴푔
⇔퐴푔++푒−
퐴푔++퐶푙−
↔퐴푔퐶푙
```
U ovoj reakciji oksidacije, srebro iz elektrode se
najprije oksidira u ione srebra, a elektroni se oslobađaju do
anode. Ti se srebrni ioni odmah kombiniraju s kloridnim ionima da nastanu srebrni klorid koji se taloži
na površini anode. Struja koja teče između anode i katode u vanjskom krugu nastalom ovom reakcijom
izravno je (tj. Linearno) proporcionalna broju molekula O2 koji se stalno smanjuju na površini katode.
Elektrode u polarografskoj ćeliji uronjene su u elektrolitsku otopinu kalijevog klorida i okružene su
teflonskom ili polipropilenskom membranom koja propušta O2 koja dopušta da se plinovi difundiraju
polako u elektrodu. Tako se mjerenjem promjene struje između katode i anode može utvrditi količina
kisika koji je otopljen u otopini. Uz prilično malu promjenu u konfiguraciji polarografskog pO2 senzora,
također je moguće mjeriti pO2 transkutano. Slika 12 ilustrira presjek Clarkovog tipa transkutanog pO
senzora. Ovaj je senzor u osnovi standardna polarografska pO2 elektroda koja je pričvršćena na površinu
kože dvostranom ljepljivom trakom. On mjeri parcijalni tlak kisika koji difundira iz krvi kroz kožu u

## Slika 11.Princip rada polarografskog Clarkovog tipa pO2.


Clarkovu elektrodu, slično načinu na koji mjeri pO2 u uzorku krvi. Međutim, budući da je difuzija O
kroz kožu normalno vrlo mala, u kućište ove elektrode ugrađena je minijaturna grijaća zavojnica koja
izaziva nježnu vazodilataciju (povećani lokalni protok krvi) kapilara u koži. Povećanjem lokalne
temperature kože na oko 43ºC, pO2 izmjeren transkutanim senzorom približava se vrijednosti ispod
arterijske krvi. Ova se elektroda intenzivno koristi u praćenju novorođenčadi na jedinici intenzivne
njege.
No, kako koža postaje gušća i
sazrijeva u odraslih pacijenata, svojstva
difuzije plina kože značajno se
mijenjaju i uzrokuju velike pogreške
koje rezultiraju nedosljednim
očitavanjem. Razvijene su različite
metode za mjerenje zasićenosti kisikom
SO2 (relativna količina kisika koju
hemoglobin nosi u eritrocitima), u
arterijskoj krvi (SaO2) ili mješovitoj
venskoj krvi (SvO2). , Ova metoda, koja
se naziva oksimetrija, temelji se na
svojstvima apsorpcije svjetlosti u krvi, a
posebno na relativnoj koncentraciji Hb i
HbO2, budući da je karakteristična boja
deoksigenirane krvi plava, dok krv s
potpuno kisikom ima izraženu svijetlo
crvenu boju.

Mjerenje se provodi na dvije specifične valne duljine: crvenu valnu duljinu, 휆1, gdje postoji
velika razlika u apsorpciji svjetlosti između Hb i HbO2 (npr. 660 nm) i druge valne dužine, 휆 2 , u bliskom
infracrvenom području spektar. Druga valna duljina može biti izobestična (područje spektra oko 805
nm, gdje su apsorbancije Hb i HbO2 jednake) ili oko 940–960 nm, gdje je apsorbancija Hb nešto manja
od one HbO2. Mjerenje se temelji na Beer-Lambertovom zakonu koji povezuje snagu odašiljene
svjetlosti, Pt, sa snagom upadajuće svjetlosti, P0, prema sljedećem odnosu:

푃푡= 푃 0 푥 [

```
푂퐷(휆 1 )
푂퐷(휆 2 )
```
]

gdje je 휆 konstanta ovisna o valnoj duljini koja se naziva koeficijent istiskivanja (ili molarna
apsorpcija) uzorka, b je duljina puta svjetlosti kroz uzorak, a c je koncentracija uzorka.
Pretpostavljajući za jednostavnost da (i) l1 ⁄4 660 nm i l2 1⁄4 805 nm (tj. Izobestični), (1)
hemolizirani uzorak krvi (krv u kojoj su eritrociti rupturirani - tj. Oslobađa se hemoglobin i jednoliko
pomiješana s plazmom) sastoji se od dvokomponentne smjese Hb i HbO2, i (2) ukupna apsorpcija
svjetlosti mješavinom ove dvije komponente je aditivna, može se izračunati jednostavan matematički
odnos za izračunavanje zasićenosti kisikom od krv:

푆푂 2 = 퐴−퐵 푥 [

푂퐷(휆 1 )

푂퐷(휆 2 )

]

pri čemu su A i B dva koeficijenta koji su funkcije specifične apsorptivnosti Hb i HbO2, OD (ili
apsorbancija) je definirana kao optička gustoća - to jest log10 (1 / T) - gdje T predstavlja prolazak
svjetlosti kroz uzorak i daje ga Pt / P0, a S02 je definiran kao cHB / (cHB-cHBO2).
Za mjerenje SO2 u krvi upotrebom benzo-oksimetra potreban je uzorak krvi, obično izvađen iz
periferne arterije. Uzorak se prenosi u optičku kivetu (stakleni spremnik s paralelnim zidom koji drži

## Slika 12. Transkutani senzor pO2.


uzorak), gdje se najprije hemolizira, a zatim osvjetljava uzastopno svjetlošću iz intenzivnog izvora bijele
boje, nakon pravilnog odabira valne duljine, koristeći uskopojasne optičke filtre.
SO2 se također može
mjeriti primjenom neinvazivnog
pulsnog oksimetra. Neinvazivni
optički senzori za mjerenje SaO
pulsnim oksimetrom sastoje se od
par malih i neprimjerenih dioda
koje emitiraju svjetlost (LED) -
tipično crvene (R) LED oko 660
nm i infracrveni (infracrveni) LED
oko 940–960 nm - i jedan, vrlo
osjetljivi silicijumski fotodetektor. Te se
komponente obično montiraju u obujmicu s
oprugom koja se može ponovo upotrijebiti ili na
ljepljivi omotač za jednokratnu upotrebu (slika
13).
Elektronski sklopovi unutar pulsnog
oksimetra generiraju digitalne prekidačke
signale za uključivanje i isključivanje dva LED-
a na uzastopni način i sinkrono mjerenje izlaza
fotodektora kada su uključene odgovarajuće
LED-diode. Senzor se obično pričvršćuje ili na
vrhovima prstiju ili na uhu, tako da se tkivo
probuši između izvora svjetlosti i fotodetektora.
Pulzna oksimetrija oslanja se na detekciju
fotopletizmografskog signala, kao što je
prikazano na slici 1 4.

#### 3.4.2. Ph Elektorde

pH opisuje ravnotežu između kiseline i
baze u otopini. Otopine kiselina imaju višak
vodikovih iona (Hþ), dok bazične otopine
imaju višak hidroksilnih iona (OH). U
razrijeđenoj otopini, produkt ovih
koncentracija iona je konstantan.
Stoga se koncentracija bilo kojeg iona
može upotrijebiti za izražavanje kiselosti ili
alkalnosti otopine. Sve neutralne otopine imaju
pH 7,0.Mjerenje pH krvi je temeljno za mnoge
dijagnostičke postupke.
U normalnoj krvi pH se održava pod
strogom kontrolom i obično je oko 7,40 (malo
bazičan). Mjerenjem pH krvi može se utvrditi
uklanjaju li pluća dovoljno CO2 iz tijela ili
koliko bubrezi dobro reguliraju acidobaznu
ravnotežu.pH elektrode pripadaju skupini
potenciometrijskih senzora (tj. elektrokemijskih senzora koji stvaraju napon). Ovi senzori stvaraju malu
razliku potencijala bez potrebe za polarizacijom elektrokemijske ćelije. PH elektroda se u osnovi sastoji
od dva odvojena elektroda: referentne elektrode i aktivne (indikatorske) elektrode, kao što je prikazano
na slici 1 5.
Dvije elektrode su obično izrađene od Ag / AgCl žice umočene u otopinu KCl i zatvorene u
staklenu posudu. Solni most, koji je u osnovi staklena cijev koja sadrži elektrolit zatvoren u membranu

## Slika 13. (a) pulsna sonda za pulsni oksimetar prsta i (b) jednokratni senzor prsta.

```
Slika 14 .Vremenska ovisnost apsorpcije svjetlosti
kroz sloj perifernog vaskularnog tkiva pokazuje
učinak arterijske pulsacije.
```

koja je propusna za sve ione, održava potencijal referentne elektrode u konstantnoj vrijednosti bez obzira
na otopinu koja se ispituje. Za razliku od referentne elektrode, aktivna elektroda je zapečaćena staklom
nepropusnim za vodik, osim na vrhu. Referentna elektroda se također može kombinirati s indikatorskom
elektrodom u jednom staklenom kućištu. Granica koja razdvaja dvije otopine ima potencijal
proporcionalan koncentraciji iona vodika u jednoj otopini i pri
konstantnoj temperaturi od 25ºC daje se:

푉=− 59 푚푉 푥 푙표푔 10 [퐻+]+퐶

```
gdje je C konstanta. Stim da je pH definisan sa:
```
푝퐻=− 푙표푔 10 [퐻+]

```
potencijal aktivne pH elektrode, V, proporcionalan je pH
otopine u ispitivanju i jednak je
```
푉= 59 푚푉 푥 푝퐻+퐶

Vrijednost C obično se nadoknađuje elektronskim
putem kad se pH elektroda kalibrira stavljanjem elektrode unutar
različitih puferskih otopina s poznatim pH vrijednostima.

#### 3.4.3. Senzori karbon dioksida

Elektrode za mjerenje parcijalnog tlaka CO2 u krvi
ili drugim tekućinama temelje se na mjerenju pH, kao što je
prikazano na slici 16. Mjerenje se temelji na opažanju da
kada se CO2 rastvara u vodi, on formira slabo disociranu
ugljičnu kiselinu (H2CO3) koja naknadno stvara slobodne
vodikove i bikarbonatne ione prema slijedećim kemijskim
reakcijama:

```
퐶푂 2 +퐻 2 푂
↔퐻 2 퐶푂 3
↔ 퐻++퐻퐶푂 3 −
```
Kao rezultat ove kemijske reakcije mijenja se pH otopine.
Ova promjena stvara potencijal između pH stakla i
referentne (npr., Ag / AgCl) elektrode proporcionalne
negativnom logaritmu pCO2.

## Slika 15.Princip rada pH elektrode...........................................................................................

## Slika 16. Princip rada pCO2 elektrode

```
elektrode
```

## 4. Optički senzori

Optički senzori igraju važnu ulogu u razvoju visoko osjetljivih i selektivnih metoda za
biohemijsku analizu. Temeljno načelo koje se koristi temelji se na promjeni optičkih svojstava biološkog
ili fizikalnog medija. Nastala promjena može biti rezultat fizičkih poremećaja ili unutarnjih promjena
apsorpcije, refleksije, raspršenja, fluorescencije, polarizacije ili indeksa loma biološkog medija.

### 4.1. Optička vlakna

Optička vlakna mogu se koristiti za prijenos svjetlosti s jedne
lokacije na drugu s minimalnim prigušenjem i bez ikakvog
transporta topline iz izvora svjetlosti. Zbog toga se koriste u
čitavom nizu minijaturnih senzora za biomedicinsku primjenu.
Optička vlakna su mala, fleksibilna i svojstvena imunitetu na
elektromagnetske i radiofrekvencijske smetnje. Oni mogu
proizvesti trenutni odgovor na suptilne promjene u
mikrookolima koje okružuju njihovu optičku površinu. Stoga
optička vlakna omogućavaju mjerenja u malim krvnim žilama
ili u osjetljivim tkivima kao što je mozak. Optička vlakna obično se izrađuju od dva koncentrična i
prozirna stakla ili plastike, kao što je prikazano na slici 17. Središnji komad poznat je kao jezgra, a
vanjski sloj, koji služi kao materijal za oblaganje, naziva se oblogom.

### 4.2. Senzorski mehanizmi

Optički senzori obično su povezani s
optičkim modulom, kao što je prikazano na
slici 1 8. Modul daje pobudnu svjetlost, koja
može biti iz monokromatskog izvora, poput
diodnog lasera, ili iz širokopojasnog izvora
(npr. Kvarc-halogen) koji je filtriran da
osigura usko propusno područje uzbuđenja.

Obično se koriste dvije valne duljine
svjetlosti:

- ona koja je osjetljiva na promjene u
    vrstama koje se mjere
- ona koja ne utječu na promjene
    koncentracije analita.

Ova valna duljina služi kao
referentna vrijednost i koristi se za
kompenzaciju fluktuacija u izlazu izvora i stabilnosti detektora. Izlaz svjetlosti iz optičkog modula
povezuje se u optički kabel pomoću odgovarajućih leća i optičkog konektora.

Nekoliko se optičkih tehnika obično koristi za osjetiti optičku promjenu na sučelju biosenzora.
Obično se temelje na evanescentnoj valnoj spektroskopiji, koja igra glavnu ulogu u optičkim senzorima
i principu površinske plazmonske rezonance.
U senzorima koji se temelje na fluorescenciji, upadno svjetlo pobuđuje emisiju fluorescencije
koja se mijenja u intenzitetu u zavisnosti od koncentracije analita koja se mjeri. Emitirana svjetlost

## Slika 17.Građa optičkog vlakna

## Slika 18.Princip senzora temelenog na optičkim vlaknima


putuje nazad niz vlakno do monitora, gdje se intenzitet svjetlosti mjeri fotodetektorom. U drugim
vrstama optičkih senzora, svojstva kemije senzora apsorbiraju svjetlost mijenjaju se u funkciji kemije
analita. U dizajnu temeljenom na apsorpciji obično se koristi reflektirajuća površina blizu vrha ili nešto
materijala za raspršivanje unutar same osjetljive kemije za vraćanje svjetlosti kroz isto optičko vlakno.

Ostali osjetilni mehanizmi iskorištavaju interakciju evanescentnog vala s molekulama koje su
prisutne unutar udaljenosti dubine penetracije i dovode do prigušenja refleksije koja se odnosi na
koncentraciju molekula. Zbog kratke dubine prodiranja i eksponencijalno opadajućeg intenziteta,
evanescentni val apsorbira spojeve koji moraju biti prisutni vrlo blizu površine. Princip je korišten za
karakterizaciju djelovanja između receptora koji su pričvršćeni na površinu i liganda koji su u otopini
iznad površine.

Ključna komponenta uspješne primjene vanjske valne spektroskopije je sučelje između površine
senzora i biološkog medija. Receptori moraju zadržati svoju prirodnu konformaciju i aktivnost vezanja,
a dovoljna mjesta vezanja moraju biti prisutna za više interakcija s analitom. U slučaju posebno slabih
apsorbujućih analita, osjetljivost se može poboljšati kombiniranjem principa evanescentnog vala s
višestrukim unutarnjim refleksijama duž bočnih dijelova neobojanog dijela vlakana optičkog vrha.
Alternativno, umjesto apsorbirajuće vrste, može se upotrijebiti i fluorofor. Svjetlost koju apsorbira
fluorofor emitira fluorescentnu svjetlost koja se može detektirati na većoj valnoj duljini, pružajući tako
bolju osjetljivost.

### 4.3. Imunološki senzori

Razvoj imunosensora temelji se na promatranju produkata reakcije koji vežu ligand između
ciljnog analita i visoko specifičnog veznog reagensa. Ključna komponenta imunosensora je element
biološkog prepoznavanja, koji se obično sastoji od antitijela ili fragmenata antitijela.
Imunološke tehnike nude izvanrednu selektivnost i osjetljivost kroz proces interakcije antitijelo-
antigen. Ovo je primarni mehanizam za prepoznavanje pomoću kojeg imunološki sustav otkriva i bori
se protiv stranih tvari, te je stoga omogućio mjerenje mnogih važnih spojeva u mikromolarnim, pa čak
i pikomolarnim koncentracijama u složenim biološkim uzorcima.
Imunološki biosenzori mogu se upotrijebiti u imunološkoj dijagnostici za otkrivanje vezanja
anti-tijela-antigena. Na slici 19 prikazan je konceptualni dijagram biosenzora imunološkog ispitivanja.

## Slika 19.Princip rada optickih imunoloških senzora


## 5. Fizička mjerenja

### 5.1. Transduktor protoka zraka........................................................................................

Jedan od najčešćih transduktora protoka zraka je Fleish pneumotachometer, prikazan na slici
20. Uređaj se sastoji od ravnog dijela s kratkom cijevi s fiksnom oprugom na sredini koji stvara blagi
pad tlaka dok zrak prolazi kroz cijev. Pad tlaka
stvoren preko zaslona mjeri se diferencijalnim
tlačnim pretvornikom. Signal koji proizvodi
transduktor tlaka proporcionalan je brzini
zraka. Cijev je obično oblikovana u stožac da
bi se stvorio laminarni oblik strujanja zraka.
Mali grijač zagrijava zaslon tako da se vodena
para ne kondenzira na njemu tijekom vremena
i stvara umjetno visoki pad tlaka.
Pneumotaometri tipa Fleish koriste se za
praćenje volumena, protoka i brzine disanja
pacijenata na mehaničkim ventilatorima.

### 5.2. Senzori za mjerenje temperature

Tjelesna temperatura jedna je od najstrože kontroliranih fizioloških varijabli i jedan od četiri
osnovna vitalna znaka koji se koriste u svakodnevnoj procjeni pacijentovog zdravlja. Unutarnja
temperatura (jezgre) u tijelu je nevjerojatno konstantna oko 37 ° C za zdravu osobu - i obično se održava
unutar ±0,5º C. Stoga je povišena tjelesna temperatura znak smetnje ili infekcije, dok značajan pad
temperature kože može biti klinička indikacija šoka.
Postoje dva različita područja u tijelu u kojima se temperatura rutinski mjeri: površina kože ispod pazuha
ili unutar tjelesne šupljine, poput usta ili rektuma. Postoji nekoliko senzora za mjerenje tjelesne
temperature.

#### 5.2.1. Termistori

Termistori su temperaturni senzori napravljeni
od komprimiranih sinterovanih oksida metala (poput
nikla, mangana ili kobalta) koji temperaturu
mijenjaju otpornost. Tržišno dostupni termistori se
kreću u obliku od malih kuglica do velikih diskova,
kao što je prikazano na slici 21. Matematički, otporno-temperaturna karakteristika termistora može biti
približno:

##### 푅푇= 푅푂 푥 푒푥푝[훽 푥(

##### 1

##### 푇

##### −

##### 1

##### 푇 0

##### )]

gdje je R0 otpor pri referentnoj temperaturi, T0 (u stupnjevima K), RT je otpor pri temperaturi, T (u
stupnjevima K), a je konstanta materijala, obično između 2.500 i 5.500 K.

## Slika 20.Fleish pretvarač zraka

## Slika 21.Uobičajeni oblici termistora


```
Tipična otporno - temperatura karakteristika
termistora prikazana je na slici 22. Imajmo na umu da
za razliku od metala i konvencionalnih otpornika koji
imaju koeficijent pozitivne temperature (kako
temperatura raste, otpor raste), termistori imaju
nelinearni odnos između temperature i otpora i
negativnog koeficijenta temperature. Povećanjem
temperature smanjuje se otpor termistora.
```
Termistorski senzor može se upotrijebiti u Swan-Ganz-
ovoj tehnologiji termodilucije za mjerenje srčanog
izlaza (volumen krvi koju srce izbacuje svake
minute) i za procjenu funkcije ventrikula. Postupak
se obično izvodi u operacijskoj sali ili jedinici intenzivne njege. To uključuje brzo bolusno ubrizgavanje
hladne indikatorske otopine, obično 3–5 ml sterilne fiziološke otopine ili otopine dekstroze koja se drži
na 0 ° C, u desnoj atrij, pomoću fleksibilnog katetera plućne arterije (slika 23 ).

Kateter termodilucije veličine 5 ili 7 sadrži mali balon i normalno se ubacuje u bedrenu ili
unutarnju jugularnu venu. Kateter je izrađen od radiopropusnog materijala koji omogućava jednostavnu
vizualizaciju rendgenskim strojem.
Sadrži tri priključka:

- balon za napuhavanje balona za
    usmjeravanje fleksibilnog vrha
    prema pravom mjestu
- proksimalni središnji venski luk
- udaljeni otvor plućne plućne
    arterije.

Nakon napuhavanja balona, vrh
fleksibilnog katetera prolazi se kroz
trikuspidalni ventil kroz desnu komoru,
kroz plućni ventil i u plućnu arteriju.
Proksimalni i distalni otvori mogu se
povezati sa pretvaračima pritiska koji
mjere krvni tlak unutar desne strane srca
dok je kateter napredan u desnoj arterij.

Nakon umetanja katetera, hladni
bolus ubrizgava se u desnu arteriju kroz
proksimalni lumen katetera. Otopina
bolusa miješa se s venskom krvlju u
desnom atriju i uzrokuje da se krv malo
ohladi. Ohlađenu krv izbacuje desni
ventrikularni kanal u plućnu arteriju, gdje
dodiruje termistor koji se nalazi u zidu
katetera u blizini njegovog udaljenog
vrha. Termistor mjeri promjenu krvne temperature dok krv prolazi u pluća.
Instrument izračunava srčani udio integrirajući promjenu u krvnoj temperaturi neposredno
nakon injekcije bolusa, koja je obrnuto proporcionalna srčanom ishodu.

## Slika 22. Otporno - temperaturna karakteristika tipičnog termistora

## Slika 23.Swan-Ganz-ov kateter sa termodilucijom.


#### 5.2.2. Bubni termometar

Nekontaktni termometri mjere temperaturu
ušnog kanala u blizini bubne opne, za koju se zna da
prati temperaturu jezgre za oko 0,5-1,0 ºC. U osnovi,
kao što je prikazano na slici 2 4 , infracrveno zračenje iz
bubne membrane usmjerava se na senzor osjetljiv na
toplinu kroz metalni valovod koji ima pozlaćenu
unutarnju površinu radi bolje reflektivnosti. Detektor,
koji je ili termopile ili piroelektrični senzor koji
pretvara toplinski tok u električnu struju, obično se
održava u okruženju s konstantnom temperaturom
kako bi se smanjile netočnosti zbog fluktuacije temperature okoline. Raspoloživi spekulum koristi se na
sondi za zaštitu pacijenata od unakrsne kontaminacije.

#### 5.2.3. Trenutni arterijski termometar..........................................................................

Neinvazivni termometar za skeniranje je Exergen
Corporation razvila kao alternativa bubnom termometru
za mjerenje tjelesne tjelesne temperature, u osnovi
eliminirajući nelagodu koju uzrokuje usta, uho ili
rektalni termometar (slika 2 5 ). Mjerenje se temelji na
skeniranju područja iznad privremene arterije pomoću
IR detektora sličnog senzoru koji se koristi u bubnom
termometru. Površna temporalna arterija proteže se
izravno od vanjske karotidne arterije i putuje ispred uha.
Analogno, leži otprilike 1 mm ispod kože, lako je
dostupan i održava dobru perfuziju krvi. Pod
pretpostavkom da u okoliš nema nuklearnog toplinskog
gubitka, površina kože iznad područja temporalne
arterije bila bi ista temperatura kao i arterijska krv u
aorti, koja je u osnovi jednaka tjelesnoj temperaturi
jezgre. Budući da je temperatura okoline normalno niža od tjelesne temperature jezgre, na površini kože
djeluje hlađenje zbog gubitka zračenja topline u okolni zrak. Da bi se uzele u obzir pogreške zbog
prirodnog gubitka topline, ručni skenirajući termometar mjeri temperaturu okoline, a istovremeno mjeri
apsolutnu temperaturu površine kože preko privremene arterije i izračunava arterijsku temperaturu
pomoću jednadžbe toplinske ravnoteže.

## Slika 24. Infracrveni termometar za uši bez kontakta.

## Slika 25.Trenutni arterijski termometar


## 6. EKG simulacija pomoću MATLAB-a

Cilj EKG simulatora je proizvesti tipične EKG valne oblike različitih vodova i što je
više moguće aritmija. Moj EKG simulator je simulator temeljen na matlabu i može proizvesti
normalan valni oblik EKG-a II. Uporaba simulatora ima brojne prednosti u simulaciji EKG
valnih oblika. Prvo je ušteda vremena, a drugo uklanjanje teškoća primanja stvarnih EKG
signala invazivnim i neinvazivnim metodama. EKG simulator omogućuje nam analizu i
proučavanje normalnih i nenormalnih EKG valnih oblika bez da stvarno koristimo EKG stroj.
Može se simulirati bilo koji zadani valni oblik EKG-om pomoću EKG simulatora.
Ovaj primjer je napravljen bez korištenja ulaza sa senzora u kodu, ali moguće su izmjene
na način da određene vrijednosti ključnih varijabli , koje mi unosimo ili koristimo default-ne u
ovom primjeru, unesemo preko očitanog senzora. Korišteni izračuni i ostali potrebni opisi
uključeni su u prilogu.

### 6.1. Značajne osobine valnog oblika EKG-a.

Tipično skalarno elektrokardiografsko olovo prikazano je na slici 26, gdje su značajne
karakteristike valnog oblika P, Q, R, S i T valovi, trajanje svakog vala i određeni vremenski
intervali kao što su PR, ST, i QT intervali.

```
Glavne osobine ovog simulatora:
```
- Može se postaviti bilo koja vrijednost
otkucaja srca
- Može se podesiti svaka vrijednost
intervala između vrhova (ex-PR interval)
- Svaka vrijednost amplitude može se
postaviti za svaki od vrhova
- Fibrilacija se može simulirati
- Buka zbog elektroda se može simulirati
- Srčani puls određenog oblika EKG vala
može se prikazati u zasebnom grafikonu
Ako promatramo sliku 26 , primijetit ćemo
da je jedno razdoblje EKG signala
mješavina oblika trokutastih i sinusoidnih
signala. Svaka značajna osobina EKG
signala može se predstaviti pomaknutom i smanjenom verzijom jednog od ovih valnih oblika.
EKG signal je periodičan, a osnovna frekvencija određena je otkucajem srca. Također

zadovoljava uvjete dirileta:

- Pojedinačna vrijednost i konačnost u zadanom intervalu
- Apsolutno integrabilno
- Konačni broj maksima i minima između konačnih intervala
- Ima ograničen broj diskontinuiteta

Furierove serije se koristie za predstavljanje EKG signala.

## Slika 26.EKG signal


### 6.2. Matlab kod

#### 6.2.1. main.m

1: x=0.01:0.01:2;
2: default=input('Press 1 if u want default ecg signal else press 2:\n');
3: if(default==1)
4: li=30/72;
5:
6: a_pwav=0.25;
7: d_pwav=0.09;
8: t_pwav=0.16;
9:
10: a_qwav=0.025;
11: d_qwav=0.066;
12: t_qwav=0.166;
13:
14: a_qrswav=1.6;
15: d_qrswav=0.11;
16:
17: a_swav=0.25;
18: d_swav=0.066;
19: t_swav=0.09;
20:
21: a_twav=0.35;
22: d_twav=0.142;
23: t_twav=0.2;
24:
25: a_uwav=0.035;
26: d_uwav=0.0476;
27: t_uwav=0.433;
28: else
29: rate=input('\n\nenter the heart beat rate :');
30: li=30/rate;
31:
32: %p wave specifications
33: fprintf('\n\np wave specifications\n');
34: d=input('Enter 1 for default specification else press 2: \n');
35: if(d==1)
36: a_pwav=0.25;
37: d_pwav=0.09;
38: t_pwav=0.16;
39: else
40: a_pwav=input('amplitude = ');
41: d_pwav=input('duration = ');
42: t_pwav=input('p-r interval = ');
43: d=0;
44: end
45:
46:
47: %q wave specifications
48: fprintf('\n\nq wave specifications\n');
49: d=input('Enter 1 for default specification else press 2: \n');
50: if(d==1)
51 : a_qwav=0.025;
52: d_qwav=0.066;
53: t_qwav=0.166;
54: else


55: a_qwav=input('amplitude = ');
56: d_qwav=input('duration = ');
57: t_qwav=0.166;
58: d=0;
59: end
60:
61:
62:
63: %qrs wave specifications
64: fprintf('\n\nqrs wave specifications\n');
65: d=input('Enter 1 for default specification else press 2: \n');
66: if(d==1)
67: a_qrswav=1.6;
68: d_qrswav=0.11;
69: else
7 0: a_qrswav=input('amplitude = ');
71: d_qrswav=input('duration = ');
72: d=0;
73: end
74:
75:
76:
77: %s wave specifications
78: fprintf('\n\ns wave specifications\n');
79: d=input('Enter 1 for default specification else press 2: \n');
80: if(d==1)
81: a_swav=0.25;
82: d_swav=0.066;
83: t_swav=0.09;
84: else
85: a_swav=input('amplitude = ');
86: d_swav=input('duration = ');
87: t_swav=0.09;
88: d=0;
89: end
90:
91:
92: %t wave specifications
93: fprintf('\n\nt wave specifications\n');
94: d=input('Enter 1 for default specification else press 2: \n');
95: if(d==1)
96: a_twav=0.35;
97: d_twav=0.142;
98: t_twav=0.2;
99: else
100: a_twav=input('amplitude = ');
101: d_twav=input('duration = ');
102: t_twav=input('s-t interval = ');
103: d=0;
104: end
105:
106:
107: %u wave specifications
108: fprintf('\n\nu wave specifications\n');
109: d=input('Enter 1 for default specification else press 2: \n');
110: if(d==1)
111: a_uwav=0.035;
112: d_uwav=0.0476;
113: t_uwav=0.433;


#### 6.2.2. p_wav.m

114: else
115: a_uwav=input('amplitude = ');
116: d_uwav=input('duration = ');
117: t_uwav=0.433;
118: d=0;
119: end
120:
121:
122:
123: end
124:
125: pwav=p_wav(x,a_pwav,d_pwav,t_pwav,li);
126:
127:
128: %qwav output
129: qwav=q_wav(x,a_qwav,d_qwav,t_qwav,li);
130:
131:
132: %qrswav output
133: qrswav=qrs_wav(x,a_qrswav,d_qrswav,li);
134:
135: %swav output
136: swav=s_wav(x,a_swav,d_swav,t_swav,li);
137:
138:
139: %twav output
140: twav=t_wav(x,a_twav,d_twav,t_twav,li);
141:
142:
143: %uwav output
144: uwav=u_wav(x,a_uwav,d_uwav,t_uwav,li);
145:
146: %ecg output
147: ecg=pwav+qrswav+twav+swav+qwav+uwav;
148: figure(1)
149: plot(x,ecg);

1: function [pwav]=p_wav(x,a_pwav,d_pwav,t_pwav,li)
2: l=li;
3: a=a_pwav;
4: x=x+t_pwav;
5: b=(2*l)/d_pwav;
6: n=100;
7: p1=1/l;
8: p2=0;
9: for i = 1:n
10: harm1=(((sin((pi/(2*b))*(b-(2*i))))/(b-
(2*i))+(sin((pi/(2*b))*(b+(2*i))))/(b+(2*i)))*(2/pi))*cos((i*pi*x)/l);
11: p2=p2+harm1;
12: end
13: pwav1=p1+p2;
14: pwav=a*pwav1;


#### 6.2.3. q_wav.m

#### 6.2.4. qrs_wav.m

#### 6.2.5. s_wav.m

1: function [qwav]=q_wav(x,a_qwav,d_qwav,t_qwav,li)
2: l=li;
3: x=x+t_qwav;
4: a=a_qwav;
5: b=(2*l)/d_qwav;
6: n=100;
7: q1=(a/(2*b))*(2-b);
8: q2=0;
9: for i = 1:n
10: harm5=(((2*b*a)/(i*i*pi*pi))*(1-cos((i*pi)/b)))*cos((i*pi*x)/l);
11: q2=q2+harm5;
12: end
13: qwav=-1*(q1+q2);

```
1: function [qrswav]=qrs_wav(x,a_qrswav,d_qrswav,li)
2: l=li;
3: a=a_qrswav;
4: b=(2*l)/d_qrswav;
5: n=100;
6: qrs1=(a/(2*b))*(2-b);
7: qrs2=0;
8: for i = 1:n
9: harm=(((2*b*a)/(i*i*pi*pi))*(1-cos((i*pi)/b)))*cos((i*pi*x)/l);
10: qrs2=qrs2+harm;
11: end
12: qrswav=qrs1+qrs2;
```
```
1: function [swav]=s_wav(x,a_swav,d_swav,t_swav,li)
2: l=li;
3: x=x-t_swav;
4: a=a_swav;
5: b=(2*l)/d_swav;
6: n=100;
7: s1=(a/(2*b))*(2-b);
8: s2=0;
9: for i = 1:n
10: harm3=(((2*b*a)/(i*i*pi*pi))*(1-cos((i*pi)/b)))*cos((i*pi*x)/l);
11: s2=s2+harm3;
12: end
13: swav=-1*(s1+s2);
```

#### 6.2.6. t_wav.m

#### 6.2.7. u_wav.m

1: function [twav]=t_wav(x,a_twav,d_twav,t_twav,li)
2: l=li;
3: a=a_twav;
4: x=x-t_twav-0.045;
5: b=(2*l)/d_twav;
6: n=100;
7: t1=1/l;
8: t2=0;
9: for i = 1:n
10: harm2=(((sin((pi/(2*b))*(b-(2*i))))/(b-
(2*i))+(sin((pi/(2*b))*(b+(2*i))))/(b+(2*i)))*(2/pi))*cos((i*pi*x)/l);
11: t2=t2+harm2;
12: end
13: twav1=t1+t2;
14: twav=a*twav1;

1: function [uwav]=u_wav(x,a_uwav,d_uwav,t_uwav,li)
2: l=li;
3: a=a_uwav
4: x=x-t_uwav;
5: b=(2*l)/d_uwav;
6: n=100;
7: u1=1/l
8: u2=0
9: for i = 1:n
10: harm4=(((sin((pi/(2*b))*(b-(2*i))))/(b-
(2*i))+(sin((pi/(2*b))*(b+(2*i))))/(b+(2*i)))*(2/pi))*cos((i*pi*x)/l);
11: u2=u2+harm4;
12: end
13: uwav1=u1+u2;
14: uwav=a*uwav1;

## Slika 27.Prikaz EKG signala nakon pokretanja skripte


## 7. Literatura

[1] https://hr.wikipedia.org/wiki/Senzori
[2] Infrared sensor
[3] Biosensor
[4] https://bit.ly/2QlBZ8M
[5] https://www.gme.cz/termistor-ptc-kty81- 110
[6] https://hrcak.srce.hr/file/222383
[7] https://bs.wikipedia.org/wiki/Opti%C4%8Dko_vlakno
[8] https://repozitorij.etfos.hr/islandora/object/etfos%3A1873/datastream/PDF/view
[9] https://en.wikipedia.org/wiki/Biosensor
[10] https://www.mathworks.com/matlabcentral/fileexchange/10858-ecg-simulation-using-matlab?s_tid=mwa_osa_a


