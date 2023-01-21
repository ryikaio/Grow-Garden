# Grow-Garden
Grow Garden is a website that incorporates a handwritten canvas to allow the user to draw the correct sum of two numbers displayed on the website, which becomes the input for the machine learning model to predict the number.    
## Dependencies
* HTML
* CSS
* Javascript
* Python
* Numpy
* Tensorflow
## Dataset:
#### MNIST dataset
MNIST set is a large collection of handwritten digits. It is a very popular dataset in the field of image processing. It is often used for benchmarking machine learning algorithms.
MNIST is short for Modified National Institute of Standards and Technology database.     
MNIST contains a collection of 70,000(training set of 60,000 examples, and a test set of 10,000 examples), 28 x 28 images of handwritten digits from 0 to 9.   
## Conversion:
To convert the tensorflow model to tensorflowjs model use the following commands:   
`pip install tensorflowjs`   
```
tensorflowjs_converter \
    --input_format=tf_saved_model \
    --output_node_names='MobilenetV1/Predictions/Reshape_1' \
    --saved_model_tags=serve \
    /mobilenet/saved_model \
    /mobilenet/web_model   
```
