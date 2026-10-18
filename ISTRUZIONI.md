# Lavagna – installazione

## Contenuto della cartella
- `index.html`, `manifest.json`, `sw.js`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`: l'app, con l'emblema del box come icona.
- `icone-alternative/A` (disco), `B` (kettlebell) e `C` (lavagna): icone di ricambio.
- Il file dei tuoi dati, `lavagna-dati.json`, è **separato** e **non va mai caricato su GitHub**: il repository è pubblico.

## 1. Pubblicare su GitHub Pages (dal Mac, circa 10 minuti)
1. Crea un account su github.com.
2. In alto a destra: **+ → New repository**. Nome `lavagna`, visibilità **Public**, poi **Create repository**.
3. Clicca **uploading an existing file** e trascina **il contenuto** della cartella (non lo zip, e senza questo file di istruzioni se preferisci). Poi **Commit changes**.
4. Vai in **Settings → Pages**. In *Source* scegli **Deploy from a branch**, branch **main**, cartella **/ (root)**, poi **Save**.
5. Dopo 1–2 minuti l'app è online su `https://TUONOME.github.io/lavagna/`.

## 2. Installare sull'iPhone
1. Apri l'indirizzo in **Safari**, poi **Condividi → Aggiungi alla schermata Home**.
2. Da qui in poi **apri sempre l'app dall'icona**. Le app sulla Home hanno uno spazio dati separato da Safari, quindi importa i dati da lì.

## 3. Importare i tuoi dati
1. Dal Mac copia `lavagna-dati.json` in **iCloud Drive**.
2. Nell'app compare *Benvenuto*. Tocca **Importa backup** e scegli il file da iCloud Drive.

## 4. Chiave API per leggere le foto
1. Vai su **console.anthropic.com** e crea l'account.
2. In **Settings → Billing → Buy credits** carica 5 $. Lascia **spenta** la ricarica automatica.
3. In **API Keys → Create key**, chiamala `Lavagna` e copiala.
4. Nell'app tocca **⚙︎**, incolla la chiave e premi **Salva e verifica**.

La chiave resta solo sul telefono. Se la perdi o la esponi, revocala dalla console e creane una nuova.

## 5. Sul Mac
- Apri lo stesso indirizzo in Safari, poi **File → Aggiungi al Dock**.
- I dati di Mac e iPhone sono separati. Per passarli da uno all'altro: **⚙︎ → Esporta backup** su iCloud Drive, poi **Importa backup** sull'altro dispositivo.
- L'importazione **sostituisce** i dati presenti.

## Backup
Ogni tanto fai **⚙︎ → Esporta backup con foto** e salvalo su iCloud Drive. Se elimini l'app dalla Home, i dati sul telefono si perdono.

## Aggiornare l'app
1. Ricarica il nuovo `index.html` nel repository: **Add file → Upload files**.
2. In `sw.js` cambia `VERSION` (es. `lavagna-v2`).
3. Chiudi e riapri l'app due volte.

## Cambiare icona
1. Sostituisci i tre file PNG con quelli di `icone-alternative/A`, `B` o `C`.
2. Rimuovi l'icona dalla Home e aggiungila di nuovo. I dati restano finché non elimini l'app.
