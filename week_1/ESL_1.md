# Elements of Statistical Learning
## Chapter 1

### Statistical learning examples
- Predict P(Patient has a second heart attack | Patient has already had another heart attack) given
  - demographic
  - diet
  - clinical measurements

- Predict Stock price given
  - company performance measures
  - economic data

- parse handwriting -> text

- estimate amt of glucose in blood given infrad absoption spectrum of blood

- identify P(prostate cancer) given
  - clinical and demographic variables


### Core ideas
- some `outcome`
  - quantitative(ex: Stock price)
  - categorical(heart attack/ no heart attack)

- based on `features`
    - ex: diet, measurements

- we have a `training set`
  - known set of features and outcome

- use above to build `learner`
  - a model that can predict theoutcome given the training set

This process is known as `supervised learning`
- It is called `supervised learning`  because we can use known values to teach our learning

Other type of learning known as `unsupervised learning`
- we only have the features, no known outcome
- we have to describe how the data is clustered


### Some examples

#### Spam Detector

Goal
- build an automatic spam detector

Features
- 4601 email messages

Outcomes
- labels `email` and `spam` on features

This is classic example of a `classification` problem
- more specifically a `binary classification` problem[spam OR email]



#### Prostate cancer[oh boy!]

Goal
- predict log(prostate specific antigen) given measurements

Features[lots]
- log cancer volume
- log prostate weight
- seminal vesicle invasion[eww i don't want to know what this is]
- tons more

Outcomes
- not stated but a scatterplot is provided

This is an example of a `regression problem` as the outcome measurement is quantitative


#### Handwritten digit sorter

Goal
- Given handwritten zip codes, parse the text

Features
- set of 16x16 8bit grayscale maps

Outcomes
- not specified

This is a `classification` problem, where we need a low error rate
in order to accomplish this, we can classify some as `don't know`

#### DNA Expression microarrays

Goal
- Map gene expression data to uncover similarities between tumor samples and genes

Features
- Heatmap of expression levels of each gene versus samples, with 6380 genes and 64 samples

Outcomes
- none given

this is an example of an `unsupervised learning` problem, as we are trying to assess

a. Which samples are most similar in terms of expression profiles across genes?

b. Which genes are most similar in terms of expression profiles across samples

c. do certain genes show high or low expression for certain cancer samples?

we want to find these naturally occurring clusters












