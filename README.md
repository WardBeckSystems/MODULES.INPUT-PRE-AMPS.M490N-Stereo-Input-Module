# M490N Stereo Input Module · Input Pre Amps

Ward-Beck Systems M490N, 1985|18. Wiki page: [M490N on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M490N.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 37 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 12 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 6 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 314 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 1 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 12 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 48 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [3 topics](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1985 - M490N - P005 - 1-2.jpg](MANUALS/1985%20-%20M490N%20-%20P005%20-%201-2.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Ambient temperature** | degrees Celsius |
| **Dimensions** | 60&quot; wide 14.15&quot; high 6.50&quot; deep (41 Mm 360 Mm 165 mm / |
| **Weight** | (1.10 kg) net. |

## Circuit description

From [1985 - M490N - Stereo Input Module (2).pdf](MANUALS/1985%20-%20M490N%20-%20Stereo%20Input%20Module%20(2).pdf) pages 11-16 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

Input Selectors witches SWI and SW2 are mutually Interlock e dan d permit these lec t ion of One of two available Stereos our c es. Ana d d ition a l COntaCt i s supplied one ach switch for control purposes.

Two balanc.. dins er t points are provided, o n.. for each channel. following the Input Selectors.

The SA 14 -120 Sub assembly contains the I.. ft and r ighl chan n.. 1 pr.._ 1Impllf l e rs. The insert returns atP 2 pins 8 &amp; jan d P 2 pins 7 &amp;- H connect to the pr e amplifier inputs via 120 J1 pins 1 &amp; 2 and 120 J I pins 5 &amp; 6 forth e right and left channels respectively.

The p r e amplifier outputs appear a t 120 J2 pin I t forth e left channel and 120J2 pin 12 fort her ig h t channel. These outputs Connect to the s t e reoa ttenua tor ATTI.

UneQual input levels would be corrected by adjustment o f these n sit i v i ty trim controls R4 9 (right) lind R t l (left) located o nth e SA14_ 120 P r e amplifier Subassembl y. Them ix ing allen u a tor ATTl should be placed Int h e 15 d B &quot;i n hand &quot; posit ion to make thiS adjustment.

The Stereo all enua tor inputs as mentioned a bov&quot; are derived from the left and right channel p reamp l ifier located cn the 511.14_ 120 Su bassembly.

Program Chan n ei Switch

Ul (r ightl and U4 (left) are analog solids tate switCh e s, s ervin gas thea c t ives witching elements o f the Program channels. The control

voltage too p era te U1 and U4 is derived from the logic circuitry

within the module and is coupled to Ul and U4 via CRI and C R3. to switCh the channel ON, this control voltage is int h e order of

+10 volts. When the control voltage drops 10 0 volts, the s w i l c h will b e OFF, resulting ina signal all.. n u a t lon o f more than 100 dB.

**CIRCUI TOESCR IP T ION**

Follow ing U1 and U4, I h e sign 1!l1 i s 1!I mp lif ied b y in te g r &quot; led circuits U2. U3 (right) 1!I n d US, U6 (left) 10 &quot; nominal l., v., 1 o f 0 dSm (e q uiv_ 1!IIe n i voltage). The ~ i g nal i ~ I hen routed 10 lhe Program As si g nmenl s w il che s SW4 and SW5.

The left and rig hl c h &quot; n n e ls con ill in ie v elba lance con i r o is which are factory preSet to match l h e level of I he left c h&quot; n n e l tot her i g h t channel. These con i r o i. I'll ? (ri g h t) 1!I n d R54 (l e ft) should require n o fur the r adj u s l men ts.

Pro gram Outputs

The P Ian d P 2 Assignments w il c hes SW4 and SWS Si multan e ou sly assign b Ol h left and right channels 10 the P \ and / o r P2 P rog r &quot; m mixing buses.

The left and rig h l Cue channel circuits are located on the SA \ 4_ 120 P r e amplifier Su b&quot;s s e mb ly. Refer to Ihe SA14_120 cirCuit description ford e t&quot; i l.

The Cue outPuts &quot; p p e 1!lr ing &quot; t 120 J2 pins 4 &amp; 5 forth e left channel and 120 J2 pin ~ 9 &amp; 10 fort her i g h t channel feed through l heir esp e Clive summing resiS lo rs tot h emo au le cc o oecrc rPI.

Au x il i&quot; r y OUlp ut ~

The Auxiliary OUIP UIS are preceded b y the As si gnmenl s w il Ch SW7 and level con l r ol R2 9/R66. Prefade o r post fade 5e l&quot;&quot;, lion is made by ~w itch SW6. SW6, SW7 and R 29/ R66 control both left and right Auxiliary feeds Si multan eo u sly.

The con l r o l vol lages required to operate the left and right ~o lid

Slate program and Cues witches are generated with the aid of logiC

circuitry u t i liZ ing integrated circuits U7 t h rough UIO.

U8 is a CMOS dual f l i p_ flops ervin gas a latch to maintain the statUS of the switch e ~, once they have been s e l toe ither the ONo r

lhe OFF position.

A number o find i vidu ali noul fun clio n s govern the s taWs oft h e dual flip _ flop US. A description of each input fun Cl ion follows:

Initial Reset:

When power i sin i lially applied 10 I hes y s le m, the comb ina t_ ion of CRI2, CR I 3, CR14 and C 33 will pull down bO l h &quot;clea r&quot; inputs of US un l il C 33 is fully charged, thus ensuring I hat all solid S1a le sw i lche s are driven 10 l he OFF po si lion.

Channel On;

Momentary operation of Ih e Channel On s w i l c h SW9 will produce a neg alive going pulse a t US, pin 2 and &quot; pres e l &quot; Ih e As ect ion of US. All e r nat i v ei y, a momentary ground closure of the External Channel On con l ro lin p ul a t 1'2, pin N will res u ll i n Ihe same con di t ion.

Once the f l i p_f lop i s &quot;pres et&quot;, i l s o u tp u lat pin 15 changes from 0 to I (approx ima tel y +10 volts). This will cause Ih e left and right Programs w i lc hes 10 switch ON. Furthermore, 05 will sal u rate r e su lli ng in the Channel On ind ica lo r lamp OS3 to switch o n. Wilh 05 saturated, the &quot; control common &quot; p o ten l i ala p pears a t thee millers of 06 and 07, depending on whelhe r Input Selectors witch SWI Or SW2 is depressed. Effectively, 06 and 07 operate similar l y to two AND gales. The c o ilecto rs o f the two transistors represent the outputS of Ihe AND gates. They appear a t 1'2, pin 13 and P. These terminals are capable o f sink ing ama x im u m current o f 4 0 mA each from a 24 volts our ce and maybe used for muting purposes.

When operating the Channel On switch SW9, a sep ara te contact is closed, accessible a t 1'2, pins 15 and S. This contact maybe used for s i multan eo us &quot;m ach ines tart &quot;.

Pin R o f 1'2 isis ola ted through diode CR5. When connected in parallel with the same out pUI o f other modules, it

provides a con v e nie n l OR gale con fig u ration, suitable to

r e s e lII. Common timer each time a Channel On bullon is

depressed.

Channel Off;

Momenlary opera li&lt;&gt;&lt;&gt; of the Channel Olf sw,tch SW8 or momen lary ground closure of Ihe External Channel Off control input al P2, pin 12 will result ina negative going pulse at U8, pin 3 and &quot;clea r&quot; Ih e A-sec tion of U8, producing 0 v o ll sal US, pin IS. ConseQuently, the left and right solids tate Program switches wills witch OFF. a swills ree conducti&quot;'g. caus,,,,g OS3 to exlingulsh. and the muting control OUll)ut Sat P2. p l&quot;, s 13 and P will be di,....b.ed.

A separa le conlact is available cn SWB a&quot;,d is acce s sio lea l P2. pin 17 and U. II maybe used for &quot;maChine 1101)&quot;.

A separate Cha&quot;'nel Off lally la mo is built,nto SWS and is con &quot;,ec ted to P2, pi&quot;,s 18 and V.

In addll,on to the nol&quot;tl'lal !&gt;Usn bu llon O()era ted Channel Off funcllon, both lef land ri gh l solids tate Program swi lches are swi lche(1 oH wherlev er lhe m,,, i,,,g a ttenua lor Is MOved tot h e &quot;infi nite&quot; position and swi lch 5...,10 is closed. The 0 volt po terl iial c1evelooed a t U7, pin 10 is fed directly to the IWO programs witches and causes them to switch OFF. However, the status of US. the Channel On indicator and the mUl lng controls remain unaffected by Ihis ooeration.

The 8-sec lion of U8 is used to cco u-et Ih e solids tale Cue liwi lehes. The flip-flo p will changes tate eaCh time a negative going transi lion lakes place atp in 6 01 US. Conse QuM tly, with each In p ul pulse, the Cue channels willa l tern ate bet w&lt;!'en ON and OFF.

ThiS change of Stale Can be b rough l about by anyone 01 three different methods:

a) Momentary operation oft h e Cues witCh switCh SW12 t al.

b) Momentary g r o u...d closure oft h e Ex ter...a l Cue COntrOl

input a t P2. pin 11.

e) Operation of I h e &quot;overp r e s s&quot; switCh 5W l l, located a t the

