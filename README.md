 Collaborators 
 1. Harsh Shukla - Shuklaharsh
 2. Harsh Athavale - hat359
 
 
 
 
 Emotion Classification in HINGLISH social media text using supervised Machine Learning Algorithms 


     Abstract 

The goal of this task is to classify the emotions of comments on social media platforms and particularly classify hate speech. For this, we examine a BiLSTM architecture with attention mechanism (BiLSTM-Attention) and try different dropout rates based on these two models. We then exploit an ensemble of these methods to give the final prediction which improves the model performance significantly compared with the baseline model.  

                

              

 

 

 

 

 

 

 

 

 Table of Contents 

 

    1.             Introduction 

                   1.1.   Motivation 

  

2.             Literature Review 

  

                    2.1.  Related Work 

                    2.2.  Outcome of Literature Review 

                    2.3.  Problem Statement 

                    2.4.  Research Objectives. 

  

3.             Methodology and Framework 

  

  3.1.  System Architecture 

      

  3.2.   Algorithms, Techniques etc. 

                    3.3.   Detailed Design Methodologies (as applicable) 

  

     4.  Work Done 

  

  4.1.   Details as required 

                    4.2.   Results and Discussion 

                    4.3.   Individual Contribution of project members (in case of group project) 

     5.Conclusion and Future Plan 

     6.References 

 

Introduction  

 

        1.1 Motivation  

 

Comments and tweets made on social media platforms in India are            predominantly made in hinglish.  

Although extensive work has been done in analysis of english tweets and comments, a new technique is needed to analyse hinglish data as it has no specific grammar rules and is made complex by variations due to geographical location, varied phonetics, spelling variation etc.  

That is why it is pivotal to do more research in the are of codemixed languages like hinglish. 

 

Literature Review  

 

      2.1 Related Work 

                  

Mathur et al.[1] introduced a novel HOT dataset for multiclass labeling of                                              offensive textual tweets in HindiEnglish code switched language. They also proposed the MIMCT model that uses multiple embeddings and secondary semantic features in a CNN-LSTM parallel channel architecture to outperform the baselines and naive transfer learning models. 

 

Al-Hassan et al.[2]  differentiated between the different anti-social 

behaviors which include (Cyberbullying, Abusive and offensive language, Radicalization and hate speech) and presented a comprehensive study on how text mining can be used in social networks. 

 

Singh et al.[3] presented various approaches to sentiment analysis for Hinglish code-mixed tweets. Two different system architectures were researched: a supervised classification model incorporating cross-lingual embeddings for English transliterated Hindi data and a transfer learning approach trained on English sentiment data and cross-lingual embeddings and applied to code-mixed data. They concluded that incorporating cross-lingual embeddings increases the performance from the baseline monolingual systems. 

 

Zhou et al[4]. presented a deep learning based approach for implicit emotion analysis task which can be seen as a classification task. They explored the LSTM model and BiLSTM model both equipped with attention mechanism using different dropout rates and leverage ensemble method to boost the classification performance 

 

 

          2.2. Outcome of Literature Review 

 

The literature helped in getting an overview of the whole process of emotion analysis and gave an insight into the work that has already been done. 

It also provided us with inspiration and a path to further work on this topic. 

 

      2.3. Problem Statement 

 

Emotion Classification in HINGLISH social media text using supervised Machine   Learning Algorithms 

 

      2.3. Research Objectives 

To gain insight on the topic and develop improved models for prediction.  

 

 

 

              

 

 

 

 

 

 

    3. Methodology and Framework 

   3.1.System Architecture 

  	 

We put forward two different models: one is CNN-BiLSTM which mainly consists of CNN and a BiLSTM layer  the other is BiLSTM-Attention which mainly consists of BiLSTM and attention mechanism. We have tried different dropout rates to get different classification results on each model. To further better the predictive performance, our final method employs an ensemble of these models, with a strategy called soft voting 

 

 

 

   3.2. Algorithms, Techniques . 

 

