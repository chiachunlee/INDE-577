## Decision Trees 
------------------------ 
This folder contains Classification Tree and Regression Tree. 

### What is decision tree? 
A decision tree is a type of non-parametric supervised learning that can be used for both regression and classification. In this notebook we explore classification decision trees on an artificial dataset. Decision Trees are a type of Supervised Machine Learning where the data is continuously split according to a certain parameter. The tree can be explained by two entities, namely decision nodes and leaves. The leaves are the decisions or the final outcomes. And the decision nodes are where the data is split. 

### How does it work?
While making decision tree, at each node of tree we ask different type of questions. Based on the asked question we will calculate the information gain corresponding to it.Information gain is used to decide which feature to split on at each step in building the tree. Simplicity is best, so we want to keep our tree small. To do so, at each step we should choose the split that results in the purest daughter nodes. A commonly used measure of purity is called information. For each node of the tree, the information value measures how much information a feature gives us about the class. The split with the highest information gain will be taken as the first split and the process will continue until all children nodes are pure, or until the information gain is 0. 
##### Gini Impurity 
First let’s understand the meaning of Pure and Impure. Pure means, in a selected sample of dataset all data belongs to same class. Impure means, data is mixture of different classes. Gini Impurity is a measurement of the likelihood of an incorrect classification of a new instance of a random variable, if that new instance were randomly classified according to the distribution of class labels from the data set. If our dataset is Pure then likelihood of incorrect classification is 0. If our sample is mixture of different classes then likelihood of incorrect classification will be high. 

<img src="https://lh4.googleusercontent.com/uXug-BxfBY1whm_pRMn-H_v_qW2fdiS3UY-v4SDU2bhjyPo32eBysL_b5Rt1_wFvHIaj8r4RdZJIJHuodG6VP1lLNVd0Zmp4Q6-K7zsVPHRhGYUA787kRymadXxy1t1YV_NeovMs" width="500"/>  

Pi is the probability of an object that is being classified to a particular class. 

##### Steps for Making decision tree 
1. Get list of rows (dataset) which are taken into consideration for making decision tree (recursively at each nodes).
2. Calculate uncertanity of our dataset or Gini impurity or how much our data is mixed up etc. 
3. Generate list of all question which needs to be asked at that node.
4. Partition rows into True rows and False rows based on each question asked. 
5. Calculate information gain based on gini impurity and partition of data from previous step. 
6. Update highest information gain based on each question asked. 
7. Update best question based on information gain (higher information gain). 
8. Divide the node on best question. Repeat again from step 1 again until we get pure node (leaf nodes). <p align="center"> <img src="https://static.javatpoint.com/tutorial/machine-learning/images/decision-tree-classification-algorithm.png" width="500"/> </p>
