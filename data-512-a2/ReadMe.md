
# Human Centered Data Science (Data-512-A2 - Bias in Data)

## Purpose of project:
The purpose of this project is to analyze <a id="https://meta.wikimedia.org/wiki/Research:Detox/Data_Release">Wikipedia talk corpus </a>, to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven app
ations. Google used Wikipedia Talk corpus used to train machine learning models for a project called [Conversation AI](https://conversationai.github.io/). Each dataset contains thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.  


## Analysis:  
I woulk like to analyze and find potential bias in data (if exists) and understand implications of bias on machine learning models.
- How does demographic profiles of crowworkers affect in consistency of labelling behaviours in toxicity hostile speech?  
- What words are more associated with comments labelled as hostile speech?

I used two datasets hostile speech - toxicity & aggression for the analysis. 

## Data Source
1. [Toxicity Datasets](https://figshare.com/articles/Wikipedia_Talk_Labels_Toxicity/4563973)
2. [Agression Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550)

## Terms of data use
[Wikimedia](https://foundation.wikimedia.org/wiki/Terms_of_Use/en) Terms of use

## Directory Structure
```bash
├── plots
├── data
├── data-512-a2.ipynb
├── ReadMe.md
├── LICENSE

```

## Requirements
[Python v3.x](https://www.python.org/)

## Visualizations


  
## License
This project is available under the [MIT License](https://github.com/amolduw/data-512/blob/main/data-512-a2/LICENSE)

