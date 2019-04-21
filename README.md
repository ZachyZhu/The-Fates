# The-Fates(Game of Thrones)
The Fate – Game of Thrones
Data Report
https://github.com/ZachyZhu/The-Fates

produce by 
Love %s Every %s %(U,Day)

 




1.Abstract
Game of Thrones is quite hot recently, and Season Eight is coming. What is the fate of the eight main characters? We used the dataset of Game of thrones to predict whether they will be alive in the final season. To analyze the dataset, we used data visualization method. Then we trained the dataset with 6 machine learning models and then predict the death and probability of alive for the 8 main characters. In the end, we build a user graphical user interface (GUI) to predict the survival probability of you supposing you are in Westeros based your information you provided to us.


2.Installation
We used numpy, pandas, plotly, BeautifulSoup, nltk, networkx, sklearn and tkinter packages.
Thanks them :).


3.Main Features
3.1. data cleaning
We used two datasets, the main one is the dataset from Kaggle and another one is from github. (https://www.kaggle.com/mylesoneill/game-of-thrones) 
(https://github.com/mathbeveridge/asoiaf)
Our original dataset has 1946 piece of data and each for a character. There are 13 features and after cleaning we have 8 features left, for the culture feature and identity feature: we get them using web scraping and natural language processing methods 
(https://github.com/ZachyZhu/The-Fates/blob/master/Data_processing%20_final.ipynb):

Table 2.1 dataset information
features	type	values
male	binary	1 is male, otherwise 0
culture	string	Rivermen, Dornish, Braavosi….
house	string	House Targaryen, House Frey…
Book1-Book5	binary	1 if appears in this book
isMarried	binary	1 is married, otherwise 0
isNoble	binary	1 is noble, otherwise 0
numDead	integer	Integer values stands for number of dead relatives for this character
identity	string	King, knight, lord, official, noble, prince, warrior, smallfolk
isAlive	binary	1 the character is alive, otherwise dead












3.2.  data visualization
We used the amazing plot package(plotly) and wordcloud to visualize all the pictures, here are two samples of our visualization:
         
                     Figure 2.1 Number of alive and dead relative                                   Figure 2.2 Wordcloud for dead families


3.3. Text mining and data analytics of tweets
We used text mining and two sentiment analytics method for eight main characters. And draw the line chart and heatmap to visualize the result. 
               
            Figure 2.3 the sentiment analysis line chart                                            Figure 2.4 the heatmap of sentiment analysis

We also draw a summary of the tweets on twitter for the characters.

3.4. Network
Since there are so many characters, we build a network based on five most important characters, the color of line the size of the nodes varies according to the weights.
                      
Figure 2.5 the network for all characters                          Figure 2.6 the network for 5 main characters


 3.5. Machine Learning
We trained our dataset with 6 machine learning algorithms, and solved the two problems.
(1) Firstly, used SMOTE and RandomOverSampler to create more samples and solved the problem of Dataset skewness.
(2) Then, we used Principal component analysis (PCA) to reduce feature dimension.
(3) Choose suitable ML algorithm to compute the accuracy by using cross validation, and grid search the hyperparameter.
Below is the result of our Machine Learning algorithms:
 
Figure 2.7 Machine Learning Results


3.6. GUI
To help users get an interactive experience, we build a GUI. Imaging you are a character in Game of Thrones. You can chose your gender, the family you want to belong to, the culture you are, your identity (for example, being a king or a knight) and other attributes, we can tell the probabilities of being alive for you! Never miss this amazing feature!
 
Figure 2.8 sample of GUI


4. Shinning Points
4.1 build part of the dataset by ourselves
In fact, our dataset is very incomplete, so we used to many methods to complete it…
4.2 beautiful and interactive plots
We learned and used the plotly package to make our images interactive and elegant.
4.3 multi methods
We used many data analytics methods to present the data and analyzed them, we used summary, sentiment analytics…
4.4 machine learning (PCA, RandomOverSampler, SMOTE)
We tried a lot of machine learning algorithms and used many methods to solve the skewness problem and do dimension reduction to make our dataset more suitable for machine learning.
4.5 Interactive experience
We build a GUI and you can build you own character in Game of Thrones.


5. Further Development
5.1. Time Complexity: 
The algorithm to scrap the website is time-consuming(O(n^2)).
5.2. Better GUI: 
we could add more features for our GUI and make it more attractive.


6. Team Members
Love %s Every %s %(U,Day)
Zeqi Zhu (zz2568)
Qi Li (ql2336)
Yashi Huang (yh3068)
Manchun Sun (ms5705)

