This repository hosts  ressources for human germline analysis : reference genome and databases for variants annotation.
This is intented to use with Ensembl [https://www.ensembl.org/info/docs/tools/vep/index.html](Variant Effect Predictor) or VEP.

Ressources, called *assets*, are managed with [scidataflow](https://github.com/vsbuffalo/scidataflow) for download, update and integrity checks.


## Available data

| Asset   | Latest                  | Other                   |
|---------|-------------------------|-------------------------|
| Genome  | GRCh38.p14 (md5sum)     | GRch38 + index (md5sum) |
| CADD    | v1.7 on GRCh38 (md5sum) |                         |
| Clinvar | GRCh38                  |                         |
| dbSNP   | GRCh38.p14 (md5sum)     |                         |
| VEP     | v112 on GRCH38 (sum)    |                         |

Notes:
- Only latest versions for each dataset are available at the moment. 
- Only public ressources through https are used.
- Data is roughly 140G in size
- Genome is available as "pipeline-ready" (GRCh38) or latest version without indexes (GRCh38.p14)

## Filename convention
Filename are lowercase only and renamed to match `$DB_$GENOME_$VERSION_$DESC.$EXT` with
- `DB` is the database name (e.g clinvar),
- `GENOME` is `grch38` or `t2t`
- `VERSION` is the database version (`v1.7` for clinvar for exaple)
- `DESC` is a description (`snv` for example)
- `EXT` is the file extension (often `.gz`)
If there are different versions of the database, all versions are stored in the same folder `$DB`.
