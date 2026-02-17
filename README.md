# RNASeq Stats Export

## R Markdown files

- `chemcells_rnaseq_data_1_read_data.Rmd`: Reads raw RNA-seq/count and metadata inputs, builds ETBR-focused sample annotations, performs TMM normalization, detects/removes outliers, and prepares cleaned intermediate data objects.
- `chemcells_rnaseq_stat_1_regression.Rmd`: Loads processed phenotype/RNA/CN data and runs gene-wise linear and mixed-model regressions (including nonlinear variants) to estimate ETBR association effects.
- `chemcells_rnaseq_stat_2_lon_track.Rmd`: Integrates regression outputs with annotation resources (including MitoCarta), compares association signals across models, and derives pathway-style longitudinal/response categories for ETBR genes.
- `chemcells_rnaseq_stat_X_plots.Rmd`: Assembles regression/pathway outputs into publication-ready figures and exports visualizations for the RNA-seq/mtDNA analysis.

## Folder file listings

### `01_Inputs`

- `01_Inputs/AllSamples.Randomized.RNAseq.csv`
- `01_Inputs/ChemicalProjectMatchUpDeltaCT.xlsx`
- `01_Inputs/Human.MitoCarta3.0.xlsx`
- `01_Inputs/mart_export.txt`
- `01_Inputs/merged.csv`

### `02_Intermediates`

- `02_Intermediates/ETBR_CN.rds`
- `02_Intermediates/ETBR_CN_anova.rds`
- `02_Intermediates/ETBR_CN_lm.rds`
- `02_Intermediates/ETBR_CN_lm2.rds`
- `02_Intermediates/ETBR_CN_lmer.rds`
- `02_Intermediates/ETBR_CN_lmer2.rds`
- `02_Intermediates/ETBR_CN_ns2.rds`
- `02_Intermediates/ETBR_CN_ns3.rds`
- `02_Intermediates/ETBR_COV.tsv: combined _1 and _2 for the full file`
- `02_Intermediates/ETBR_LON.rds`
- `02_Intermediates/ETBR_LON_lm.rds`
- `02_Intermediates/ETBR_LON_lmer.rds`
- `02_Intermediates/ETBR_MT.rds`
- `02_Intermediates/ETBR_MT_lm.rds`
- `02_Intermediates/ETBR_MT_lmer.rds`
- `02_Intermediates/ETBR_NC_LON.rds`
- `02_Intermediates/ETBR_dose_lm.rds`
- `02_Intermediates/ETBR_dose_lmer.rds`
- `02_Intermediates/ETBR_linear.rds`
- `02_Intermediates/ETBR_paths.rds`
- `02_Intermediates/Experiment_Samples.rds`
- `02_Intermediates/RNA_TMM.rds`
- `02_Intermediates/mtDNA.rds`
