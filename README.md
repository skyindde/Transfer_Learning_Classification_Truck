# Transfer_Learning_Classification_Truck
Transfer Learning: Image classification with MobileNet-V2


Using trained mobilenet V2 model, 100% accuracy was achieved.

all the important libraries are imported, including Tensorflow and Keras.

The image is set to 224 by 224 pixels.

using image data generator the training data is being uploaded.

there were 60 images belonging to six classes in the training image data.

the validation data is also uploaded.

There were 150 validation images belonging to six classes.And the six classes are Big container with color blue and yellow. Small container with blue.And green and yellow.And loader with red and yellow tractor.

the Mobilenet V2 model from Keras is loaded. this is a very big CNN model with 53 convolutional layers and there are 3.5 million parameters

we get an already trained model so that we don't have to train it fully and we can get most of the train parameters of this model except for the last layer.

trainable has been kept false so that we get the already trained parameters. in the summary there are 2.25 million parameters. But all of them are already trained as
trainable was set to false.

in this model which was extracted, we add a final layer with six categories. In the summary, we have other than 2.26 million already trained parameters and 7686 parameters which should be trained.

we compile the model with categorical cross entropy and we are using batch start callback to improve the performance.

The model is trained with our training image data. number of epocs has been set to 8. This was based on experience while developing this.

The accuracy on training data and validation data gradually increases over the epochs. Finally, at the end of the epics, both testing and validation accuracy reaches

100%.

The train model is used to predict category for the training data again.

testing image data is uploaded. The model is applied to predict the classes on the testing data set.

to assess the performance of the model classification report on testing data is printed. the model performed perfectly.

The accuracy for each class as well as overall accuracy is 100%.
on the confusion matrix all the numbers are along the main diagonal.And all the elements elsewhere is 0. This shows that all the 150 images belonging to six categories with 25 images in each have been predicted accurately without any false positive or false negative outcomes. 

the lost value during the training has decreased over the epochs.

Similarly, the training and validation accuracy over the EPICS has increased and finally saturated to 100%. 

And the training and validation loss hasdecreased and converged to around 0.4.