slide erten uetorb eyond the &quot; infinite &quot; position.

The ON status oft he channels is indicated by 052,

which Is driven by 04.

WAR C - BECK SYSTEMS LTC.

M4 90N STEREO INPUT MODULE

Cue Off;

Ana d d itio n a l fe &quot; lure ensures that the Cue channels will &quot; Iw&quot; y s SWi lCh to OFF whenever the slide a tle nu a tor is moved onto o r away from the &quot;in finite &quot; position, regardless of their priors tate. The controls ig n a l for this action Is initial e d by the change of state o f Ih e Atl e n u &quot;t o r CUI switch SW10, There s ultanl level Change, being e i l her pos il ive or neg alive going, isp ro c e s s e d l h rough U?, U9, and UIO. The out p UI produced a l pin 4 of Ul0 willa l ways b e &quot; neg&quot; live going pulse o f approx ima tel y 500 mill is eco nds d uralion. CRll passes this pulse 10 U8, pin 8, Ihe reby &quot;c learing &quot; the BseClion oft he flip _ flop, andreS ul ting in pin 1 1of U8 to switch to (o r::~~:;esa~F FO. vol ts, int urn Switching the left and right Cue

logic control in pu ls are buffered 10 guard againSI spur iou s noise and switch bounce.

Power Supply Decoupl i n q

The &quot; Clive dec o u plin g n e l work consist ing of 09 Ihro ugh 0 12 along with their a ssoci al ed components, decou p leo r regulate I h ein coming +/_25 volts u p ply vol lag e down 10 +/ -20 volts. CR19 and C R20 serve 10 prevent amplifier damage int h e event o f supply voltage reversal. The dec o up l ing ne l work drops the +/ _2 5 volts u p ply rails 10 &quot; nominal voltage of +/ -20 volts. 08 dec o u p les and filters the 20 V positives u p ply rai i, res u i li ng ina n OUlp UI of +t2 volts too p era te Ih e C MOS c irc ui l ry.

U2, UJ, USa n d U6 are further dec ou pled to +/ -18 volts. Rl e, R1 9 and Cl 0 - C 13 dec o u ple Ihe +18 volts while RSS, R56 and C23 _ C 26 d ecou p lethe _ 18 volts. Separate o n-b oar d powers u p ply dec o u p l ing isp r ovid e don the SA14_ 120 Pre&quot;m pl ifie r Su basse mbly

WAR C · S E CI&lt; SYSTEMS LTC.

M490N STEREO INPUT MOOUlE

**MFG PART NUMBER**

Capac lto.-2.2 &quot;F/3 $ V

**0.' &quot; F/3 $V**

,_. l SSO/A HJ$/ l00

**T J9OC225MOJ$A5**

T39QA.l 0U40JS A5

**TJ9QA.1OSMOJSAS**

JJ &quot;F / 10 V T3 90[)3 ]6M0 1QAS

