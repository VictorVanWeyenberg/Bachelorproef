# Is het nuttig om digitaal te gaan?

## Waarom niet Additive?

[Computer Music Journal: Multirate Additive Synthesis](https://www.mitpressjournals.org/doi/pdf/10.1162/014892699559625)

[Betere link](https://www.jstor.org/stable/3680619?read-now=1&seq=1#page_scan_tab_contents)

## Waarom niet Granular?

[Composing with Real-Time Granular Sound](https://www.jstor.org/stable/833014?seq=1#metadata_info_tab_contents)

@article{10.2307/833014, ISSN = {00316016}, URL = {<http://www.jstor.org/stable/833014}>, author = {Barry Truax}, journal = {Perspectives of New Music}, number = {2}, pages = {120--134}, publisher = {Perspectives of New Music}, title = {Composing with Real-Time Granular Sound}, volume = {28}, year = {1990} }

Het is van eigen al een techniek die enkel digitaal toegepast kan worden. Granular synthesis - samen met corpus-based granular synthesis - zijn recent de twee meest aantrekkelijke methodes voor sound synthesis. Let wel: het doelpubliek en de grootste aanhangers van deze methodes bevinden zich in de informatieve sector. De technieken zijn zeer bruikbaar voor geluidssimulaties en -imitaties. Sounddesigners kunnen de techniek gebruiken voor kleine sound effects in films of games. (Corpus-based granular) synthesis kan zelfs met AI toegepast worden.

Hoewel het een populaire techniek is in de informatieve sector, wil dat niet meteen zeggen dat het ook interessant is voor artiesten. Truax legt uit waarom.

### p. 123

Zegt dat hij een techniek gevonden heeft om real-time granular synthesis toe te passen. Voordelen van granular synthesis zijn dat het minder opslagruimte gebruikt en minder berekeningen maakt.

### p.124

Bespreekt [_Wings of Nike_](https://www.sfu.ca/~truax/nike.html), een muziekstuk dat ontstaan is uit granular snythesis.

### p.125

Bespreekt de mogelijkheden van granular synthesis en welke gevolgen ze hebben afhankelijk van hoe je ze toepast. Granulaire muziek kan met betere precizie bewerkt worden.

### p. 126

Granular maakt gebruik van een groot aantal events. Er zijn krachtige strategieën nodig vooraleer granular effectief wordt voor componisten. Stelt een hiërarchie voor van gegroepeerde controle parameters om verschillende aspecten van het geluid in één keer aan te passen. De groepen worden gebruikt m plotse veranderingen in het geluid teweeg te brengen. Dit kan een éénmalig event zijn of een sequentie van presets die een geanimeerd effect geven door de tijd heen. Deze groepen heten `presets`. Een sequentie van `presets` heet een `score` (partituur).

In tegenstelling tot discrete veranderingen zijn er ook continue. Hier stelt Truax `ramps` voor.

_Uitleg_ `masks`?

### p. 129

Truax becritiseert het traditionele Fourier geluidsmodel:

- Het houdt geen rekening met tijd. Het gaat ervan uit dat alle geluidsgolven oneindig lang duren. Beschouw het geluid van een instrument. Bij het aanslaan van een noot klinkt het geluid van het instrument anders dan wanneer het aangehouden of losgelaten wordt. De harmonieën van een geluid veranderen op die kleine tijdspanne.
- Ons gehoorsysteem werkt meer granulair dan "Fourier".

### p.131

Het is onmogelijk voor een componist om ieder event of grain specifiek te componeren. Daarom is de hiërarchische groepering van controle parameters essentieel.

### p. 132

(Laatste zin) Truax ziet geen toekomst in granular synthesis voor "mainstream computer musical development". Dit omdat het geen intuïtieve of gestandardiseerde manier van componeren is zonder al te veel muzikale kennis te hebben. Je kan zeggen dat niet granulaire systemen volledige dimensies van sounddesign negeren. Maar de vereiste voorkennis en het aantal te beïnvloeden parameters maakt granular synthesis een onaantrekkelijk systeem voor real-time componisten.

Er is ruimte voor ideeën en uitbreiding. Truax geeft in dezelfde paper een benadering van granular synthesis die de manier toegankelijker maakt voor real-time artiesten. Maar als er geen vraag naar is op de markt en het doelpubliek relatief klein is, is het ook onaantrekkelijk om toepasbare software voor te ontwikkelen.

## Waarom niet corpus-based granular?

Het is een beperking van Granular.

## Waarom niet met Wavelets?

[Synthesizing Sound Textures through Wavelet Tree Learning](http://musicweb.ucsd.edu/~sdubnov/Papers/CGA.pdf)

[A Wavelet Synthesis Technique for Creating Realistic Virtual Environment Sounds](https://www.mitpressjournals.org/doi/pdf/10.1162/105474602320935838)

[An Introduction to Wavelets](https://www.eecis.udel.edu/~amer/CISC651/IEEEwavelet.pdf)

Bij geluidsanalyse wordt bevoorkeurd om wavelet transforms te gebruiken omdat deze - in tegenstelling tot de Fourier transform - niet enkel het frequentie domein maar ook het tijdsdomein in kaart brengen.

Een simpel voorbeeld is dat de basis golven in subtractive synthesis als oneindig aanzien kunnen worden. Het heeft één periode die oneindig lang herhaald zal worden. Het geluid verandert van nature niet doorheen de tijd. Het heeft dus geen tijdsdomein.

Bij het aanslaan van een noot op eender welk instrument zal de intonatie en ambiance van het geluid anders klinken bij het aanslaan van de snaar dan een aantal milliseconden later wanneer het geluid uitdeint.

Wavelet geluidsanalyse gaat geluid proberen imiteren door basisbewerkingen uit te voeren op een "wavelet". Een wavelet is een kleine golf - zo'n tiental millliseconden lang - die aanzien wordt als één periode van een standaard geluidsgolf. De wavelet kan uitgerokken worden om de low-frequency karakteristieken van het originele geluid te benaderen en samengedrukt worden voor de high-frequency karakteristieken. Om aan te geven wanneer de kleinere wavelets zich voordoen in het tijdsdomein krijgt iedere wavelet een offset toegewezen relatief ten opzichte van het begin van de grootste wavelet ofwel mother wavelet. De schaling en offset van een wavelet zijn de twee coëfficiënten a.h.v. welke de wavelet transform een input geluid representeert in zowel het frequentie- als tijdsdomein.

Waar de wavelet transform een voordeel heeft in geluidsanalyse, kan niet hetzelfde gezegd worden over geluidsgeneratie of -verwerking. Na het correct kiezen van een mother wavelet zou men alle coëfficiënten handmatig correct moeten invullen tot men het gewenste geluid bekomt. Dit is zelfs minder efficiënt dan additieve geluidsgeneratie.
