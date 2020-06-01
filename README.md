# Wheeler-Classifier
A deep learning model for image classification in between four wheelers and two wheelers. 

<ol>
<li>Obtaining Dataset</li>
<li>Creating Transfer Model</li>
<li>Training Model</li>
</ol>


## 1 Obtaining Dataset
The first step is to obtain the dataset. I obtained all the images through Google Images. I made a Testing and Validation data set from Google Images. This dataset consists of 

Folder Structure is this

* Wheeler Classifier 
    * Training
         * Two Wheelers(693)
         * Four Wheelers(729)
    * Validation
         * Two Wheelers(81)
         * Four Wheelers(77)
         
         


 ## Creating Transfer Model
 I used a Transfer Model, InceptionV3 using which I trained all the images. I set the layers.trainable to False and created my own    Neuron Layers. 
 
 
 ## Training Model
 I used Adam optimizer and loss parameter to be binary-crossentropy, to classify into four wheelers and two wheelers.
