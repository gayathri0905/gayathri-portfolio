# Gayathri Venkat

# Data Scientist

### Education
MS in Data Science

### Work Experience
#### Data Scientist @ Tensor Data Scientists
##### Key projects 
    - Customer segmentation model.
    - Recommendation systems.
    - Customer churn prediction.

##### Description
    - Developed and implemented a machine learning-based customer segmentation model to enhance targeted marketing efforts and improve customer satisfaction.

##### Key Achievements
    - Achieved a 20% increase in email campaign conversion rates by delivering personalized content to segmented customer groups.
    - Reduced customer acquisition costs by 15% through more efficient advertising spend allocation based on segmentation insights.

##### Technologies Used
    - Python, pySpark, Azure databricks, scikit-learn, pandas, SQL, Tableau

##### Challenges Faced
    - Addressed issues related to data quality and feature engineering to ensure accurate segmentation.
    - Addressed issues related to imbalanced data and feature selection to improve model performance.

##### Lessons Learned
    - Gained valuable insights into customer behavior and preferences, leading to more effective marketing strategies.

##### Impact
    - The project resulted in improved marketing ROI and customer engagement, contributing to a 18% increase in customer conversions.


#### Solutions Engineer @ Sonline  LLC
##### Key projects
    - Scalable search systems. 
    - Search Engine Optimization.
    - Ranking Systems.
    
##### Description 
    - Designed and implemented a scalable search system to enhance search speed and efficiency for a high-traffic platform.
    
##### Key Achievements 
    - Improved search response time by 30%, resulting in a significantly enhanced user experience. 
    - Implemented horizontal scaling techniques, allowing the system to handle a 50% increase in concurrent search queries. 
    - Reduced infrastructure costs by 20% through optimized resource allocation and utilization. 
    
##### Technologies Used 
    - Java, Python, Elasticsearch, AWS (EC2, S3), Docker 

##### Challenges Faced 
    - Addressed indexing bottlenecks and optimized query processing to achieve performance improvements.
    - Optimizing high-traffic systems, with a focus on scalability and performance. 

##### Impact 
    - The project led to a notable increase in user satisfaction and engagement, contributing to a 15% rise in conversion rates for search-driven sales. 

### Projects

#### Ice Hockey Tournament

![](/Images/ice_hockey_game.gif)

In this project, I built a SuperTuxKart ice hockey agent based on supervised learning approach. In this game, our hocket agent plays against an AI agent with a game session of two minutes per round.  To win the game our agent have to score more goals than the opponent AI agent within two minutes. Explored two approaches: 1. Dagger based imitation learning; 2. Supervised learning approach based on vision and control. Final implementation was using the supervised learning approach because it gave better results compared to the Dagger method. I trained a deep network, with an average score 2-0 against the AI agent accorss different difficulty levels (Simple,Medium,Hard).
  
#### Self Driving Go-Kart Racer 

![](/Images/go_kart_racer.gif)

In this project, I built a racer kart that uses computer vision to drive in different terrains. This game was developed in the SuperTuxKart game environment.  This kart uses ONLY the camera screen images as its input to predict its trajectory of motion. I developed a fully convolutional network using a encoder-decoder structure with  batch normalization to process the input image and predicted an 'aim point'. This aim point is value which had x and y co-ordinate of the kart position to which the kart was supposed to drive, inorder to complete the race. And, I also implemented a controller which handled the steering, acceleration, braking and drifting of the kart based  on the predicted aim point.  

#### Question Answering System

Developed a question answering model that answers  questions based on passages from Wikipedia. This is my final project where I modified an existing neural question answering system and proposed an improved model which was able to identify answers better than the baseline model. I was given three main  datasets:  SQuAD (Rajpurkar et al., 2016), NewsQA (Trischler et al., 2017), and BioASQ (Tsatsaronis et al.,2015) to work with. 

![alt text](/Images/question_answering_system_using_SQuAD.png)

SQuAD asks questions about Wikipedia articles, NewsQA about news articles, and BioASQ about biomedical text.Furthermore, I also tested my model against the adversarial SQuAD data from Jia and Liang (2017). This data
adds sentences which look like the question but contain nonsense entities, and easily fool many pre-trained
SQuAD models. I implemeted a single model Bi-LSTM and trained it on the SQuAD dataset. The model showed between 5-6% improvement in performance on  both the SQuAD and Adversial SQuAD datasets. And, I did two minor changes to the baseline models:  1.Repositioning the attention  layers and 2. Fine tuning the hyperparameters.


![alt text](/Images/baseline_model_architecture.png)

![alt text](/Images/comparitive_performance.png)

![alt text](/Images/modified-attention-architecture.png)

![alt text](/Images/query2context_attention_implemetation.png)

#### Results

- The proposed model shows ~5% improvement in EM against the baseline.
- The  model is able to find answers for 'When' and 'Who' based questions. This is because these answers  are based on named entities with short context.
- Whereas, answers for 'Why' questions  require deep logical understanding of the context. The model struggles on questions based on 'why'.
- Thus the future scope of the project coulf be that, if we modify the model to better understand the context will help in improving the performance further.
- The aligned attention embedding layer which was implemented for a context-question pair clearly signifies the  prime context phrase/word that maps to the query word. For example, the word 'many' maps to the context words:'one','four','eight','appearances'.
- Then by drawing the probability mass for the start and end index of the prediction span we get the gold answer.
 
#### Device Predictive Maintenance

A company has a fleet of devices transmitting daily sensor readings. In this project, I created a predictive maintenance solution to proactively identify maintenance requirements and cadence.

- The predictive maintenance dataset had 124494 rows and 12 columns.
- The dataset was highly imbalanced with 106 unique failures and 124388 non failures.
- Applied SMOTE oversampling and RandomUnderSampler algorithms to handle the imbalance in the dataset.
- Used precision and recall as a performance metric to analyze my model.
- Calculated Precision-Recall Area Under Curve (AUC) score for differnt thresholds and evaluated the performance of the model.
- Used Logistic Regression as the baseline algorithm and other boosting algorithms such as, AdaBoost, GradientBoost for maintenance prediction.

#### Future Scope

- Implement different algorithms such as: OneClassSVM, IsolationForest algorithms.
- These algorithms are highly specialized in Anomaly detection. Unlike the regular supervised SVM, the one-class SVM does not have target labels for the model training process.
- Instead, it learns the boundary for the normal data points and identifies the data outside the border to be anomalies, which would work well for our dataset.

![](/Images/predictive_maintenance_results.png)






