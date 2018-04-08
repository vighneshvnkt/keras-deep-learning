# cognitive-assignment3 on video classification using UCF11 dataset

We used [Microsoft's CNTK Implementation on UCF11 dataset for video classification](https://github.com/Microsoft/CNTK/blob/master/Examples/Video/GettingStarted/Python/Conv3D_UCF11.py)
<br/> and tried to implement the same thing in Keras with a slightly different approach <br/>
We divide our approach into 2 parts : 
<br/> Part 1 :
```
1) Download UCF11 dataset zip file
2) Extract files and examine folder structure - each folder contains videos belonging to the category and annotations
3) Make data ready by generating a CSV file for training and testing, each CSV file containing path to video and category it belongs to.
4) Convert videos to numpy array files and upload to AWS
```
<br/> Part 2 :
```
1) Load numpy files(train_data, train_labels,test_data,test_labels)
2) Pass them into Conv3D model written in Keras
3) Compile and observe results
```
It gave a testing accuracy of around 38% but greatly reduced time to train the model by already saving data in a numpy array.
<br/> Since the training data remains the same, there is no need to convert videos into numpy arrays every time we train the model.
