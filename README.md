# DNA_binding-protein-prediciton
prediction of DNA-binding protein, the accucacy reaches about 84%

In the process of data extraction, 
we mainly extract four kinds of features: 
  1) the frequencies of 20 kinds of amino acid of protein. It is 20D. 
  2) the best 10 of the top-2-gram base on the work of Zhou[1]. It is 10D. 
  3) local-DPP feature based on the PSSM, according to the work of Wei[2]. It is about 120D. 
  4) PSSM-DT feature based on the PSSM, according to the work of Zhou[1]. It is 2000D. 
  So, we extract 2150D effective features.
In the process of choosing classifier and building model. We have tried different classifier models: 
  logistic regression, support vector machine, gradient boosting, xgboost and random forest.
We do a lot of work on the feature extraction and choose classification model. 
Finally, we can get the 2150D features step by step. What’s more, different classification will have great effect on the accuracy of result. So, we do the comparison of them to choose the best.
Finally, we can get the best accuracy of 84.0% using the 1250D feature and the gradient boosting classification model.
