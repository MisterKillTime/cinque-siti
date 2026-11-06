# Cinque siti, cinque settori

**Live:** https://misterkilltime.github.io/cinque-siti/

Cinque siti costruiti con l'AI in una sera, per dimostrare un punto: con lo strumento giusto e la voglia di usarlo bene si fa molto più di "un prompt". Un file HTML per sito, niente framework, niente template.

| Sito | Settore | Cosa c'è dentro |
|---|---|---|
| [Forgia Training Club](forgia/) | Palestra | titolo che cambia spessore seguendo il cursore, scintille sul nastro (clicca per farle esplodere), stato aperto/chiuso e affollamento previsto in tempo reale, calcolatore del massimale con bilanciere caricato a dischi, abbonamenti in 3D |
| [Trattoria La Grangia](grangia/) | Ristorante | paesaggio della risaia che segue l'ora vera (alba, tramonto, notte con lucciole), piatto del giorno disegnato con il vapore, menu animato con abbinamento vini, prenotazione |
| [Studio Dentistico Morandi](morandi/) | Studio medico | sfondo fluido animato, odontogramma cliccabile, slider prima/dopo automatico, prenotazione a step, timer dello spazzolino guidato, calcolatore rate |
| [Torrefazione Ottone](ottone/) | E-commerce | chicchi che cadono e scappano dal cursore, ruota degli aromi, quiz, laboratorio di estrazione con caraffa che si riempie, carrello funzionante |
| [Meridiana Viaggi](meridiana/) | Agenzia viaggi | mappamondo da girare con notte e giorno reali, zoom sul punto cliccato, aereo in volo sulla rotta, Street View integrato, passaporto con timbri da collezionare |

## Lighthouse (mobile)

| Sito | Prestazioni | Accessibilità | Best practice | SEO |
|---|---|---|---|---|
| [Forgia Training Club](forgia/) | 99 | 100 | 100 | 100 |
| [Trattoria La Grangia](grangia/) | 99 | 100 | 100 | 100 |
| [Studio Dentistico Morandi](morandi/) | 98 | 100 | 100 | 100 |
| [Torrefazione Ottone](ottone/) | 99 | 100 | 100 | 100 |
| [Meridiana Viaggi](meridiana/) | 89 | 100 | 100 | 100 |

## SEO e GEO

- **Dati strutturati Schema.org** su ogni pagina: `ExerciseGym`, `Restaurant` con menu completo, `Dentist` + `FAQPage`, `Store` con catalogo prodotti, `TravelAgency` con `TouristTrip` e coordinate.
- **Open Graph e Twitter Card** con immagine dedicata (`og.png`) per ogni sito: anteprima ricca quando il link viene condiviso.
- **URL canonici, meta description uniche, titoli pensati per la ricerca locale.**
- **[`sitemap.xml`](sitemap.xml)** con tutte le pagine.
- **[`llms.txt`](llms.txt)**: riassunto in Markdown dei fatti chiave di ogni attività, per i motori di risposta AI (ChatGPT, Claude, Perplexity).
- **[`robots.txt`](robots.txt)** che ammette esplicitamente i crawler AI. Nota: i crawler leggono `robots.txt` solo alla radice del dominio, quindi questo file diventa effettivo con un dominio personalizzato.

## Struttura

```
index.html        pagina d'ingresso
forgia/           palestra
grangia/          ristorante
morandi/          studio dentistico
ottone/           e-commerce
meridiana/        agenzia viaggi (dati cartografici Natural Earth via world-atlas)
sitemap.xml  robots.txt  llms.txt  404.html
```

Le attività, gli indirizzi e i numeri di telefono sono di fantasia.
