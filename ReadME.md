## Aqueous Kinetic Solubility Model Validation

This project uses the Aqueous Kinetic Solubility model from Ersilia 
Hub to predict the solubility of 1000 compounds sourced from public 
repositories. The model, identified by its EOS model ID `eos74bo`.

## Data Collection and Preparation 

This project required a dataset of chemical compounds for analysis. 
The following steps outline how the data was selected and prepared;
this dataset was collected from PubChem, one of the most comprehensive
chemical databases available.

- Searched for compounds on PubChem based on the project's specific criteria, that compounds data that contain ISOSMILES.
- Downloaded `1000` compound data from PubChem, including fields such as Compound ID, ISOSMILES, Canonical SMILES, among others, in CSV format.
- Focused on ISOSMILES for analysis due to its inclusion of stereochemical information for solubility prediction models.
- Removed all fields except for ISOSMILES from the dataset.
- Verified the formatting and validity of the ISOSMILES strings to ensure they represented accurate chemical structures.
- Compiled the cleaned ISOSMILES strings into a final dataset, ready for predictive modeling.

