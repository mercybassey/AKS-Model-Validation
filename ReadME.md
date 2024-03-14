## Aqueous Kinetic Solubility Model Validation

This project uses the Aqueous Kinetic Solubility model from Ersilia 
Hub to predict the solubility of 1000 compounds sourced from public 
repositories. The model, identified by its EOS model ID `eos74bo`.

## Data Collection and Preparation 

This project required a dataset of chemical compounds for analysis. 
The following steps outline how the data was selected and prepared;
this dataset was collected from PubChem, one of the most comprehensive
chemical databases available.

- **Step 1**: To initiate the research, the PubChem database's search functionality 
was used to identify compounds containing ISOSMILES data. 

- **Step 2**: Following the selection of relevant compounds, data for around 1000 of
these compounds were downloaded from PubChem. The data was extracted
in CSV format, encompassing various fields such as Compound ID, ISOSMILES,
Canonical SMILES, and other pertinent chemical properties. 

- **Step 3**: Given the project's emphasis on developing accurate solubility
prediction models, the analysis was narrowed to concentrate solely
on the ISOSMILES data. 

- **Step 4**: To streamline the dataset for more efficient analysis, all fields except 
for ISOSMILES were removed. The resulting dataset comprised solely of 
ISOSMILES strings, each representing the stereochemical configuration of a compound.

- **Step 5**: The ISOSMILES strings where verified in terms of formatting thereby preparing
the dataset for prediction.

- **Step 6**: With the ISOSMILES strings validated and necessary corrections made, 
the cleaned strings where then compiled into a cohesive dataset 
ready for use in predictive modeling.



