# Python Installatie
Voor je aan de slag kan gaan met een programmeertaal is dien je deze eerst *te installeren*.
Dit houdt in dat je één of meerdere stukken software op je computer installeert welke je toelaten programma's te schrijven en uit te voeren. Meestal omvat dit minimaal een compiler of interpreter, deze vertaalt de *commando's* die je schreef in een programma dat door een computer uitgevoerd kan worden. Daarnaast kan dit ook specifieke bibliotheken bevatten, welke door anderen geschreven programma onderdelen bevatten, een debugger welke je helpt met het opsporen van fouten in je programma en misschien zelfs een IDE (Integrated Development Environment) waarin alles samengebracht is.

In het geval van Python is het gelukkig ook mogelijk zonder zelf maar iets te installeren aan de slag te gaan. Op deze pagina krijg je een korte beschrijving hoe dit in zijn werk gaat, evenals een beschrijving hoe je toch zelf een Python omgeving op je eigen computer kan installeren. Voor deze tutorials is dit laatste echter niet nodig. Dit deel is toegevoegd voor de volledigheid, en kan gebruikt worden door hen die daar wel interesse of nood aan zouden hebben.

## Inhoud
1. [Python zonder lokale installatie](#noinstall)  
   1.1. [Google Colaboratory](#colab)  
   1.2. [Andere cloud/web services](#webservice)  
2. [Python met lokale installatie](#install)  
   2.1. [Anaconda](#anaconda)  
   2.2. [MiniConda](#miniconda)  
   2.3. [VSCode](#vscode)  
<!-- Links are a bit tricky, local links go through anchors: HTML-A-tags. However, to work the "name" variable should be all non-caps -->
<!-- add 2 blank spaces at the end of a line to get a linebreak or use < br/> or add empty line -->

##  <a name='noinstall'> </a> 1. Python zonder lokale installatie  

###  <a name='colab'> </a> 1.1. Google Colaboratory
Binnen deze tutorial-reeks zullen we Python leren kennen aan de hand van Jupyter Notebooks. Deze notebooks kun je lokaal uitvoeren indien je Python op je computer installeert, maar ook als zogenaamde **_Google Colaboratory_** documenten op de google drive van je google account. Dit kan op zeer eenvoudige wijze: 

1. Open je **google drive** in een web browser.
2. Klik op **New** (Links boven)&rarr; **More** &rarr; **Google Colaboratory**
3. **!!** Indien je hierboven geen Google Colaboratory ziet verschijnen, dan betekent dit dat je deze *app* nog dient toe te voegen. Dit kan als volgt:

   1. **New** &rarr; **More** &rarr; **Connect more apps**
   2. Zoek **Google Colaboratory**
   3. Selecteer **Colaboratory** (Oranje symbool)
   4. Installeer (Install).
   5. Na de installatie kun je puntje *2* hierboven uitvoeren.

4. Er wordt nu een nieuw document aangemaakt met de naam **Untitled0.ipynb**. Hierin kun je aan de slag gaan indien je zelf een nieuw notebook wil aanmaken. Je kan echter ook een bestaand notebook openen (zie puntje *5* hieronder)
5. **Inladen van een Tutorial-notebook**. Naast het aanmaken van eigen notebooks is het ook eenvoudig om een notebook in te laden van een andere locatie. Je kan de tutorials van deze reeks, welke op **Github** te vinden zijn, eenvoudig rechtstreeks inladen.

   1. In je Colaboratory document, klik op **File** &rarr; **Open Notebook**.<br/>
   2. In het pop-up venster selecteer je **GitHub**<br/>
   3. **!!** Er zal nog een extra pop-up venster verschijnen dat vraagt om in te loggen in je Github account. Dit is een neveneffect van het aangevinkt staan van de optie **Include private repos**. Je kan deze optie afvinken en het inlog venster zonder verder gevolg sluiten.
   4. Om de notebooks van deze tutorial te vinden kun je in de **zoekoptie** volgende tekst invoeren: *DannyVanpoucke/PythonTutorials*
   5. Je krijgt nu enkele tutorials om uit te kiezen. Klik op het Jupyter notebook in de lijst dat je wenst te openen (*e.g.* **01_IntroPython.ipynb** )
   6. Zoals je in de adresbalk kan zien is het notebook nog steeds in de GitHub repository gelokaliseerd, wat betekent dat je deze niet zal kunnen opslaan (tenzij het een notebook in een eigen GitHub repository is. *Sla daarom het notebook op in je drive door* **Copy to Drive** *te klikken.*
   7. Je kan nu in de kopie aan de slag gaan en deze naar eigen noden en goeddunken aanpassen.


###  <a name='webservice'> </a> 1.2. Andere cloud/web services
De populariteit van Python heeft ervoor gezorgd dat er dat er ook verschillende webservices beschikbaar zijn waar je als gebruiker Python code kan ontwikkelen en testen, zonder zelf iets te moeten installeren. Enkele voorbeelden (zonder aanbeveling) kun je hieronder vinden:
   1. [PythonAnywhere](https://www.pythonanywhere.com/)
   2. [repl.it](https://replit.com/)


##  <a name='install'> </a> 2. Python met lokale installatie
Afhankelijk van je besturingssysteem (Windows, Mac or Linux) en de persoonlijke wensen, kan de installatie van een programmeeromgeving voor Python eenvoudiger of complexer zijn. Er bestaan verschillende omgevingen en IDE's elk met hun voor en nadelen. 

###  <a name='anaconda'> </a> 2.1. Anaconda
De anaconda omgeving geeft je toegang tot een uitgebreid aantal tools welke je kan gebruiken bij het ontwikkelen van Python scripts. Er is een *commandline* omgeving om efficiënt nieuwe bibliotheken te installeren of te upgraden (maar dit kan ook via de GUI). De Spyder-tool is een simpele IDE waarin je zowel python rechtstreeks kan uitvoeren als scripts kan schrijven. De Jupyter notebook tool laat je toe lokaal Jupyter notebooks te creëren en uit te voeren.

De installatie instructies voor verschillende besturingssystemen kun je terugvinden in de [online handleiding](https://docs.anaconda.com/anaconda/install/index.html). In het geval van een Windows systeem kun je als volgt te werk gaan:

1. **Download Anaconda** [Installer](https://www.anaconda.com/products/distribution). Deze *installer* is vrij groot (>600Mb), dus dat kan even duren.
2. **Voer de Anaconda-Installer uit**
   - **!! OPLETTEN !!** Installeer *enkel voor jezelf* en **niet voor _alle_ _gebruikers_** gezien dit laatste problemen kan geven met permissies (*i.e.* toegankelijkheid van bestanden)
   - **!! OPLETTEN !!** Installeer op een plaats waar je voldoende ruimte hebt (5-10Gb minimaal) gezien een python installatie snel in grootte kan groeien met het toevoegen van *packages* en *environments*.
   - **!! OPLETTEN !!** Vermijd installaties op **OneDrive**,**GoogleDrive**,... en andere van dergelijke virtuele drives (ook als is dit waar je *default* gebruiksinformatie terechtkomt. Installatie op dergelijke drives geeft over het algemeen problemen met toegankelijkheid.
3. **Installatie van Jupyter notebooks**
   1. Start de **Anaconda navigator** (groene cirkelvormige icoon).
   2. Update de navigator indien gevraagd, en herstart na de update.
   3. Check of **Jupyter notebooks** geïnstalleerd zijn. Indien niet: Installeer en sluit de navigator af na afloop van de installatie.
   4. Persoonlijk ben ik niet zo een fan van het idee dat alle bestanden van een gebruiker in de *user/documents* map terecht moeten komen. Omdat Jupyter notebooks de map waarin het programma opent beschouwen als de *root*-map, is het niet mogelijk naar een hoger liggende map te gaan of bestanden in een parallelle map te openen. Om dit feature te omzeilen en Jupyter notebooks in een root-map van je keuze te openen ga je als volgt te werk:
      1.  Ga naar de map met de **snelkoppeling naar Jupyter notebook**.
      2.  Klik rechts op de snelkoppeling en kies **properties** (eigenschappen)
      3. Pas de **Start in** locatie aan naar de map van je keuze. (*e.g.* D:\ )
      4.  **Verwijder** het *%USERPROFILE%* in het **Target** veld.
      5.   **Voeg de gekozen locatie toe** (hier was dat D:\ ) aan het **einde** van het **Target** veld.
      6.  Indien je meerdere drives op je computer hebt, en je wenst Jupyter notebooks vanop verschillende drives te starten, dan kun je gebruik maken van snelkoppelingen tussen de verschillende drives.(Merk op dat je eindpunt van een snelkoppeling telkens de rol	van een *root* map krijgt.)
4. **Update van Python omgeving naar huidige versie**
   1. Start de **Anaconda Powershell Prompt** als **_administrator_** (zwarte venster icoon)
   2. Om de meest recente versie van conda te hebben type je in de powershell: **conda update conda**.
   3. Hoewel Jupyter notebooks reeds zeer krachtig zijn, zijn er enkele plugins welke je werk nog eenvoudiger kunnen maken. Hiervoor ga je als volgt te werk.
      1.   In de Powershell type je: **conda install -c conda-forge Jupyter_contrib_nbextensions**
      2.  Daarna type je, nog steeds in de Powershell: **Jupyter contrib nbextension install -user**
      3. Open nu het **Jupyter notebook** programma (oranje icoon)
      4.  In de webbrowser, in de tab waar je de bestandsboom ziet klik je op de tab **Nbextensions**
      5.   Deselecteer **Disable configuration...**
      6.  Selecteer nu de extensies van je keuze. Bijvoorbeeld:
          - *Latex environments* die je toelaten latex vergelijkingen in jouw **markdown** opmaak toe te voegen.
          - *Scratchpad* een kleine kladblok pop-up waarin je snel python commando's kan uittesten.
          - *ExecuteTime* om te zien hoe lang het duurde om een cel uit te voeren.
          - *Codefolding* wat je toelaat om stukken code samen te vouwen en zo een compactere en overzichtelijkere notebook te creëren.

###  <a name='miniconda'> </a> 2.2. Miniconda
Miniconda is een lichtgewicht broertje van Anaconda. Dit is een interessante omgeving welke je bijvoorbeeld kan gebruiken om zelf python te installeren in een supercomputer omgeving. De installatie instructies zijn [hier](https://docs.conda.io/en/latest/miniconda.html) te vinden.

### <a name='vscode'> </a> 2.3. VSCode Installatie
Indien je reeds *Visual Studio Code* geïnstalleerd hebt om aan code-ontwikkeling in een andere programmeertaal te doen, kun je ook hier python aan toevoegen. Je kan zowel Jupyter notebooks als python scripts in VSCode schrijven, bekijken en uitvoeren. Installatie instructies kunnen [hier](https://code.visualstudio.com/docs/languages/python) gevonden worden.
