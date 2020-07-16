# boka_prov_trafikverket
En skript som automatiskt söker efter förarprov.  
Skripten bokar inga tider själv utan tiden läggs i varukorgen som då blir reserverad i 15 minuter.  
Ett ljud kommer spelas upp när en tid har hittats.


## VIKTIGT
Skripten har endast testats vid bokning av körprov B men bör funka för de flesta proven.  
config.py måste matcha det som står på hemsidan. Står det t.ex. "Ja, manuell" på hemsidan ang. hyrbil så måste det stå precis så i config.py  
Följ https://code.visualstudio.com/docs/python/python-tutorial för att ladda ned Python och VSCode  
Se https://www.w3schools.com/python/python_strings.asp för strings dokumentation  
Se https://www.w3schools.com/python/python_lists.asp  för lists dokumentation  
Se LICENSE


## Donationer
Om du känner för att bidra till mina körlektioner så kan du donera en slant nedan:  
  
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=H76THWVZQ7KA4)  


## Installation

### 1. Installera nödvändiga paket
> pip install -r requirements.txt

### 2. Installera chromedriver
Se: https://sites.google.com/a/chromium.org/chromedriver/home  
Installera samma version som du har på google chrome  
Se: chrome://settings/help

### 3. Fyll i config.py
Döp om config_sample.py till config.py
Texten måste matcha den på hemsidan. Gå igenom manuellt och fyll i.

#### 1. chromedriver_location
Lägg chromedriver.exe i C:/ eller ändra config.py till filens sökväg

#### 2. license_type
Lägg till behörigheten du vill boka prov inför (ex. B, B96, Buss etc)

#### 3. exam
Lägg till vilket prov du vill boka (ex. Körprov B, Kunskapsprov B)

#### 4. rent_option
Välj mellan ex. "Nej", "Ja, automat" eller "Ja, manuell". Ta bort eller kommentera (#) om inte används (ex. vid kunskapsprov B eller MC)

#### 5. language_option
Välj språk, ex. Svenska, Engelska. Ta bort eller kommentera (#) om inte används (ex. vid körprov B eller MC)

#### 5. dates
Lägg till 2 datum. Skripten kommer leta prov mellan dem två

#### 6. locations
Lägg till de orterna du vill boka provet vid

