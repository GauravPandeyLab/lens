Release lens2.0 incorporates diversity into the RL framework to enable the selection of more accurate and parsimonious ensembles. This version builds upon the previous version of lens (https://github.com/GauravPandeyLab/lens-2017), and follows the same basic design. Diversity is calculated between pairs of current and potential future state ensembles during reinforcement learning (RL) search. The potential future ensemble that has the highest value of the diversity measure, i.e., is the most diverse with respect to the current ensemble, is the next state of the agent during the exploration phase of the RL process.

The diversity measures implemented are:
- diversity measures based on Pearson's correlation coefficient, cosine similarity, and Euclidean distance (unsupervised)
- Yule's Q [1] and Fleiss' kappa [2] (supervised)

Notes:
- The implementation in intended to run batch jobs on hpc clusters and was developed on Minerva (https://labs.icahn.mssm.edu/minervalab/).
- In <path>/RL, <path> to be replaced with corresponding location.
  
REFERENCES

[1] T. G. Dietterich, “An Experimental Comparison of Three Methods forConstructing Ensembles of Decision Trees: Bagging, Boosting, and Randomization,” Machine Learning, vol. 40, no. 2, pp. 139–157, 2000.
[2] G. U. Yule, “On the Association of Attributes in Statistics: With Illustrations from the Material of the Childhood Society,” Philosophical Transactions of the Royal Society of London, Series A, vol. 194, pp.257–319, 1900.