47 pF 47 pF 33 uF /lO V 33 uF /l0 V

Philips 2222-638-310479

COO 0.1 uF /lOO V Sp.. ague ICIOX7R 104MOS08

en 0.' uF /l00 V CO2 47 u F/ 40 V Philips

47 uF / 40 V 2.2 u F/3$ V 0.' uF / J$ V

**T390A I O4M(IJ5A$**

JJ uF /l0 V uF/3 S V TJ900J ]6MO tQAS

**T39OA1 05M0 35A5**

JJ uF / l 0 V TJ 900J J6M0 10.4S C&lt;9 47pF 2222-6 38_34 479

47 p F

33 uF / lO V JJ u F / 10 V

**,_. T3 9003]6M01QA S**

0.' uF/ l 00 V SP.... gu e lC to X7R 1Q4MOSOB

0. ' u F/ l 00 V 4 7 u F/4 0 V

C20 47 u F/4 0 V m 0.' u F/35 V Kernel T39OA104M 03 $AS

**C 20**

C29, u F / J$ V

, u F/ J5 V T390A 10 SMOJSAS

C 'O u F / JS V

4.7 u F/l0 V T39OB475MOIOA S

C&quot; uF /3$ V TJ9OA105 M035A 5

47 uF/ 2$ V TJ90E476 M02$A S ca 2.2 u F /35 V T39OC225 M035A S

</details>

