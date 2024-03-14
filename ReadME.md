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

## Results
A scatter plot was used to visualize the predicted outcomes for the solubility
of compounds, ranging between `0.0` and `1.0`, against their indices in the dataset,
which span from `0` to `1000`. The predicted outcome values suggest a probability
score with `0.0` indicating a low probability of the compound being soluble 
and `1.0` indicating a high probability of solubility.

- **Compounds with Low Predicted Solubility**: A noticeable number 
of compounds had predicted outcomes at `0.0`, indicating that the
model identifies these compounds as having a very low probability of being soluble.

- **Moderate Predictions**: Some compounds were scattered around
`0.1` and `0.2` regions suggesting a slightly higher, yet still low,
probability of solubility. 

- **Varied Predictions**: Fewer compounds were scattered across the middle 
range of the plot, between `0.4` and `0.8`; suggesting that a smaller 
portion of the dataset possess characteristics that the model 
interprets as indicating moderate to high solubility.

- **Highly Soluble Predictions**: Some compounds were aligned exactly at
`1.0`, suggesting the model is very confident in their high solubility.
This extreme confidence might stem from specific molecular signatures 
that strongly indicate solubility, based on the model’s training data.


