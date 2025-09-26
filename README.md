# Collision Risk Classification in Orbit Using SVM and Ensemble Techniques: A Pipeline for the Automatic Identification of High-Risk Events in CDM Messages 

## Abstract:
Master’s thesis carried out at the Italian Space Operations Command (COS) in collaboration with Sapienza University.
Developed an ensemble ML pipeline for predicting collision risk in Low Earth Orbit from Conjunction Data Messages (CDM).
Core system based on 56 SVMs with modular architecture and voting mechanisms, plus a regression module for risk estimation.
On the official ESA dataset, the pipeline achieved a score equivalent to 2nd place among 97 teams in the 2019 ESA Collision Avoidance Challenge.
The thesis provides full methodological details, pseudocode, and results (code not publicly available).

--- 

## Project Overview
This thesis was developed during a curricular internship at the Italian Space Operations Command (COS), in collaboration with Sapienza University of Rome.
The project aimed to design a predictive system capable of automatically estimating the final collision risk of Low Earth Orbit (LEO) conjunction events, at least two days in advance, using only the information contained in standardized Conjunction Data Messages (CDM).

The system was implemented in Python, combining multiple libraries and frameworks:
   - **PyTorch** for prototyping neural components and optimization routines
   - **scikit-learn** for preprocessing, classical ML models, and evaluation metrics
   - **numpy/pandas** for efficient data handling and numerical computation
   - **matplotlib/seaborn** for visualization and result analysis

The final pipeline adopts a multi-layer modular architecture:
   - 56 Support Vector Machines (SVMs) coordinated through voting and consensus strategies
   - Specialized classifiers to handle uncertain or borderline events
   - A regression module for continuous risk estimation of high-risk cases

For performance evaluation, the system was tested on the ESA Spacecraft Collision Avoidance Challenge (2019) dataset, following the official competition metrics.
Although this work did not directly participate in the Challenge, the obtained score of 0.559 corresponds to the 2nd best overall result among 97 teams, and the best result among all machine learning–only approaches.

---

## References

For further information on the **Spacecraft Collision Avoidance Challenge (2019)**, see:  
Thomas Uriot et al. “Spacecraft collision avoidance challenge: Design and results of a machine learning competition”. In: Astrodynamics 6.2 (2022), pp. 121–140. doi: 10.1007/s42064-021-0101-5.

---

## Repository Contents

**Full Thesis (PDF, in Italian)**: a complete description of the work, including:
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