<!-- /module data -->

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc2xFbXoxTmRWY1U/view?resourcekey=0-No1bV1J_YsGgm_xmTFma-w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc2xFbXoxTmRWY1U&resourcekey=0-No1bV1J_YsGgm_xmTFma-w" width="240" alt="1985 - M490N - 490-04-028 - STEREO INPUT MODULE MODULE LAYOUT.jpg"></a><br><sub>1985|18 · 490-04-028 - STEREO INPUT MODULE MODULE LAYOUT · <a href="MECHANICAL/1985%20-%20M490N%20-%20490-04-028%20-%20STEREO%20INPUT%20MODULE%20MODULE%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWENuX2xaUTJiM2M/view?resourcekey=0-xH0w15FDKKn7W5FP55AhfA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWENuX2xaUTJiM2M&resourcekey=0-xH0w15FDKKn7W5FP55AhfA" width="240" alt="1985 - M490N - 490-04-028.jpg"></a><br><sub>1985|18 · 490-04-028 · <a href="MECHANICAL/1985%20-%20M490N%20-%20490-04-028%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVU1Ob2Z2TEtxNlU/view?resourcekey=0-IewfUbiSpzThMwqZ2yQ87A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVU1Ob2Z2TEtxNlU&resourcekey=0-IewfUbiSpzThMwqZ2yQ87A" width="240" alt="1985 - M490N - 14-120-02-001 - COMMON COMMON SPEC IFIED LAST COMPONENT DESIGNA.jpg"></a><br><sub>1985|18 · 14-120-02-001 - COMMON COMMON SPEC IFIED LAST COMPONENT DESIGNA · <a href="SCHEMATICS/1985%20-%20M490N%20-%2014-120-02-001%20-%20COMMON%20COMMON%20SPEC%20IFIED%20LAST%20COMPONENT%20DESIGNA%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZEFTUmZuMFJad2M/view?resourcekey=0-t-HH1lFJtO4CTplL2a-x5Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZEFTUmZuMFJad2M&resourcekey=0-t-HH1lFJtO4CTplL2a-x5Q" width="240" alt="1985 - M490N - 14-120-02-001 - UNLESS OTHERWISE SPECIFIED IODES ARE.jpg"></a><br><sub>1985|18 · 14-120-02-001 - UNLESS OTHERWISE SPECIFIED IODES ARE · <a href="SCHEMATICS/1985%20-%20M490N%20-%2014-120-02-001%20-%20UNLESS%20OTHERWISE%20SPECIFIED%20IODES%20ARE%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNUhOOV9Bd1lDeDQ/view?resourcekey=0--1zxF3oahF9jIqiu_yT6ng" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNUhOOV9Bd1lDeDQ&resourcekey=0--1zxF3oahF9jIqiu_yT6ng" width="240" alt="1985 - M490N - 14-120-06-001 - STEREO PREAMPLIFIER COMPONENT LAYOUT.jpg"></a><br><sub>1985|18 · 14-120-06-001 - STEREO PREAMPLIFIER COMPONENT LAYOUT · <a href="SCHEMATICS/1985%20-%20M490N%20-%2014-120-06-001%20-%20STEREO%20PREAMPLIFIER%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVVROSnozWjFCcWs/view?resourcekey=0-OSAmNxCA669ViCIAxltHPA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVVROSnozWjFCcWs&resourcekey=0-OSAmNxCA669ViCIAxltHPA" width="240" alt="1985 - M490N - 490-01-014 - OFFX ON-START TIMER RESET OFF TALLY OFF.jpg"></a><br><sub>1985|18 · 490-01-014 - OFFX ON-START TIMER RESET OFF TALLY OFF · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-01-014%20-%20OFFX%20ON-START%20TIMER%20RESET%20OFF%20TALLY%20OFF%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc3hPZFBBLUEzMms/view?resourcekey=0-a636x9lBoKdbZ4v88Upe8Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc3hPZFBBLUEzMms&resourcekey=0-a636x9lBoKdbZ4v88Upe8Q" width="240" alt="1985 - M490N - 490-01-014 - STEREO INPUT MODULE FUNC TIONAL.jpg"></a><br><sub>1985|18 · 490-01-014 - STEREO INPUT MODULE FUNC TIONAL · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-01-014%20-%20STEREO%20INPUT%20MODULE%20FUNC%20TIONAL%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQ29QSVVxZDgwODg/view?resourcekey=0-qRh7SKVv19p3mtMEyEa1TA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQ29QSVVxZDgwODg&resourcekey=0-qRh7SKVv19p3mtMEyEa1TA" width="240" alt="1985 - M490N - 490-02-014 - STEREO INPUT MODULE SCHEMATIC.jpg"></a><br><sub>1985|18 · 490-02-014 - STEREO INPUT MODULE SCHEMATIC · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-02-014%20-%20STEREO%20INPUT%20MODULE%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdHFFUFktQVlIWFU/view?resourcekey=0-C5nSfTsdlAEvdqdi-Xnyzw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdHFFUFktQVlIWFU&resourcekey=0-C5nSfTsdlAEvdqdi-Xnyzw" width="240" alt="1985 - M490N - 490-02-014.jpg"></a><br><sub>1985|18 · 490-02-014 · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-02-014%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKajdWVWJsaEhWOUU/view?resourcekey=0-bjzu93t-gtRQQm5UtUBotA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKajdWVWJsaEhWOUU&resourcekey=0-bjzu93t-gtRQQm5UtUBotA" width="240" alt="1985 - M490N - 490-06-024 - AUX PRE-POST ON-OFF.jpg"></a><br><sub>1985|18 · 490-06-024 - AUX PRE-POST ON-OFF · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-06-024%20-%20AUX%20PRE-POST%20ON-OFF%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKME5VdnFwZmItZ1k/view?resourcekey=0-RNadAawNGym8frJdzkYD7w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKME5VdnFwZmItZ1k&resourcekey=0-RNadAawNGym8frJdzkYD7w" width="240" alt="1985 - M490N - 490-06-024 - STEREO INPUT MODULE COMPONENT LAYOUT.jpg"></a><br><sub>1985|18 · 490-06-024 - STEREO INPUT MODULE COMPONENT LAYOUT · <a href="SCHEMATICS/1985%20-%20M490N%20-%20490-06-024%20-%20STEREO%20INPUT%20MODULE%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

