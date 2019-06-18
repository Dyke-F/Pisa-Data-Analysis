# Pisa Dataset Exploration
## by Gabriela Sikora


## Dataset

The dataset that I used for this project was the PISA 2012 dataset. PISA, in particular, is a "survey of students' skills and knowledge as they approach the end of compulsory education. It is not a conventional school test. Rather than examining how well students have learned the school curriculum, it looks at how well prepared they are for life beyond school" (Udacity, 2019).

Within this datset we can find information for about 510,000 students. For each of these students, there are 636 answers which we can see in the columns. Of these, I decided to wrangle this dataset into a more manageable dataset of 15167 students with 19 columns. These columns carry the following information about each student: 

- Country                                          
- Student ID                                         
- Gender                                           
- Out-of-School Study Time - Homework              
- Out-of-School Study Time - Guided Homework       
- Out-of-School Study Time - Personal Tutor        
- Out-of-School Study Time - Commercial Company    
- Out-of-School Study Time - With Parent           
- Learning Time - Mathematics                      
- Learning Time - Test Language                    
- Learning Time - Science                          
- Average Math Score                               
- Average Reading Score                            
- Average Science Score                            
- Average Total Score                              
- Education - Father                                
- Education - Mother                                
- Out-of-School Study Time - Total                 
- Learning Time - Total


## Summary of Findings

Throughout the exploration of the cleaned PISA dataset, I wanted to  explore two questions: 
- Is there a relationship between the amount of time a student dedicates to learning and their score? 
- Are there differences in achievement based on gender or parental education levels?

When comparing the amount of time a student puts into their studies and the score they achieved, there ended up being practically no relationship between the Learning Time - Total, the Out-of-School Study Time - Total, and each of the Score metrics. This immediately hinted at the answer: there is no relationship between time spent learning and the ultimate score. Nevertheless, I looked deeper into the variables that comprised each of these totals.

When breaking down the Learning Time variables, it became obvious that Learning Time - Science was the variable that raised the Learning Time - Total. It had an average positive correlation of 0.093 between it and the Score variables, and this is enough to classify it as a weak positive correlation. When looking at it more closely in the multivariate exploration, it became clear that the Learning Time - Science variable had this weak positive correlation only when it came to higher levels of parental education. 

As for the Out-of-School Study Time variables, almost all of them showed a weak negative correlation. The one variable that did not show a weak negative correlation was Out-of-School Study Time - Homework. This variable actually had an average positive correlation of 0.237 between it and the Score variables. This indicated that although homework is a positive indicator for a student's score, Out-of-School Study Time is in general not a very good metric for predicting the success of a student's score. 

In regards to whether or not there is a relationship between the amount of time a student dedicates to learning and their score, I would have to say that the two variables of Learning Time - Science and Out-of-School Study Time - Homework are not strong enough to create a clear conclusion. Therefore, I would say that the amount of time a student dedicates to learning does not have a clear correlation with their score. 

As for the section question of whether there are differences in achievement based on gender or parental education levels, the answers are more clear. Although the amount was higher of students with parents who have higher educational levels, a pattern was very clear with what was expected. It is clear from the data in this dataset that the more education a parent has, the more likely the child is to have a higher score. There are, of course, outliers for each group, but the average tended to increase. That is however until either the mother or the father attained upper secondary education. From that point on, the score plateaus among the student's Average Total Score. We can, nevertheless say that parental level of education has a positive correlation with the Average Total Score. 

On the other hand, the second half of this question did not have such a difference. In fact, from all the plots observed, it seems as if gender does not play a role in the Score a student is likely to receive. There was however once exception. There was a slight advantage for female students when it came to the Average Reading Score. But beyond that, the males and females performed very similarly. 


## Key Insights for Presentation

For the presentation, I will ...
