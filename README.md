# S6
EVA4 Session 6 assginment


## Step 1

### Target . 

1.   Set up and defining skeleton with Convolution block, GAP and Convolution block.

### Results .  

1.   Parameters: 13,584
2.   Best Train Accuracy 98.53%
3.   Best Test Accuracy 98.34%

### Analysis   

1.   Basic skeleton model doesn't meet target accuracy of 99.4% and model is slightly over-fitting.
2.   Parameters count is >10k



## Step 2

### Target . 

1.   Adding batch-norm and drop-out to reduce over-fitting and improve the model efficiency.
2.   Iterate to find the best drop-out value (0.05 to 0.2)

### Results .  

1.   Parameters: 13,584
2.   Best results with 0.05 as Dropout value where difference b/w test and train accuracy is small.
3.   Best Train Accuracy 99.12%
4.   Best Test Accuracy 99.45%

### Analysis   

1.  Model is under-fitting and total parameters also > 10k.



## Step 3

### Target . 

1.   Eventhough the model is under-fitting and we need to add more parameters. We need to optimizing of output channels to decrease the parameters < 10 K to meet the requirement.

### Results .  

1.   Parameters: 9,752
2.   Best Train Accuracy 99.24%
3.   Best Test Accuracy 99.39%

### Analysis   

1.  Total parameters < 10k
2.  Model performance is good but not achieving 99.4% accuracy target.




## Step 4

### Target . 

1.   Add image augmentation w random rotation and random affine to improve the model performance.

### Results .  

1.   Parameters: 9,752
2.   Best Train Accuracy 98.03%
3.   Best Test Accuracy 99.26%


### Analysis   

1.  Total parameters < 10k
2.  Data augmentation didn't improve the accuracy.



## Step 5

### Target . 

1.   Adding LR Scheduler 
2.   Iterated on learning rate (0.01, 0.02)
3.   Iterated on removing batch-norm and drop-out in initial layer of convolution.

### Results .  

1.   Parameters: 9,712
2.   Best Train Accuracy 99.22%
3.   Best Test Accuracy 99.48%


### Analysis   

1.  Total parameters < 10k
2.  Accuracy > 99.40 consistently for 4 instances in 15 epochs.
3.  Model performance is good as difference between train and test is small.