Not on Google Drive yet: `M490N - RTO-144 Connections.pdf`

## RTO-144 pinout

10 contacts (J2), 1 contacts (J3), 22 contacts (P1), 22 contacts (P2). Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|
| 1 |  | unread |  | low |
| 1 |  | unread |  | low |
| 1 | LEFT PGRM 1 | audio | A3 + | high |
| 1 | MIC IN A | in | A1 + | high |
| 2 | LEFT PGRM 1 | audio | A3 - | high |
| 3 | RIGHT PGRM 1 | audio | A4 + | high |
| 3 | MIC IN B | in | A2 + | high |
| 4 | RIGHT PGRM 1 | audio | A4 - | high |
| 6 | INSERT SEND | out | B1 + | high |
| 7 | INSERT RETURN | in | B2 + | high |
| 8 |  | unread |  | low |
| 10 |  | unread |  | low |
| 19 | -25 V | power |  | high |
| 20 | COMMON | ground |  | high |
| 21 | +25 V | power |  | high |
| 22 |  | unread |  | low |
| 22 |  | unread |  | low |
| A | MIC IN A | in | A1 - | high |
| C | MIC IN B | in | A2 - | high |
| F | INSERT SEND | out | B1 - | high |
| H | INSERT RETURN | in | B2 - | high |

