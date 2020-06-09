# Wheeler-Classifier
A deep learning model for image classification for four wheelers and two wheelers. 

<ol>
<li>Obtaining Dataset</li>
<li>Creating Transfer Model</li>
<li>Training Model</li>
</ol>


## 1 Obtaining Dataset
   Obtaining dataset for this model was surprisingly tough, I expected to find images for this with ease with the help of this tool.  
   [Image Collector](https://chrome.google.com/webstore/detail/download-all-images/ifipmflagepipjokmbdecpmjbibjnakm?hl=en)<br/><br/>
   All you need to do is search for the images you want, scrool from top to bottom in Google Images or any other sources such as   
   Unsplash, and click on the extension. Though, it's just scrolling and clicking, collecting a dataset for more than 8000 images was  
   tough. 

This is the folder structure. 
* Wheeler Classifier 
    * Training
         * Two Wheelers
         * Four Wheelers
    * Validation
         * Two Wheelers
         * Four Wheelers
         

         
 ![Sample Image Display](https://github.com/lakshmansamvith/Wheeler-Classifier/blob/master/Screenshots/Imgshow.png)


 ## Creating Transfer Model
    I used a Transfer Model, InceptionV3 using which I trained all the images. I set the layers.trainable to False, except for the last     two layers  and created the last two layers.  
 
   
   ![Inception Model](https://github.com/lakshmansamvith/Wheeler-Classifier/blob/master/Inception.png)
 
 
 
 ## Training Model
   I used Adam optimizer and  binary-crossentropy as loss parameter for compilation of the model, to classify into four wheelers and two    wheelers. I trained the model for 15 epochs
   
   ![Epoch Transition](https://github.com/lakshmansamvith/Wheeler-Classifier/blob/master/Screenshots/Epoch-Training.png)
   
    From this model you can see that the accuracy of the model is very high from the first epoch. In fact, you can also see that      
    validation acc. I also plotted a loss and accuracy graph for better understanding. 
    
   ![Loss Accuracy Graph](https://github.com/lakshmansamvith/Wheeler-Classifier/blob/master/Screenshots/Accuracy-Loss.png)
   
   
