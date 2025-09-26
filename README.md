# Collision Risk Classification in Orbit Using SVM and Ensemble Techniques: A Pipeline for the Automatic Identification of High-Risk Events in CDM Messages

This work was carried out as part of a curricular internship at the **Italian Space Operations Command (COS)**, in collaboration with **Sapienza University of Rome**.  
The project focused on developing a predictive system based on **machine learning techniques**, capable of estimating, at least two days in advance, the final collision risk associated with each conjunction event in Low Earth Orbit (LEO), using only the information contained in **Conjunction Data Messages (CDM)**, the standardized messages describing the orbital conditions of the two objects involved.  

For performance evaluation, the project adopted the official datasets and metrics of the **Spacecraft Collision Avoidance Challenge**, organized by the **European Space Agency (ESA)** in 2019.  

After a general overview of the problem and the algorithms explored, the thesis provides a detailed description of the final classification pipeline: a multilayer system, based on a modular architecture and an ensemble of models.  
At its core, the pipeline relies on **56 Support Vector Machines (SVMs)**, coordinated through voting and consensus mechanisms to identify reliably classifiable events. Uncertain cases are handled by subsequent stages, which employ specialized classifiers trained on targeted subsets of the dataset.  
In parallel, a regression module was developed to provide a continuous risk estimate for events classified as high-risk. 

The integration of the two models was tested on the official dataset of the ESA Spacecraft Collision Avoidance Challenge (2019), using the same evaluation metrics defined by the competition. Although this work did not participate in the Challenge itself, the obtained **score of 0.559** can be directly compared with the official leaderboard: it corresponds to the **2nd best overall result among 97 teams**, and the best result among all approaches entirely based on machine learning techniques.

---

## References

For further information on the **Spacecraft Collision Avoidance Challenge (2019)**, see:  
Thomas Uriot et al. “Spacecraft collision avoidance challenge: Design and results of a machine learning competition”. In: Astrodynamics 6.2 (2022), pp. 121–140. doi: 10.1007/s42064-021-0101-5.

---

## Repository Contents

- **Full Thesis (PDF, in Italian)**: a complete description of the work, including:
  - Problem formulation
  - Machine Learning models tested and employed
  - Results and evaluation metrics (F2, Recall, FPR, MSEHR, final score)
  - Graphs and result tables
  - Pseudocode and detailed model explanations  

**NOTE**: The thesis document is written in Italian. However, graphs, tables, and pseudocode are in English, making the technical content accessible to non-Italian speakers.  

---

## Code Availability

The original code used for experiments is **not publicly available** due to privacy and intellectual property reasons.   Nevertheless, all methodological details, model designs, and results are fully documented in the thesis (PDF).  

---

## License

This repository is intended for academic and informational purposes.  
All materials are the intellectual property of the author and may not be copied or redistributed without permission.  

---


