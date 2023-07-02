# Data Augmentation
 
The user has an option to augment only the subset of the data that was selected on the Feature Selection page or augment all the data. The user can select the augmentation algorithms to run. The following augmentation algorithms are available:
- SMOTE: Synthetic Minority Oversampling Technique. [Link](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)
- GANs: Generative Adversarial Networks.

After the augmentation algorithm is selected, the **Generate Data** button applies the selected algorithm to augment the data based on the default parameters of each algorithm. Once completed, the results of the algorithms can be examined by expanding the boxes. 

The user can also download the augmented data as a csv file by clicking the **Download** button.