## <center> Assignment 4 </center>

### **Group Members**             
•	Sarthak Dargan – sarthak221995@gmail.com                
•	CV Chiranthan - chiranthancv95@gmail.com                   
•	Mayank Singhal - singhal.mayank77@gmail.com  [ Currently Affected with COVID 19 ]    
• Jayasankar Raju S - muralis2raj@gmail.com  


## Part 1 - Back Propagation
Link to Excel : https://docs.google.com/spreadsheets/d/1a6AN9F0QVc2iToQlo_pnjtil3GEFMty4rmZdRUvI-BY/edit?usp=sharing
Link to Back Propagation Read Me: https://github.com/sarthak221995/TSAI_EVA6/blob/main/Session%204/ReadMe%20-%20%20Back%20Prop.md

## Part 2 - MNIST DIGITS PYTORCH CLASSIFIER

**Best solution Results** : Achieved 99.52% Accuracy on Test Data on 19th Epoch with Total Trainable Params: 19,834. 

**Key Steps** : 
1. We Started with augmenting the training data. We applied Random Rotations, Scaling, Shearing transformations.
2. Created Train Loader and Test Loader
3. Designed the Neural Network using Convolution layers/Max Pool/Dropouts/GAP/Batch Normalization/FC with Total Trainable Params:19,834
4. Train and Test the Model

**Data Augmentation:**

![image](https://user-images.githubusercontent.com/11936036/120030179-c2805000-c014-11eb-8020-94fafc0c7503.png)

**Neural Network Architecture:**

![image](https://user-images.githubusercontent.com/11936036/120030398-0a9f7280-c015-11eb-9111-23668c2a68d0.png)


Other Solutions 

1. https://github.com/sarthak221995/TSAI_EVA6/blob/main/Session%204/Session_4_Less_than_20k_Parameters%20FC%209941.ipynb [ No Data Augmentation: 99.41% Accuracy ]
