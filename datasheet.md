# Datasheet for Dataset

## Dataset name
Simulated Precision Mitochondria Onion Nanocarrier Dataset

## One-line description
A synthetic, literature-benchmarked dataset describing candidate multilayer nanocarrier architectures for mitochondrial matrix delivery and expression of engineered human mtDNA.

## Motivation
This dataset was created to support a computational proof-of-concept programme focused on a six-layer onion nanocarrier for mitochondrial genome engineering. The dataset enables analysis of how nanocarrier design variables may influence staged delivery, matrix access, reporter expression, persistence, and cell viability.

## Dataset composition
The dataset contains simulated candidate architectures, with each row representing one design instance. Variables include:
- material composition features,
- synthetic nucleoid properties,
- mitochondrial targeting and membrane-fusion variables,
- milestone pass or fail outcomes,
- matrix-delivery and reporter-expression metrics,
- cell-viability and persistence values,
- cluster assignments and down-selection information.

Associated derived tables summarize:
- descriptive statistics,
- milestone pass rates,
- classifier performance,
- feature importance,
- regression metrics,
- cluster summaries,
- top-ranked designs.

## Instances
Each instance corresponds to one simulated nanocarrier design evaluated under the programme logic.

## Data origin
The dataset is synthetic. It was generated algorithmically using parameter ranges designed to be biologically plausible and informed by peer-reviewed literature on:
- TFAM-mediated mtDNA packaging,
- mitochondrial membrane biology,
- cardiolipin and OPA1-related fusion,
- ionizable lipid nanoparticle behaviour,
- lipophilic cation mitochondrial targeting,
- reporter-gene output logic.

It is not a direct measurement dataset from cells, tissues, animals, or patients.

## Collection process
No human participants, animals, or clinical records were involved. The dataset was created in silico through stochastic simulation and rule-based milestone logic.

## Preprocessing
Preprocessing steps include:
- variable generation within constrained biologically plausible ranges,
- derivation of milestone pass or fail labels,
- generation of reporter outputs conditional on delivery variables,
- construction of composite performance scores,
- optional scaling and dimensionality reduction for clustering and visualization.

## Recommended uses
This dataset is appropriate for:
- computational exploration,
- proof-of-concept analysis,
- machine-learning benchmarking on structured synthetic biology-inspired data,
- hypothesis generation for mitochondrial nanocarrier design,
- visualization and programme planning.

## Non-recommended uses
This dataset should not be used for:
- biological claims of demonstrated mitochondrial delivery,
- direct translational inference,
- clinical prediction,
- safety claims,
- benchmarking against real experimental data without clear qualification.

## Known limitations
- The dataset is simulated and therefore reflects design assumptions embedded in the generator.
- Some relationships are intentionally structured to reflect mechanistic expectations.
- The dataset does not capture full biological complexity such as mitophagy, mitochondrial population heterogeneity, organelle dynamics, immune sensing, long-term inheritance, or replication competition.
- Reporter outputs are synthetic proxies, not biochemical assays.

## Sensitive content
The dataset does not contain:
- personally identifiable information,
- patient data,
- protected health information,
- animal identifiers,
- proprietary laboratory records.

## Validation
Internal validation includes:
- inspection of value ranges,
- milestone consistency checks,
- summary-statistic review,
- model-based assessment of whether the generated data produce interpretable mechanistic structure.

External experimental validation has not yet been performed.

## Dataset files
Primary and associated files include:
- `simulated_precision_mito_dataset.csv`
- `table_1_dataset_summary.csv`
- `table_2_milestone_pass_rates.csv`
- `table_3_classifier_metrics.csv`
- `table_4_classifier_feature_importance.csv`
- `table_5_regression_metrics.csv`
- `table_6_regression_permutation_importance.csv`
- `table_7_cluster_summary.csv`
- `table_8_top20_designs.csv`
- `table_9_compact_results_summary.csv`

## Distribution
The dataset is distributed as part of the repository for academic, conceptual, and exploratory use. Any reuse should preserve the statement that the dataset is synthetic.

## Versioning
This datasheet describes the current proof-of-concept dataset version associated with the executed notebook and exported CSV tables. Future versions should document:
- changed variable definitions,
- altered simulation assumptions,
- revised milestone logic,
- inclusion of experimental data if added later.

## Contact
Mark Ihrwell R. Petalcorin, PhD  
m.petalcorin@gmail.com
