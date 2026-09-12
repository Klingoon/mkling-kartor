# mkling-kartor

Separat, offentlig distribution av kartunderlag och ljud för [Kling Labs](https://www.mkling.org).

## EDGAR CO₂ 1970–2024

55 årsvisa texturer, 3600 × 1800 pixlar (0,1° rutnät), kopierade utan omkodning från mkling.org-projektet. Ursprung: IEA-EDGAR CO₂, EDGAR_2025_GHG, TOTALS, European Commission Joint Research Centre (JRC) / IEA.

- [Källa, dokumentation och återanvändningsvillkor](https://edgar.jrc.ec.europa.eu/dataset_ghg2025)
- [Manifest](data/edgar-co2-0p1deg/manifest.json)
- Publik URL: `https://kartor.mkling.org/data/edgar-co2-0p1deg/edgar-co2-1970-0p1deg.webp`

Filerna är härledda visualiseringstexturer, inte ursprungliga numeriska mätdata: en fast logaritmisk normalisering till 8 bitar och WebP quality 90 har redan applicerats i källprojektet. Flytten ändrar inga bildvärden eller filbytes. 2023–2024 inkluderar EDGAR Fast Track-estimat.

GitHub Pages publicerar rotkatalogen på grenen `main`. `CNAME` kopplar kartor.mkling.org. Ingen Git LFS används. `checksums.sha256` dokumenterar filernas SHA-256 för verifiering.

## Jordgloben: terräng och färger

`data/earth/` innehåller 170 höjdrutor från GEBCO_2026, NASA Blue Marble (juli 2004) och NOAA:s landmask. Filerna har kopierats byte för byte från jordlabben, utan ändrad upplösning eller komprimering. Höjdrutorna är härledda visningsdata, inte originaldatabasens fulla upplösning.

- [GEBCO-manifest, bearbetning, begränsningar och attribution](data/earth/manifest.json)
- [NASA/NOAA-källor, originaladresser och attribution](data/earth/colour-sources.json)

GEBCO-underlaget är inte avsett för navigation. Ingen källa antyds stödja Kling Labs.

## Musik och licenser

Ljudfilerna i `audio/` är oförändrade kopior av labbens befintliga M4A-filer. Rättigheter tillhör respektive upphovsperson. Ingen generell kodlicens i detta projekt ersätter dessa villkor.

| Fil | Verk och upphovsperson | Licens | Källa |
| --- | --- | --- | --- |
| space-station.m4a | Space Station — Alexandr Zhelanov | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) | [OpenGameArt](https://opengameart.org/content/space-station-1) |
| la-madeline-au-truffe.m4a | La Madeline Au Truffe (composed by Jeris) — basematic feat. Jeris | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) | [ccMixter](https://ccmixter.org/files/basematic/33580) |
| namu-myoho-renge-kyo.m4a | Namu Myōhō Renge Kyō — Dreamonizer feat. SO SHA & Zenboy1955 | [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) | [ccMixter](https://ccmixter.org/files/Dimensional_Pulse/71076) |
| boss-pidge.m4a | B O S S P I D G E — SO SHA | [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) | [ccMixter](https://ccmixter.org/files/thatcrazylittleasian/66766) |

De två BY-NC-spåren får endast återanvändas enligt licensens icke-kommersiella villkor. Källprojektets ljudfiler är M4A-versioner; inga ytterligare ändringar har gjorts vid denna flytt.

`lab-assets-checksums.json` dokumenterar varje ny fils storlek och SHA-256. Webbplatsen hämtar filerna via HTTPS från `raw.githubusercontent.com`, låsta till en specifik Git-commit, liksom de befintliga CO₂-kartorna. DNS och `CNAME` har inte ändrats.

Huvudwebbplats, säkerhetskopior och inloggningsuppgifter ingår inte.
