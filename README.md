## Problem Statement
+ Educational institutions face numerous challenges in trying to maintain a safe environment and effective administrative procedures. Regularly, attendance and identification tracking methods are manual, tedious, prone to errors and cannot offer real-time monitoring. Additionally, conventional access control systems may be vulnerable to hacking or security breaches. For this reason, there is a need for an automated solution that will effectively address these issues with respect to school security at large.

## Use Case Diagram
<div align="center">
 <img src="https://github.com/user-attachments/assets/a2c7156e-ed51-4a6d-9796-2cb46ffd1f5b">
</div>

## Algorithms Used
1. Haar Cascades - For Face Detection
2. Local Binary Pattern Histograms (LBPHs) - For Face Recognition

## Technologies Used
+ Python and OpenCV

## Domains
+ Machine Learning and Computer Vision

## Results
 + ### 1. Confusion Matrix
   <div align="center">
    <img src="https://github.com/user-attachments/assets/c9b90387-88c1-4405-83bf-d6c0febbebf5">
   </div>

   + It is a matrix where the rows represent the true identities, columns are the predicted identities, and diagonal elements are the number of correctly predicted 
   identities for each class; and others are misclassifications. The elements on the diagonal, in blue, indicate the correct predictions for each class of identity. It 
   correctly classified 'Aman' 9 times. The off-diagonal elements show misclassification. It misclassified 'Krishna' as 'Rohan' 3 times. Similarly, it misclassified 'Kendal' 
   as 'Aman' once and as 'Kohli' once as can be seen from the row 'Kendal' at the intersection of the columns 'Aman' and 'Kohli'.

 + ### 2. Receiver Operating Characteristics (ROC) and Area Under Curve (AUC)
   <div align="center">
    <img src="https://github.com/user-attachments/assets/0c61a70f-cf7a-4062-8078-80f37037bfaf">
   </div>

   + This plot shows that class 'Hritesh' returns the highest AUC of 0.97, hence indicating excellent classification performance for this class, while classes like 'Karim' 
   and 'Krishna' returned a pretty poor AUC value of 0.61, hence their poor classification performance. The ROC curve helps to draw competition between TPR and FPR for each 
   single class. The top-left corner has good classification performance since this point maximizes the rate of true positives with a minimum false positive rate. 


Our project demonstrates variable performance across different classes, with precision ranging from 0.50 to 1.00, recall from 0.33 to 1.00, and F1 scores from 0.33 to 0.94, while achieving an overall accuracy of 0.75, indicating robust performance in certain scenarios but room for improvement in others.