**Straps:** Insert: JMP.6.7 · Insert: JMP.F.H

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNl83cWNOYTlYcWM/view?resourcekey=0-fcKQCewk9gSFjgZAU6V89Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNl83cWNOYTlYcWM&resourcekey=0-fcKQCewk9gSFjgZAU6V89Q" width="240" alt="1985 - M490N - P001 - Title Page.jpg"></a><br><sub>1985|18 · P001 - Title Page</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRGZxNlNEUDlZa2M/view?resourcekey=0-dbxQv8VrI8ESugJ00lNM5w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRGZxNlNEUDlZa2M&resourcekey=0-dbxQv8VrI8ESugJ00lNM5w" width="240" alt="1985 - M490N - P002.jpg"></a><br><sub>1985|18 · P002</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZERGT2Rtd0Q1OVU/view?resourcekey=0-UKUu1zhNYe-RbdABybaztg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZERGT2Rtd0Q1OVU&resourcekey=0-UKUu1zhNYe-RbdABybaztg" width="240" alt="1985 - M490N - P003.jpg"></a><br><sub>1985|18 · P003</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOG1kakszdkhZYUE/view?resourcekey=0-NvCrvn03uk1bvRTUgBEYgA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOG1kakszdkhZYUE&resourcekey=0-NvCrvn03uk1bvRTUgBEYgA" width="240" alt="1985 - M490N - P004 - 1-1.jpg"></a><br><sub>1985|18 · P004 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaDNBNzM0dkx1aUE/view?resourcekey=0-2JtV4DGXAnQrG3MVmQFAqQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaDNBNzM0dkx1aUE&resourcekey=0-2JtV4DGXAnQrG3MVmQFAqQ" width="240" alt="1985 - M490N - P005 - 1-2.jpg"></a><br><sub>1985|18 · P005 - 1-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMXY5T254V05YUzA/view?resourcekey=0-nyzTok0E1KXiZgTQYYt0Lg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMXY5T254V05YUzA&resourcekey=0-nyzTok0E1KXiZgTQYYt0Lg" width="240" alt="1985 - M490N - P006 - 2-1.jpg"></a><br><sub>1985|18 · P006 - 2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVWZZY1hrdmV6ODQ/view?resourcekey=0-mq_NAtnjqUItuUOgyGe3vA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVWZZY1hrdmV6ODQ&resourcekey=0-mq_NAtnjqUItuUOgyGe3vA" width="240" alt="1985 - M490N - P007 - 2-2.jpg"></a><br><sub>1985|18 · P007 - 2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSWxxT1p4bzhTeWc/view?resourcekey=0-RJ3rekd6Mmk05a7LjjrQXQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSWxxT1p4bzhTeWc&resourcekey=0-RJ3rekd6Mmk05a7LjjrQXQ" width="240" alt="1985 - M490N - P008 - 3-1.jpg"></a><br><sub>1985|18 · P008 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcEl4Q3JUQmlzeTg/view?resourcekey=0-T2AvR6teJbrSHt7juxpPdw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcEl4Q3JUQmlzeTg&resourcekey=0-T2AvR6teJbrSHt7juxpPdw" width="240" alt="1985 - M490N - P009 - 3-2.jpg"></a><br><sub>1985|18 · P009 - 3-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc1ZNTTcxVFFLbVE/view?resourcekey=0-JxkqgVPFuGLn7Blu2y07Zw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc1ZNTTcxVFFLbVE&resourcekey=0-JxkqgVPFuGLn7Blu2y07Zw" width="240" alt="1985 - M490N - P010 - 3-3.jpg"></a><br><sub>1985|18 · P010 - 3-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQU95V1N0d28xTU0/view?resourcekey=0-b8wCz3-9iKDIl-Qkm6LJuQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQU95V1N0d28xTU0&resourcekey=0-b8wCz3-9iKDIl-Qkm6LJuQ" width="240" alt="1985 - M490N - P011 - 4-1.jpg"></a><br><sub>1985|18 · P011 - 4-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSDcxX2RBczJfdkk/view?resourcekey=0-dt78KgLI3NOGh8WdI9krKQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSDcxX2RBczJfdkk&resourcekey=0-dt78KgLI3NOGh8WdI9krKQ" width="240" alt="1985 - M490N - P012 - 4-2.jpg"></a><br><sub>1985|18 · P012 - 4-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWjNTVVZzVTV5YTA/view?resourcekey=0-zSJEqTn9XBaetn8XwY7e3g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWjNTVVZzVTV5YTA&resourcekey=0-zSJEqTn9XBaetn8XwY7e3g" width="240" alt="1985 - M490N - P013 - 4-3.jpg"></a><br><sub>1985|18 · P013 - 4-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd1dyU254bEdlS1E/view?resourcekey=0-TIOUefMfbLth6xFtB8YEUA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd1dyU254bEdlS1E&resourcekey=0-TIOUefMfbLth6xFtB8YEUA" width="240" alt="1985 - M490N - P014 - 4-4.jpg"></a><br><sub>1985|18 · P014 - 4-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbF9hTng3OHY3ZHc/view?resourcekey=0-uQHQfAV75yR5LbImjEPAjw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbF9hTng3OHY3ZHc&resourcekey=0-uQHQfAV75yR5LbImjEPAjw" width="240" alt="1985 - M490N - P015 - 4-5.jpg"></a><br><sub>1985|18 · P015 - 4-5</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKR1IzWXQ1a0NYS2c/view?resourcekey=0-DG38F2HOoUqQc-o9dGIp4g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKR1IzWXQ1a0NYS2c&resourcekey=0-DG38F2HOoUqQc-o9dGIp4g" width="240" alt="1985 - M490N - P016 - 5-1.jpg"></a><br><sub>1985|18 · P016 - 5-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTEVWdnk2S0hnNXM/view?resourcekey=0-gYszTJyS2J-U5C30uzQ2bQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTEVWdnk2S0hnNXM&resourcekey=0-gYszTJyS2J-U5C30uzQ2bQ" width="240" alt="1985 - M490N - P017 - 5-2.jpg"></a><br><sub>1985|18 · P017 - 5-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUmZOSGR1UVpyelk/view?resourcekey=0-HtPML3SKrWVk_MIp6C126g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUmZOSGR1UVpyelk&resourcekey=0-HtPML3SKrWVk_MIp6C126g" width="240" alt="1985 - M490N - P018 - 5-3.jpg"></a><br><sub>1985|18 · P018 - 5-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZW9tdW9ud1FtdnM/view?resourcekey=0-rpCvuxcUG2rqqZkrMUHlbg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZW9tdW9ud1FtdnM&resourcekey=0-rpCvuxcUG2rqqZkrMUHlbg" width="240" alt="1985 - M490N - P019 - 5-4.jpg"></a><br><sub>1985|18 · P019 - 5-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKU0Rtdk9MXzRHY00/view?resourcekey=0-nvHBkGEDKRGszBtiHERJVA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKU0Rtdk9MXzRHY00&resourcekey=0-nvHBkGEDKRGszBtiHERJVA" width="240" alt="1985 - M490N - P020 - 5-5.jpg"></a><br><sub>1985|18 · P020 - 5-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRjdSbWZSLUVRX2s/view?resourcekey=0-wx0vmKPs0A7R0yiphGcROQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRjdSbWZSLUVRX2s&resourcekey=0-wx0vmKPs0A7R0yiphGcROQ" width="240" alt="1985 - M490N - P021 - 5-6.jpg"></a><br><sub>1985|18 · P021 - 5-6</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVFJ3M0YwUTl4RGc/view?resourcekey=0-PG13o0tGtYKMyxWRes2wIg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVFJ3M0YwUTl4RGc&resourcekey=0-PG13o0tGtYKMyxWRes2wIg" width="240" alt="1985 - M490N - P022 - 5-7.jpg"></a><br><sub>1985|18 · P022 - 5-7</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ0t0cjk0ZHZ1cHc/view?resourcekey=0-R4UZ19TyMmOLwXmhAwJweg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ0t0cjk0ZHZ1cHc&resourcekey=0-R4UZ19TyMmOLwXmhAwJweg" width="240" alt="1985 - M490N - P023 - 5-8.jpg"></a><br><sub>1985|18 · P023 - 5-8</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWGdpOEdyYnhaZFE/view?resourcekey=0-9nzXyJbpZzRlF1gj9cPdyw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWGdpOEdyYnhaZFE&resourcekey=0-9nzXyJbpZzRlF1gj9cPdyw" width="240" alt="1985 - M490N - P024 - 6-1.jpg"></a><br><sub>1985|18 · P024 - 6-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWVZQaVo1Z3V0eXM/view?resourcekey=0-LN8CDrnK3Uq8b1IHTpY7sw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWVZQaVo1Z3V0eXM&resourcekey=0-LN8CDrnK3Uq8b1IHTpY7sw" width="240" alt="1985 - M490N - P025 - 6-2.jpg"></a><br><sub>1985|18 · P025 - 6-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWDJPekgxUDczUFk/view?resourcekey=0-UdIaOBLw-ScIfqjSve3ngg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWDJPekgxUDczUFk&resourcekey=0-UdIaOBLw-ScIfqjSve3ngg" width="240" alt="1985 - M490N - P030.jpg"></a><br><sub>1985|18 · P030</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRDBwRGlTNm93SGM/view?resourcekey=0-6PtBYZU6Znqxv1anlgw6Xg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRDBwRGlTNm93SGM&resourcekey=0-6PtBYZU6Znqxv1anlgw6Xg" width="240" alt="1985 - M490N - P032 - SA14-120 - 1-1.jpg"></a><br><sub>1985|18 · P032 - SA14-120 - 1-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbFJ5QjNZYV9CWE0/view?resourcekey=0-Qv4hAZuU7caEmnEP8H4dTg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbFJ5QjNZYV9CWE0&resourcekey=0-Qv4hAZuU7caEmnEP8H4dTg" width="240" alt="1985 - M490N - P033 - SA14-120 - 1-2.jpg"></a><br><sub>1985|18 · P033 - SA14-120 - 1-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcXU1MG4zWjNKMms/view?resourcekey=0-gfkAxzVpWQG0XsaAfS9oXQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcXU1MG4zWjNKMms&resourcekey=0-gfkAxzVpWQG0XsaAfS9oXQ" width="240" alt="1985 - M490N - P034 - SA14-120 - 2-1.jpg"></a><br><sub>1985|18 · P034 - SA14-120 - 2-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRE1oNDhjVVhHcFU/view?resourcekey=0-CSKUXJjOIRZIj8mPJAHRZw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRE1oNDhjVVhHcFU&resourcekey=0-CSKUXJjOIRZIj8mPJAHRZw" width="240" alt="1985 - M490N - P035 - SA14-120 - 2-2.jpg"></a><br><sub>1985|18 · P035 - SA14-120 - 2-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYjdTTnp3QldudDg/view?resourcekey=0-K5HLVI3wq4dy3PN7834Xlg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYjdTTnp3QldudDg&resourcekey=0-K5HLVI3wq4dy3PN7834Xlg" width="240" alt="1985 - M490N - P036 - SA14-120 - 2-3.jpg"></a><br><sub>1985|18 · P036 - SA14-120 - 2-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdGdrcV9BREZJeGM/view?resourcekey=0-OjZfzS3tXbbODizjir5Ymg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdGdrcV9BREZJeGM&resourcekey=0-OjZfzS3tXbbODizjir5Ymg" width="240" alt="1985 - M490N - P037 - SA14-120 - 2-4.jpg"></a><br><sub>1985|18 · P037 - SA14-120 - 2-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdkZOYkhKM2M0R0U/view?resourcekey=0-N74H_z2508zyve58O4GZOw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdkZOYkhKM2M0R0U&resourcekey=0-N74H_z2508zyve58O4GZOw" width="240" alt="1985 - M490N - P038 - SA14-120 - 2-5.jpg"></a><br><sub>1985|18 · P038 - SA14-120 - 2-5</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVjhOZnphcHlBOFk/view?resourcekey=0-MQXO_BAX7uiXRzAukoQFJw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVjhOZnphcHlBOFk&resourcekey=0-MQXO_BAX7uiXRzAukoQFJw" width="240" alt="1985 - M490N - P039 - SA14-120 - 2-6.jpg"></a><br><sub>1985|18 · P039 - SA14-120 - 2-6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMFM4UWV3UG9zRU0/view?resourcekey=0-Izw-YHGjNzUpNvluxf81_w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMFM4UWV3UG9zRU0&resourcekey=0-Izw-YHGjNzUpNvluxf81_w" width="240" alt="1985 - M490N - Stereo Input Module (2).pdf"></a><br><sub>1985|18 · Stereo Input Module (2)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdWpWeDR5dFZFdnc/view?resourcekey=0-fVx2oI6XclcjgrEd0YFQhg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdWpWeDR5dFZFdnc&resourcekey=0-fVx2oI6XclcjgrEd0YFQhg" width="240" alt="1985 - M490N - Stereo Input Module.pdf"></a><br><sub>1985|18 · Stereo Input Module</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRUJZaWc0OW9YeTA/view?resourcekey=0-Bx_vdNKCfzsJEWKWECrRGg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRUJZaWc0OW9YeTA&resourcekey=0-Bx_vdNKCfzsJEWKWECrRGg" width="240" alt="1988 - M490N - P031 - SA14-120.jpg"></a><br><sub>1988|21 · P031 - SA14-120</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1985 - M490N - 14-120-02-001 - COMMON COMMON SPEC IFIED LAST COMPONENT DESIGNA.kicad_sch](KICAD/1985%20-%20M490N%20-%2014-120-02-001%20-%20COMMON%20COMMON%20SPEC%20IFIED%20LAST%20COMPONENT%20DESIGNA.kicad_sch)
- [1985 - M490N - 14-120-02-001 - UNLESS OTHERWISE SPECIFIED IODES ARE.kicad_sch](KICAD/1985%20-%20M490N%20-%2014-120-02-001%20-%20UNLESS%20OTHERWISE%20SPECIFIED%20IODES%20ARE.kicad_sch)
- [1985 - M490N - 490-01-014 - OFFX ON-START TIMER RESET OFF TALLY OFF.kicad_sch](KICAD/1985%20-%20M490N%20-%20490-01-014%20-%20OFFX%20ON-START%20TIMER%20RESET%20OFF%20TALLY%20OFF.kicad_sch)
- [1985 - M490N - 490-01-014 - STEREO INPUT MODULE FUNC TIONAL.kicad_sch](KICAD/1985%20-%20M490N%20-%20490-01-014%20-%20STEREO%20INPUT%20MODULE%20FUNC%20TIONAL.kicad_sch)
- [1985 - M490N - 490-02-014 - STEREO INPUT MODULE SCHEMATIC.kicad_sch](KICAD/1985%20-%20M490N%20-%20490-02-014%20-%20STEREO%20INPUT%20MODULE%20SCHEMATIC.kicad_sch)
- [1985 - M490N - 490-02-014.kicad_sch](KICAD/1985%20-%20M490N%20-%20490-02-014.kicad_sch)
- [1985 - M490N - Stereo Input Module (2) p45.kicad_sch](KICAD/1985%20-%20M490N%20-%20Stereo%20Input%20Module%20(2)%20p45.kicad_sch)
- [1985 - M490N - Stereo Input Module p29.kicad_sch](KICAD/1985%20-%20M490N%20-%20Stereo%20Input%20Module%20p29.kicad_sch)
- [1985 - M490N - Stereo Input Module p31.kicad_sch](KICAD/1985%20-%20M490N%20-%20Stereo%20Input%20Module%20p31.kicad_sch)
- [1985 - M490N - Stereo Input Module p45.kicad_sch](KICAD/1985%20-%20M490N%20-%20Stereo%20Input%20Module%20p45.kicad_sch)
- [M490N.kicad_sym](KICAD/M490N.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
