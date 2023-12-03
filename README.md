# MedCare Wellness Research Center

### Team Members
- Edoardo Cocciò 282401
- Alexandra Tabarani 282091
- Lorenzo Laterza 283121


## Introduction
*At MedCare Wellness Research Center, we embark on a groundbreaking journey to predict the physical health of individuals using an extensive dataset encompassing 261,311 records.* Our ambitious project stands out in its scale and depth, delving into an array of factors that influence our physical health. The dataset is a rich tapestry of information, featuring a diverse range of attributes from physical and mental health assessments to lifestyle indicators such as exercise habits, sleep patterns, and smoking status. Notably, it comprises a higher proportion of categorical variables (13 in total) compared to numerical ones (5), including the unique PatientID for each individual.

*Our approach is rooted in the OSEMN framework*, a robust and systematic pipeline that includes obtaining, scrubbing, exploring, modeling, and interpreting data. This comprehensive methodology ensures a meticulous and thorough analysis of the dataset. A key component of our project is an in-depth Exploratory Data Analysis (EDA), designed to uncover hidden patterns and insights, and visualizing our data. This step is crucial as it lays the foundation for subsequent phases of our research.

*Beyond EDA, our project extends into the critical realm of data preprocessing and model evaluation.* This phase is fundamental in transforming our extensive dataset into a form that's primed for effective machine learning analysis. Key preprocessing steps include meticulous scaling and encoding, tailored specifically to suit the unique composition of our dataset. It's a process that not only prepares the data but also enables us to uncover and understand latent patterns and relationships, which are crucial for boosting the performance and predictive accuracy of our target variable.

*Our approach is characterized by a rigorous experimentation with a variety of machine learning models.* This phase is not just about applying algorithms; it's about a meticulous and iterative process of fine-tuning each model to achieve optimal performance. We thoroughly test various models, adjusting and calibrating them to hone in on the most effective techniques for predicting physical health outcomes. 

## Methods




## Experimental design

Our project's experimental design was methodically organized into two distinct phases, each pivotal in assessing the influence of data preprocessing on the performance of various predictive models.

*Phase One: Baseline Model Evaluation*
The initial phase focused on evaluating a suite of predictive models using the original, unmodified dataset. The primary objective here was to establish baseline benchmarks. This was crucial for understanding the initial predictive capabilities of each model and observing how they interacted with the complexities of our dataset. This phase served as the foundation for comparison in our subsequent analysis.

*Phase Two: Impact of Refined Data Preprocessing*
In the second phase, the same set of models was reassessed, but this time on a dataset that had undergone extensive preprocessing. The aim was to measure the effect of this refined data treatment on model performance, offering a comparative analysis against our established baselines.

*Model Selection and Rationale*
- *Linear Regression*: Implemented only in the second phase due to its sensitivity to outliers and non-linearities. The original dataset's extreme skewness made it challenging to glean meaningful interpretations from this model initially.
- *Decision Trees*: Chosen for their capacity to model non-linear relationships, offering insights into the dataset's complex structure.
- *Random Forest*: Selected for its ability to mitigate overfitting issues seen in decision trees, thereby enhancing accuracy.
- *Hist Gradient Boosting*: Preferred for its efficiency in handling large datasets and its adeptness in managing missing values. 

Each model was meticulously tuned to ensure optimal performance, taking into account the unique characteristics of our dataset.

*Evaluation Metrics: Precision in Measurement*
Our choice of evaluation metrics was guided by the need for accuracy and relevance in a regression setting:
- *Mean Absolute Error (MAE)*: Chosen for its straightforward representation of the average error magnitude, offering a direct understanding of model accuracy.
- *Mean Squared Error (MSE)*: Utilized for its ability to highlight larger errors, a critical aspect when assessing model reliability.
- *R-squared (R^2)*: Employed to quantify the percentage of variance in the 'Physical Health' score that our models could explain, providing a measure of the models' explanatory power.

