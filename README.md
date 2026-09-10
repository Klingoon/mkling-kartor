# mkling-kartor

Separat, offentlig distribution av kartunderlag för [Kling Labs](https://www.mkling.org).

## EDGAR CO₂ 1970–2024

55 årsvisa texturer, 3600 × 1800 pixlar (0,1° rutnät), kopierade utan omkodning från mkling.org-projektet. Ursprung: IEA-EDGAR CO₂, EDGAR_2025_GHG, TOTALS, European Commission Joint Research Centre (JRC) / IEA.

- [Källa, dokumentation och återanvändningsvillkor](https://edgar.jrc.ec.europa.eu/dataset_ghg2025)
- [Manifest](data/edgar-co2-0p1deg/manifest.json)
- Publik URL: `https://kartor.mkling.org/data/edgar-co2-0p1deg/edgar-co2-1970-0p1deg.webp`

Filerna är härledda visualiseringstexturer, inte ursprungliga numeriska mätdata: en fast logaritmisk normalisering till 8 bitar och WebP quality 90 har redan applicerats i källprojektet. Flytten ändrar inga bildvärden eller filbytes. 2023–2024 inkluderar EDGAR Fast Track-estimat.

GitHub Pages publicerar rotkatalogen på grenen `main`. `CNAME` kopplar kartor.mkling.org. Ingen Git LFS används. `checksums.sha256` dokumenterar filernas SHA-256 för verifiering.

Endast detta kartunderlag publiceras här. Huvudwebbplats, säkerhetskopior och inloggningsuppgifter ingår inte.
