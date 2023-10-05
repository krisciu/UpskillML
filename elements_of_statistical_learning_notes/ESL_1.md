# Elements of Statistical Learning
## Chapter 1

### Statistical Learning Examples
- Predict P(Patient has a second heart attack | Patient has already had a heart attack) given:
  - Demographics
  - Diet
  - Clinical measurements

- Predict stock price given:
  - Company performance measures
  - Economic data

- Parse handwriting -> text

- Estimate amount of glucose in blood given infrared absorption spectrum of blood

- Identify P(prostate cancer) given:
  - Clinical and demographic variables


### Core Ideas
- Some `outcome`:
  - Quantitative (e.g., Stock price)
  - Categorical (heart attack/ no heart attack)

- Based on `features`:
  - e.g., Diet, measurements

- We have a `training set`:
  - Known set of features and outcome

- Use above to build `learner`:
  - A model that can predict the outcome given the training set

This process is known as `supervised learning`.
- It is called `supervised learning` because we can use known values to teach our learning.

Other type of learning known as `unsupervised learning`.
- We only have the features, no known outcome.
- We have to describe how the data is clustered.


### Some Examples

#### Spam Detector

Goal:
- Build an automatic spam detector

Features:
- 4601 email messages

Outcomes:
- Labels `email` and `spam` on features

This is a classic example of a `classification` problem.
- More specifically, a `binary classification` problem [spam OR email].



#### Prostate Cancer [Oh boy!]

Goal:
- Predict log(prostate specific antigen) given measurements

Features [Lots]:
- Log cancer volume
- Log prostate weight
- Seminal vesicle invasion [Eww, I don't want to know what this is]
- Tons more

Outcomes:
- Not stated but a scatterplot is provided

This is an example of a `regression problem` as the outcome measurement is quantitative.


#### Handwritten Digit Sorter

Goal:
- Given handwritten zip codes, parse the text

Features:
- Set of 16x16 8-bit grayscale maps

Outcomes:
- Not specified

This is a `classification` problem, where we need a low error rate.
In order to accomplish this, we can classify some as `don't know`.


#### DNA Expression Microarrays

Goal:
- Map gene expression data to uncover similarities between tumor samples and genes

Features:
- Heatmap of expression levels of each gene versus samples, with 6830 genes and 64 samples

Outcomes:
- None given

This is an example of an `unsupervised learning` problem, as we are trying to assess:

a. Which samples are most similar in terms of expression profiles across genes?

b. Which genes are most similar in terms of expression profiles across samples?

c. Do certain genes show high or low expression for certain cancer samples?

We want to find these naturally occurring clusters.












