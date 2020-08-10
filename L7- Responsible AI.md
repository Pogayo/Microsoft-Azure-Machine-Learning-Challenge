**Lesson 7: Responsible AI**

# Chapter 2 - Modern AI: challenges and principles
## Why care about Responsible AI?
- **Increasing inequality**: Training data that is biased can promote inequality
- **Weaponization**: AI is being weaponized to improve vectors of attack in cybersecurity
- **Unintentional bias**: An advertising system accidentally showed an ad for high-income jobs to men more often than it showed the ad to women.
- **Adverserial attacks**: Your self driving car is fooled by someone who carefully applied a specially designed sticker to a stop sign.
- Killer drones: Defering the decision to kill or harm to a machine learning model
- **Deep fakes**: Enable the weaponization of misinformation and pose a serious threat to the reliability of news and media
- **Data poisoning**:Someone deliberately manipulates the public data used for model training.
- **Hype**: A lot of hype that drives totally unrealistic expectations
- **The butterfly effect**: An infinitesimally small change in the input to a model causes huge, poorly understood impact.

## Approaches to Resposible AI
1. Model explainability/interpretability: Ability to explain and interprate the outcomes of a model. Insights can be used to validate model behaviour and various hypothesis and ultimately build trust with beneficiaries.
There are two aspects:
    * **Global behaviour**: an explanation of how the model operates in general
    * **Specific predictions/local explanation**:understand why the model made a certain predictions for specific inputs
    
2. Fairness: investigating who might be harmed by the model.
    * Who is neglected?
    * Who is mis-represented
    
#Chapter 3: Microsoft AI principles
1. Fairness - AI systems should treat all people fairly
2. Reliability and safety -AI systems should perform consistently and minimize risk.
3. Privacy and Security - AI systems should protect people and their personal data.
4. Inclusiveness - AI systems should empower everyone and engage people
5. Transparency - AI systems should be understandable
6. Accountability -Algorithms and the people who write them should be responsible or answerable for their impacts.

Mnemonic - PARFIT
> Transparency and Accountability are the foundational principles. 

#Chapter 5: Model Transparency and Accountability

- Less Opaque/ easy to explain - Decision trees
- More opaque/ difficult to explain - Neural networks

Feature importance tells us how each input feature is important in contributing to the resulting predictions.
## Model explainability in Azure Machine Learning

Explainers: Used to explain models. There are 2 kinds:

###Direct explainers 
You use them when you know the specific tool that will be best for the job. Integrated into the Azure ML SDK and expose a common output format and API. You will choose a direct explainer based on your model type
- Model agnostic explainers: SHAP Tree explainer, SHAP Deep explainer
- Model specific explainers: Mimic explainer, SHAP Kernel explainer

##Meta explainers
Are used for automatic selection of direct explainers. Vary based on the type of data used for training
- Tabular explainer
- Text explainer
- Image explainer

#Chapter 8: Model Fairness

[Fairlearn](https://github.com/fairlearn/fairlearn): Toolkit to identify and mitigate unfairness in machine learning models
