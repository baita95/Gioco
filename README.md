# Salta e Centra

Gioco mobile: tocca lo schermo per far saltare l'anello dall'acqua, inclina il telefono per guidarlo a mezz'aria e centralo sul bastoncino del suo colore.

Richiede HTTPS per funzionare l'inclinometro (`DeviceOrientationEvent`) — per questo va pubblicato su GitHub Pages e non aperto come file locale.

## Come pubblicarlo (GitHub Pages)

### Opzione A — dal sito github.com (senza terminale)

1. Vai su [github.com/new](https://github.com/new), crea un repository nuovo (es. `salta-e-centra`), pubblico.
2. Nella pagina del repo appena creato, clicca **"uploading an existing file"**.
3. Trascina dentro il file `index.html` (e questo `README.md` se vuoi).
4. Fai commit direttamente su `main`.
5. Vai su **Settings > Pages** (menu a sinistra).
6. In **Source** seleziona il branch `main` e cartella `/ (root)`, poi **Save**.
7. Dopo circa 1 minuto sarà online su:
   `https://<tuo-username>.github.io/salta-e-centra/`

### Opzione B — da terminale (se hai già git configurato, come per il lap timer)

```bash
cd salta-e-centra
git init
git add .
git commit -m "Prima versione del gioco"
git branch -M main
git remote add origin https://github.com/<tuo-username>/salta-e-centra.git
git push -u origin main
```

Poi attiva Pages da Settings > Pages come al punto 5-6 sopra.

## Nota importante

Apri il link `https://...github.io/...` **da Safari o Chrome del telefono**, non dall'app Claude o da un browser in-app: solo così il permesso "Motion & Orientation Access" viene richiesto e concesso correttamente (su iPhone: Impostazioni > Safari > Motion & Orientation Access deve essere attivo).

## File

- `index.html` — il gioco completo, nessuna dipendenza esterna, nessuna build necessaria.
