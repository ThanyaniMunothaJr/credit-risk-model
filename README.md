# credit-risk-model
This is a credit risk modelling framework for Probability of Default estimation and expected loss.

## 1. Credit Risk Framework & Modelling Scope
This project implements a credit risk modeling framework aligned with standard banking practice and regulatory concepts. The objective is to estimate Expected Credit Loss (ECL) for a portfolio of unsecured retail loans by modeling its key risk components.

Credit risk is decomposed as:

###    Expected Loss (EL) = PD × LGD × EAD


where:

PD (Probability of Default) represents the likelihood that a borrower defaults within a fixed time horizon,

LGD (Loss Given Default) represents the proportion of exposure lost conditional on default,

EAD (Exposure at Default) represents the outstanding exposure at the time of default.

The primary focus of this project is the estimation of 12-month PD using an interpretable statistical model. LGD and EAD are treated as secondary components and are incorporated through simplified assumptions for the purpose of computing Expected Loss.

Definition of Default

A default event is defined as a loan that becomes 90 or more days past due or is classified as charged off within a 12-month observation horizon following loan origination.

Modeling Horizon

All PD estimates are produced on a 12-month horizon, consistent with regulatory credit risk frameworks such as Basel II/III and IFRS 9.

Modeling Approach

Probability of Default is modeled using logistic regression, selected for its interpretability, stability, and widespread use in banking credit risk applications. Model assumptions, estimation procedures, and validation techniques are documented separately.

Scope and Limitations

This project is intended as an educational implementation of a credit risk model and does not constitute a production or regulatory-approved model. The framework emphasizes transparency, statistical reasoning, and alignment with industry practice.
