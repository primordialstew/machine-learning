# Machine Learning with Python
A daylong workshop from [District Data Labs][0]


## Workshop Materials
- [code repository][1] on GitHub
- [workshop forum][2] on Piazza
- [slides][3] on Slideshare


### Definitions
*instance*  a single data point or example composed of fields
*feature*   a quantity describing an instance
*dimension* one or more attributes that describe a property


### Models
_Model_ is an overloaded term. Here are some of its usages:

- *model family* describes, at the broadest level, the connection btw vars of
  interest
- *model form* specifies exactly how the variables of interest are connected
  (within the framework of the model family)
- *fitted model* is a concrete instance of the model form where all parameters
  have been estimated from data, and the model can be used to generate
  predictions

#### Instance Methods
Compare instances in data set with a similarity measure to find best matches
- suffers from curse of dimensionality
- focus on feature representation and similarity metrics between instances

E.g.
* k-Nearest Neighbors (kNN)
* Self-Organizing Maps (SOM)
* Learning Vector Quantization (LVQ)

*Curse of dimensionality* when you go from one dimension to a higher dimension,
distances increase. In instance-based approaches, greater distance between
instances increases computational cost.

#### Regression
Model relationship of independent variables X to dependent variable Y by
iteratively optimizing error made in predictions

E.g.
* Ordinary Least Squares
* 

#### Regularization Methods
Extend another method (usually regression) penalizing complexity (minimize
overfit)
- simple, popular, powerful
- better at generalization

E.g.
* Ridge Regression
* Lease Absolute Shrinkage & Selection Operation (LASSO)
* Elastic Net

#### Decision Trees
Model of decisions based on data attributes. Predictions are made by following
forks in a tree structure until a descision is made. Used for classification &
regression.

By artificially reducing complexity of your decision tree (making it shallower
e.g. to be easier to undestand), you can introduce a lot of variance.

E.g.
* Classification & Regression Tree (CART)
* Decision Stump
* Random Forest
* Multivariate Adaptive Regression Splines (MARS)
* Gradient Boosting Machines (GBM)

#### Bayesian
Explicitly apply Bayes' Theorem for classification and regression tasks.
Usually by fitting a probability function constructed via the chain rule and a
naive simplification of Bayse.

Naive Bayes != _Bayesian methods_, NB is only one Bayesian method.
Significantly, it assumes that variables are independent.

E.g.
* Naive Bayes
* Averaged One-Dependence Estimators (AODE)
* Bayesian Belief Network (BBN)


### Feature Space
refers to the _n_-dimensions where your variables live (


### Mappings
a mapping is a function _phi_ that adds a dimension to the feature space, e.g.
R^3 -> R^4


### Your task
Given a data set of instances of size _N_, create a model that is fit from the
data (built) by extracting features and dimensions. Then use that model to
predict outcomes...

1. data wrangling (normalization, standardization, imputing)
2. feature analysis/extraction
3. model selection/building
4. model evaluation
5. operationalize model


### Book reccomendations
Someone was asking Benjamin Bengfort for book recommendations:

- _Thoughtful Machine Learning_[4], Matthew Kirk (in Ruby; Python ver. pending)
- _Collective Intelligence_[5], Toby Segaran


## References
[0]: http://www.districtdatalabs.com/#view-courses
[1]: https://github.com/DistrictDataLabs/machine-learning.git
[2]: https://piazza.com/class/iksgl08u58i3h4?cid=1
[3]: http://www.slideshare.net/BenjaminBengfort/introduction-to-machine-learning-with-scikitlearn
[4]: http://shop.oreilly.com/product/0636920039082.do
[5]: 
