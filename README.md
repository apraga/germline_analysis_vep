This repository hosts  ressources for human germline analysis : reference genome and databases for variants annotation.
This is intented to use with Ensembl [https://www.ensembl.org/info/docs/tools/vep/index.html](Variant Effect Predictor) or VEP.

Ressources, called *assets*, are managed with [scidataflow](https://github.com/vsbuffalo/scidataflow) for download, update and integrity checks.

Notes:
- Only latest versions for each dataset are available at the moment. 
- Only public ressources through https are used.
- Data is roughly 140G in size
- Genome is available as "pipeline-ready" (GRCh38) or latest version without indexes (GRCh38.p14)

Available data

| Asset   | Latest                  | Other                   |
|---------|-------------------------|-------------------------|
| Genome  | GRCh38.p14 (md5sum)     | GRch38 + index (md5sum) |
| CADD    | v1.7 on GRCh38 (md5sum) | v1.6 on GRCh38 (md5sum) |
| Clinvar | GRCh38                  |                         |
| dbSNP   | GRCh38.p14 (md5sum)     |                         |
| VEP     | v112 on GRCH38 (sum)    |                         |
