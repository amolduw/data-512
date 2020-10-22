
# Human Centered Data Science (Data-512-A2 - Bias in Data)

## Purpose of project:
The purpose of this project is to analyze <a id="https://meta.wikimedia.org/wiki/Research:Detox/Data_Release">Wikipedia talk corpus </a>, to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven app
ations. Google used Wikipedia Talk corpus used to train machine learning models for a project called [Conversation AI](https://conversationai.github.io/). Each dataset contains thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.  


## Analysis:  
I woulk like to analyze and find potential bias in data (if exists) and understand implications of bias on machine learning models.
- How does demographic profiles of crowworkers affect in consistency of labelling behaviours in toxicity hostile speech?  
- What words are more associated with comments labelled as hostile speech?

I used two datasets toxicity & aggression for the analysis. I also referred Perspective Hacks gallery for deeper analysis. 

## Data Source
1. [Toxicity Datasets](https://figshare.com/articles/Wikipedia_Talk_Labels_Toxicity/4563973)
2. [Agression Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550)
3. [Perspective Hacks Gallery](https://github.com/conversationai/perspectiveapi/wiki/perspective-hacks)

## Terms of use
Terms of use and detailed research is available at [Detox - Wikimedia](https://meta.wikimedia.org/wiki/Research:Detox).

## Directory Structure
```bash
├── plots
├── data
├── hcds-a2-data-bias.ipynb
├── ReadMe.md
├── LICENSE

```

## Requirements
[Python v3.x](https://www.python.org/)
[Seaborn latest version](https://seaborn.pydata.org/index.html)

## Findings:
We have discussed findings at detail in notebook. Below is summary.
- We found there is inherent participation bias in annotation worker population by different dempgraphic dimensions such as age_group, gender, eduation, english_first_language etc. 
- We further found that the set of annotations both across aggression and toxicity has skewed distribution by various dempgraphic attributes. Hence both of these datasets has bias built in it. 
- Before using this data in machine learning algorithms, appropriate steps should be taken to balance the dataset and to take into account population demographic imbalance. 

## Visualizations

Some of the analysis visuals are shown below for quick reference.

### Aggression annotation workers demographic distribution:
![Aggression annotation workers demographic distribution](https://github.com/amolduw/data-512/blob/main/data-512-a2/plots/Aggression%20annotation%20workers%20demographic%20balance.png)

### Aggression annotations distribution by annotation worker demographic:
![Aggression annotations distribution by annotation worker demographic](https://github.com/amolduw/data-512/blob/main/data-512-a2/plots/Aggression%20annotations%20demographic%20distribution.png)

### Distribution of mean aggression score by annotation workers age group:
![Distribution of mean aggression score by annotation workers age group](https://github.com/amolduw/data-512/blob/main/data-512-a2/plots/Distribution%20of%20workers%20mean%20aggression%20rating%20by%20age%20group.png)

### Distribution of mean toxicity score by annotation workers education:
![Distribution of mean toxicity score by annotation workers education](https://github.com/amolduw/data-512/blob/main/data-512-a2/plots/Distribution%20of%20workers%20mean%20toxicity%20rating%20by%20education.png)

### Word cloud for words considered Toxic but not Aggressive:
![Word cloud for words considered Toxic but not Aggressive](https://github.com/amolduw/data-512/blob/main/data-512-a2/plots/Word%20Cloud%20for%20Toxic%20comments%20that%20are%20not%20considered%20Aggressive.png)
  
## License
This project is available under the [MIT License](https://github.com/amolduw/data-512/blob/main/data-512-a2/LICENSE)

