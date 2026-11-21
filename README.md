# Salute mentale dei ragazzi – dataviz Radar QN

Pagine pubblicate su GitHub Pages. Ogni grafico legge il proprio CSV in `data/`: per aggiornarlo basta cambiare il CSV.

- **Accessi dei minori al pronto soccorso per disagio psichico**: https://caterinamalanetto-star.github.io/caterinamalanetto-star-salute-mentale-ragazzi/pronto-soccorso/
- **Accessi dei minori al pronto soccorso per gruppo di diagnosi**: https://caterinamalanetto-star.github.io/caterinamalanetto-star-salute-mentale-ragazzi/diagnosi/
- **Casi gestiti dalle linee 1.96.96 e 114**: https://caterinamalanetto-star.github.io/caterinamalanetto-star-salute-mentale-ragazzi/linee-ascolto/
- **Motivi delle richieste di aiuto al 1.96.96**: https://caterinamalanetto-star.github.io/caterinamalanetto-star-salute-mentale-ragazzi/motivi/
- **Servizi attivati dal 1.96.96 dopo la chiamata**: https://caterinamalanetto-star.github.io/caterinamalanetto-star-salute-mentale-ragazzi/dopo-la-chiamata/

## Dati e fonti

- `data/pronto-soccorso-minori.csv`, `data/diagnosi-pronto-soccorso-minori.csv`: Ministero della Salute, Rapporto salute mentale 2021, 2022, 2023, 2024, tabella 12.6.1 (NSIS-EMUR). I totali per diagnosi coincidono con il totale 0-17 di ogni anno.
- `data/casi-linee-ascolto.csv`: Telefono Azzurro, bilanci sociali 2019-2025 (dato di ogni anno come riportato nel bilancio di quell'anno).
- `data/aree-bisogno-1-96-96.csv`, `data/attivazioni-1-96-96.csv`: Telefono Azzurro, dossier «Ascoltare il disagio, leggere i bisogni» (servizio 1.96.96, dati 2025), tabelle 4-7 e figure 4 e 10. «Altre aree» nel grafico dei motivi è calcolata per differenza (100 − somma delle quattro aree).

## Snippet per il CMS

Vedi `index.html`: per ogni dataviz c'è l'iframe con lo script inline. Se ci sono più dataviz nello stesso articolo, lo script può restare in ognuna (il controllo `__radarQNv2` evita doppioni).