TF-IDF - The TF*IDF algorithm is used to weigh a keyword in any     

content and assign importance to that keyword based on the number of     

times it appears in the document 

 

              ●   Word2vec - Word2vec is a two-layer neural net that processes text by                         

vectorizing” words. Its input is a text corpus and its output is a set of      vectors: feature vectors that represent words in that corpus. While Word2vec  is not a deep neural network, it turns text into a numerical form that deep    neural networks can understand. 

  

LSTM - Long Short-Term Memory (LSTM) networks are a type of recurrent       

             neural network capable of learning order dependence in sequence          

             prediction problems. 

 

Ensemble - Ensemble methods is a machine learning technique that  

              combines several base models in order to produce one optimal predictive  

              model 

 

` 

3.3. Methodologies . 

Dataset Collection: 

●  A dataset of around 11998 comments is taken from Facebook. 

  

Data Preprocessing: 

●  In this step, all those words which don’t contribute to accuracy such as punctuations, numbers, stop words etc. are removed from the reviews. 

●  All the english comments are also removed and devanagari hindi  is transliterated to hinglish. 

 

 

Feature Generation: 

  	We have computed the feature matrix using : 

●       TF-IDF 

 

   	 

Classification: 

We have used following classifiers to predict the sentiment of each   

comment:: 

●       Bilstm 

●       Bilstm-Attention 

 

 

 

 

 

 

 4. Work Done  

 

4.1. Results 

 

On training the embedded matrix, which is obtained after processing with Word2Vec, 

with BiLSTM ad BiLSTM + attention  

 

68% accuracy was obtained with BiLSTM and 75% accuracy was obtained with BiLSTM + attention layer  

 

 

4.2 Individual Contribution of project members  

 

Harsh Athavale :  

                        Literature Review, Data extraction,feature extraction using HindiSenti        

                        Wordnet, Word2vec application, BiLSTM 

 

Harsh Shukla : 

Literature Review, Data pre processing, TfiDF, BiLSTM + attention, Comparing Word2Vec and Fasttext.   

 

 

   	 

 

 

 

 

 

 

5.   Conclusion and Future     

      Plans 

 

                      We have presented a deep learning based approach for implicit  

                      emotion analysis task which can be seen as a classification  

                      task. We explore BiLSTM model both equipped       

                      with attention mechanism using different dropout rates and   

leverage ensemble method to boost the classification   

performance. Experimental results demonstrate that our    

system is effective for this implicit emotion  

                                 classification task. As for future works, it can follow three  

directions. Firstly, we intend to try different ensemble methods      

like soft voting.We would like to combine TF-IDF vectors with   

embedding matrix for greater insight 

 

 

 

            

 

 

 

 

 

6. References 

 

1. Mathur P, Sawhney R, Ayyar M, Shah R. Did you offend me? Classification of Offensive Tweets in Hinglish Language. Proceedings of the 2nd Workshop on Abusive Language Online (ALW2). 2018; 

 

2. Al-Hassan, Areej & Al-Dossari, Hmood. (2019). DETECTION OF HATE SPEECH IN SOCIAL NETWORKS: A SURVEY ON MULTILINGUAL CORPUS. 83-100. 10.5121/csit.2019.90208.  

 

3. Singh P, Lefever E. Sentiment analysis for Hinglish code-mixed tweets by means of cross-lingual word embeddings. 4th Workshop on Computational Approaches to Code Switching, Proceedings. Marseille, France: European Language Resources Association (ELRA); 2020. p. 45–51. 

 

4. Zhou Q, Wu H. NLP at IEST 2018: BiLSTM-Attention and LSTM-Attention via Soft Voting in Emotion Classification. Proceedings of the 9th Workshop on Computational Approaches to Subjectivity, Sentiment and Social Media Analysis. 2018; 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 
