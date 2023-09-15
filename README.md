# Exploring methods to identify proxy variables
Read the project paper [here](Final_Project_Report.pdf).

Proxies are features of a dataset that can serve as indicators or substitutes for removed demographic attributes and can contribute to algorithmic discrimination within a machine learning model. In this project, we demonstrate four methods to identify proxies of demographic features: Pearson’s correlation, pairwise Cramer’s V, feature combinations, and feature redundancy (using FACET).

Pearson’s correlation coefficient is suitable in identifying linear relationships between continuous variables, while Cramer’s V is more appropriate for evaluating relationships between categorical variables. However, both methods are limited in that they only analyze pairwise relationships and do not take into context the contribution of each feature on the model output.

To account for the former, we demonstrate how combinations of features could also function as proxies, especially when used in non-linear models. To maximize effectiveness, we propose a sequence of a correlation-based method, followed by an evaluation of feature combinations. To account for the latter, we also demonstrated a simplified evaluation of feature redundancy using the FACET library, which generates a redundancy matrix using SHAP values.

While these four methods together serve as a practical tool for proxy detection and feature evaluation, this project contributes to the larger goal of ensuring that AI-based systems adhere to the Algorithmic Discrimination Protections principle of the AI Bill of Rights, promoting fairness and mitigating discrimination in automated decision making systems.

_This project was done as part of Brown University's Fairness in Automated Decision Making Systems (CSCI 1951Z) course, under the advice of Prof Suresh Venkatasubramanian._
