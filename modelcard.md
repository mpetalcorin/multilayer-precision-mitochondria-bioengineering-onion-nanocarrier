# Model Card

## Model name
Precision Mitochondria Onion Nanocarrier Proof-of-Concept Models

## One-line description
A set of simulation-driven machine-learning models for predicting end-to-end mitochondrial delivery success and reporter output from layered nanocarrier design features.

## Model scope
This model card describes the statistical and machine-learning components used in a computational proof-of-concept study of a six-layer onion nanocarrier for mitochondrial matrix delivery and expression of engineered human mtDNA.

The workflow includes:
- a supervised classification model for overall programme success,
- a supervised regression model for reporter output,
- unsupervised clustering for architecture-class discovery,
- correlation and partial-dependence analyses for mechanistic interpretation.

## Intended use
These models are intended to:
- identify candidate design variables associated with success,
- support down-selection of nanocarrier architectures,
- provide interpretable hypotheses for experimental prioritization,
- explore structure in the simulated design space.

## Out-of-scope use
These models are not intended for:
- clinical decision-making,
- patient stratification,
- prediction of therapeutic efficacy in humans,
- direct experimental validation,
- regulatory use,
- claims of real mitochondrial delivery success.

## Model inputs
Input features include simulated nanocarrier design and assay variables such as:
- particle size,
- ionizable lipid fraction,
- TPP density,
- TFAM-to-mtDNA ratio,
- nucleoid size,
- nuclease resistance,
- cardiolipin percentage,
- OPA1-mimic activity,
- MOF stability and logic scores,
- endosomal escape,
- mitochondrial accumulation,
- OMM fusion,
- IMM content mixing,
- cell viability.

## Model outputs
### Classification output
Binary prediction of overall end-to-end programme success.

### Regression output
Predicted reporter signal, expressed as fold over background.

### Clustering output
Architecture-cluster assignment in reduced feature space.

## Model types
- Random forest classifier for overall success.
- Random forest regressor for reporter output.
- Principal component analysis and clustering for architecture classes.

## Training data
The training data are synthetic and generated from biologically plausible parameter ranges informed by peer-reviewed mitochondrial biology, membrane fusion, nanocarrier, and reporter-system literature. The dataset is not derived from direct wet-lab measurements.

## Performance summary
In the proof-of-concept notebook:
- the classification model achieved near-perfect discrimination on the held-out synthetic test set,
- the regression model captured a moderate fraction of reporter-output variance,
- feature-importance analysis consistently highlighted nuclease resistance and inner membrane fusion-related variables as major determinants.

These values reflect performance on simulated data only.

## Interpretability
Interpretability is supported through:
- feature-importance ranking,
- permutation importance,
- confusion matrix analysis,
- observed-versus-predicted plots,
- partial-dependence plots,
- cluster-level summaries.

## Key assumptions
The models assume that:
- the layered architecture can be represented by measurable component features,
- milestone transitions can be approximated using threshold-based logic,
- reporter output depends on delivery-state variables in a structured way,
- biologically benchmarked synthetic ranges approximate a meaningful hypothesis space.

## Limitations
- The data are simulated rather than experimentally measured.
- The models cannot capture all physical, biochemical, or cellular nonlinearities of real mitochondria.
- Feature importance on synthetic data reflects the structure of the simulation framework and not proven biological causality.
- Performance metrics may be optimistic relative to real-world biological systems.
- The current models do not represent long-term replication, heteroplasmy competition, immune sensing, or organelle inheritance.

## Risks
Potential risks include:
- over-interpretation of synthetic performance,
- false confidence in specific design variables,
- assuming predictive validity outside the simulated space,
- treating classifier success as evidence of biological feasibility.

## Ethical and safety considerations
This work concerns foundational delivery concepts for mitochondrial genome engineering. Any future translation into experimental practice should include:
- rigorous biosafety review,
- compartment-specific validation,
- exclusion of off-target effects,
- careful assessment of persistence and inheritance,
- transparent reporting of failure modes and uncertainty.

## Maintenance
This model card applies to the current proof-of-concept repository version. It should be updated if:
- new datasets are added,
- the simulation framework changes,
- new models replace the current pipeline,
- experimental data are incorporated.

## Contact
Mark Ihrwell R. Petalcorin, PhD  
m.petalcorin@gmail.com
