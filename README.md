# Roborok-S5Max-Package
Gestione Roborock S5Max da HomeAssistant


<img src="https://github.com/skillaci86/Roborok-S5Max-Package/blob/main/Anteprima.png" alt="Anteprima">


# Prerequisiti
Custom Component necessari:
  - button-card 
  - vertical-stack-in-card
  - hui-horizontal-stack-card
  - text-divider-row
  - xiaomi-vacuum-map-card

Integrazioni HACS necessarie:
- Xiaomi Cloud Map Extractor (solo se volete la card con la mappa)
  
# Permette di
  - Gestione acqua 
  - Gestione ventole
  - Multistanza
  - Ripetizioni singole stanze
  - Pulizia Zone
  - Vai alla posizione
  - Svuota Sacchetto
  - Carica Acqua
  - Reset sensori vacuum
  - Notifiche Telegram/google

# Spiegazioni
Questo packages è molto articolato. Comprende funzioni che probabilmente a molti di voi non serviranno e quindi potrete eliminare.

- Consumabili:
Il packages ha dei sensori interattivi per i filtri e i pezzi di ricambio. Manderà un avviso quando stanno per esaurirsi.

- Serbatoio: 
Ho impostato un sensore counter che conta i cicli di pulizia, superati 5 (è possibile customizzare quest'opzione) cicli il serbatoio verrà considerato pieno e verrà inviata una notifica per ricordarsi di svuotarlo. 
Ci sono due modi di svuotare il serbatoio:
  - 1 - Cliccare sull'immagine svuota il serbatoio (che appare solo quando il serbatoio è pieno). Automaticamente il robottino si avvicina al punto del cestino della spazzatura.
  - 2 - Oppure se si vuole svuotare prima basta cliccare sull'icona del cestino, automaticamente il robottino si avvicino al punto del cestino.

<img src="https://github.com/skillaci86/Roborok-S5Max-Package/blob/main/SvuotaSerbatoio.png" alt="Anteprima">	 

- Serbatoio Acqua: 
Ho creato un tasto che fa in modo che il robottino si avvicina alla cucina per permettere la carica dell'acqua
Basta cliccare sull'icona della goccia ed automaticamente il robot si avvicina alla cucina.

- Reset Sensori 
Per ogni sensore ho creato un tasto che permette il reset del count senza usare l'applicazione MiHome.

<img src="https://github.com/skillaci86/Roborok-S5Max-Package/blob/main/ResetSensori.png" alt="Anteprima">	 

# Funzioni speciali
- Il robottino torna alla base da solo in caso di errore o perdita della mappa.


# Impostazioni
Tutto (o quasi) quello che dovete impostare indicato con delle XXX, vi basta cercar X nel testo per trovare cosa dovete sostituire.
In linea di massima dovrete correggere i settaggi del vostro Vacuum, i notify.XXXX.
Questo packages è stato copiato/modificato in base alle mie esigenze dal progetto originale di Francesco Calamita al quale ringrazio per aver prodotto la maggior parte di codice :-)!!!