Through this structured and meticulous experimental design, we aimed to not only assess the performance of various models under different conditions but also to understand the deeper impacts of data preprocessing on our predictive capabilities.


## Results

In the first phase of our project, where we utilized the initial dataset, the results from our models indicated a modest level of predictive ability. Notably, the Hist Gradient Boosting model struck a balance between performance complexity and accuracy. This was evidenced by its Mean Absolute Error (MAE) and R-squared values, which pointed to a reasonable, yet not exceptional, level of accuracy and ability to explain the variance in the dataset.
These initial findings were pivotal as they brought to light the critical need for model tuning. The moderate performance across the board suggested that while our models were on the right track, there was significant room for improvement, especially in terms of enhancing their predictive capabilities. This was particularly evident in their limited success in capturing the full spectrum of variance within our complex dataset.
The results from this phase underscored an important insight: a more selective approach in data preprocessing could potentially lead to better model performance. It became clear that fine-tuning our models and perhaps even adopting a more targeted selection of the data could yield more accurate and reliable predictions. This understanding guided our next steps, where we would delve deeper into optimizing our models and exploring the impact of refined data selection on their performance.

![Alt text](models_completedf.png)

Upon revising the dataset to exclude potential filling values, we embarked on the second phase of our model evaluation. This step involved a re-assessment of the models with the newly refined dataset, leading to notably enhanced performances. 
This phase marked a clear improvement in accuracy and reliability across all models, as evidenced by reduced Mean Absolute Error (MAE) and increased R-squared values. These metrics were especially pronounced in the performance of the Hist Gradient Boosting model, which emerged as the standout performer. The enhanced dataset allowed this model to excel, showcasing its superior capability in predicting physical health outcomes.
The positive outcomes of this phase reinforced the value of our data cleaning and refinement process. It became evident that our approach to data selection and preprocessing was instrumental in elevating the predictive power of our models. This phase not only demonstrated the overall improvements in model performance but also highlighted the proficiency of the Hist Gradient Boosting model in our refined context.

![Alt text](models_df.png)


## Conclusions

In this group project, we had the invaluable opportunity to apply and refine our practical knowledge in the field of predictive modeling for healthcare data analysis. This experience allowed us to delve deep into the complexities of working with real-world health data, developing our understanding and skills in data preprocessing, model selection, tuning and interpretation of the results.
This experience was not just about applying theoretical knowledge; it was a practical foray into the intricacies of real-world data and the subtleties of model behavior. We emerged from this project with a refined understanding of how data tells a story in the healthcare context and how our role is pivotal in interpreting and presenting this narrative.

Yet, as with any rigorous scientific inquiry, our project opened doors to new questions and paths for exploration. We made significant headway in improving model accuracy, yet some aspects of physical health prediction remain not fully uncovered. 
Looking forward, there's a promising avenue in enhancing our approach to filtering out potential filler values. By refining this filtering process, we anticipate uncovering deeper, more subtle patterns within the dataset, potentially leading to further breakthroughs in predictive accuracy. Future endeavors could involve a more intricate analysis of these aspects, possibly integrating more nuanced data points or employing advanced modeling techniques that can better capture the complex tapestry of factors influencing physical health.

In wrapping up our work with the MedCenter dataset, it's like we've been doctors using data to understand people's health. Just like doctors use symptoms to figure out what's wrong with someone, we used data to predict how healthy people might be!

Our project showed how important data analysis is in healthcare. We used machine learning to find patterns in the data, which helped us understand how different things affect people's health. It's like using a stethoscope to listen to someone's heart, but we were listening to the data.

In conclusion,  this project was more than an academic endeavor; it was a step into the future, demonstrating the incredible potential of technology in healthcare. Our findings lay the groundwork for future research, offering a glimpse into a world where healthcare is driven by data, tailored to individual needs, and more proactive in preventing illness!
