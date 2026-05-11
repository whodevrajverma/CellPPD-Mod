# CellPPD-Mod: Prediction of Cell-Penetrating Potential of Modified Peptides Containing Natural and Chemically Modified Residues


**CellPPD-Mod** is an advanced computational resource designed to predict the cell-penetrating potential of peptides that contain both natural and chemically modified residues.
While most existing tools are restricted to peptides composed of the 20 standard amino acids, CellPPD-Mod addresses a critical gap in the field by accounting for the diverse chemical modifications—such as non-natural residues,
D-amino acids, and fatty acid attachments—commonly used to enhance the stability and delivery efficiency of therapeutic peptides.

**Web Server:** https://webs.iiitd.edu.in/raghava/cellppdmod/


## Citation

Kumar, V., Agrawal, P., Kumar, R., Bhalla, S., Usmani, S. S., Varshney, G. C., & Raghava, G. P. S. (2018).
**Prediction of Cell-Penetrating Potential of Modified Peptides Containing Natural and Chemically Modified Residues.** *Frontiers in Microbiology*, 9:725.
https://doi.org/10.3389/fmicb.2018.00725

This project is also available on Zenodo at https://doi.org/10.5281/zenodo.20117230


## About the Research

Chemical modifications are often essential to prevent the rapid degradation of peptides by proteases in the body. However, these modifications can significantly alter a peptide's ability to cross cell membranes.
CellPPD-Mod provides a systematic method to evaluate these "hybrid" sequences.

* **Extensive Dataset:** The models were developed using a comprehensive dataset of **1,273 modified peptides** (949 CPPs and 324 non-CPPs) curated from the CPPsite 2.0 database.
* **Chemical Diversity:** The dataset includes peptides with various modifications, including D-amino acids, unusual amino acids, and terminal modifications like acetylation or amidation.


## Key Features

### 1. Handling Chemically Modified Residues

* **MOL2 and SMILES Integration:** The tool utilizes structural information from MOL2 files to represent modified residues, allowing the model to "understand" the chemical nature of non-natural components.
* **Molecular Descriptors:** Computes nearly 50 physicochemical and structural descriptors for both natural and modified residues.

### 2. Robust Machine Learning Models

* **Algorithms:** Employs Support Vector Machine (SVM) and Random Forest classifiers.
* **Performance:** The best-performing model achieved a maximum **accuracy of 89.10%** and an AUROC of 0.94 on a validation dataset.
* **Feature Importance:** Identified that properties such as hydrophobicity and the presence of specific cationic modifications are key drivers of penetration potential in modified sequences.

### 3. Integrated Web Services

* **Prediction Module:** Users can submit sequences containing natural and modified residues (using specific notation for modifications) to predict their translocation efficiency.
* **Analog Design:** Facilitates the "in silico" optimization of peptides by testing the impact of different chemical modifications on their cell-penetrating score.
* **Comprehensive Documentation:** The server provides a clear mapping of available chemical modifications and the specific codes required for submission.



## Applications

* **Peptide Drug Development:** Optimizing the design of metabolically stable, modified peptide carriers for intracellular drug delivery.
* **Therapeutic Engineering:** Refining the sequence of antimicrobial or anticancer peptides to ensure high cellular uptake without compromising biological activity.
* **Pharmacokinetics:** Screening modified leads for their potential to overcome biological barriers.



## Contact & Authors

**Prof. Gajendra P. S. Raghava** (Corresponding Author)

raghava@iiitd.ac.in

Department of Computational Biology, Indraprastha Institute of Information Technology (IIIT Delhi), New Delhi, India.


## Support

The development of CellPPD-Mod was supported by the **Department of Biotechnology (DBT)** and the **Council of Scientific and Industrial Research (CSIR)**, Government of India.
