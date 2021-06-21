# Facebook-Friend-Recommendation-using-Graph-Mining
1. Data set used is avilable on kaggle :  https://www.kaggle.com/c/FacebookRecruiting
2. Mapping the problem into supervised learning problem:
      Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz           score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.
     Some reference papers and videos :
       https://www.cs.cornell.edu/home/kleinber/link-pred.pdf                              
       https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf
       https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf
       https://www.youtube.com/watch?v=2M77Hgy17cg
3. Feature Engineering: 

we will create these each of these features for both train and test data points
1.Weight Features
     weight of incoming edges                           
     weight of outgoing edges                        
     weight of incoming edges + weight of outgoing edges          
     weight of incoming edges * weight of outgoing edges               
     2*weight of incoming edges + weight of outgoing edges               
     weight of incoming edges + 2*weight of outgoing edges             
2.Page Ranking of source                                  
3.Page Ranking of dest                                                                
4.katz of source                                                                  
5.katz of dest                                                                   
6.hubs of source                                                             
7.hubs of dest                                                                        
8.authorities_s of source                                                             
9.authorities_s of dest                                                                          
