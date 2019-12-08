PROJECT DESCRIPTION:

Prediction of electrical grid stability using Logistic Regression.


ALGORITHM DESCRIPTION:

Imported Logistic Regression Module from scikit-learn library.

Logistic regression, despite its name, is a linear model for classification rather than regression. Logistic regression is also known in the literature as logit regression, maximum-entropy classification (MaxEnt) or the log-linear classifier. In this model, the probabilities describing the possible outcomes of a single trial are modeled using a logistic function.
Logistic regression is implemented in LogisticRegression. This implementation can fit binary, One-vs-Rest, or multinomial logistic regression with optional 
l_1,l_2 or Elastic-Net regularization.
"lbfgs" solver has been used.
The “lbfgs” is an optimization algorithm that approximates the Broyden–Fletcher–Goldfarb–Shanno algorithm, which belongs to quasi-Newton methods. The “lbfgs” solver is recommended for use for small data-sets but for larger datasets its performance suffers. 
For more information about the module visit: https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression


DATASET DESCRIPTION:

The local stability analysis of the 4-node star system (electricity producer is in the center) implementing Decentral Smart Grid Control concept.


ATTRIBUTE INFORMATION:

11 predictive attributes, 1 non-predictive(p1), 2 goal fields:
1. tau[x]: reaction time of participant (real from the range [0.5,10]s). Tau1 - the value for electricity producer.
2. p[x]: nominal power consumed(negative)/produced(positive)(real). For consumers from the range [-0.5,-2]s^-2; p1 = abs(p2 + p3 + p4)
3. g[x]: coefficient (gamma) proportional to price elasticity (real from the range [0.05,1]s^-1). g1 - the value for electricity producer.
4. stab: the maximal real part of the characteristic equation root (if positive - the system is linearly unstable)(real)
5. stabf: the stability label of the system (categorical: stable/unstable)


DATASET WEBSITE:

https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+
