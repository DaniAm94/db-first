# DB First
### nome repo: db-first
    Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.
    Per la consegna, potete inserire la vostra tabella in un file markdown come vi ho fatto vedere a lezione, oppure farla su Excel, Fogli Google ecc e fare uno screen.


Colonne|Tipo di dato|Attributi
--|--|--
id|BIGINT|PRIMARY_KEY, AUTO_INCREMENT
targa|CHAR(7)|NOTNULL, UNIQUE
num_telaio|CHAR(17)|NOTNULL, UNIQUE
marchio|VARCHAR(20)|NOTNULL
modello|VARCHAR(20)|NOTNULL
allestimento|VARCHAR(20)|NULL
paese_d'origine|CHAR(5)|NULL
tipologia_cambio|CHAR(1)|NOTNULL
porte|TINYINT|NOTNULL
posti|TINYINT|NOTNULL
potenza(CV)|SMALLINT|NOTNULL
carburante|CHAR(1)|NOTNULL
cilindrata|TINYINT|NOTNULL
trazione|CHAR(1)|NOTNULL, DEFAULT('a') (anteriore)
classe_emissioni|CHAR(1)|NOTNULL
consumo_medio(km/l)|TINYINT|NOTNULL
classe_veicolo(Suv,Berlina...)|CHAR(1)|NOTNULL
colore|VARCHAR(20)|NOTNULL
interni|VARCHAR(20)|NOTNULL
inizio_produzione|YEAR|NOTNULL
fine_produzione|YEAR|NULL
anno_immatricolazione|YEAR|NOTNULL
numero_proprietari|TINYINT|NOTNULL, DEFAULT(1)
km_percorsi|MEDIUMINT|NOTNULL
stato_carrozzeria|CHAR(1)|NOTNULL
stato_interni|CHAR(1)|NOTNULL
stato_pneumatici|CHAR(1)|NOTNULL
ultimo_tagliando|DATE|NOTNULL
scadenza_revisione|DATE|NOTNULL
incidentata_e_riparata|TINYINT/BOOL|NOTNULL, DEFAULT(0)
autoradio|TINYINT/BOOL|NULL
bluetooth|TINYINT/BOOL|NULL
abs|TINYINT/BOOL|NOTNULL
controllo_trazione|TINYINT/BOOL|NULL
airbag_laterali|TINYINT/BOOL|NULL
