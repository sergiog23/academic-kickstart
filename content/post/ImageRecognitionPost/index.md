
+++ title = "Image Recognition " 
summary = " Image recognition using Jupyter Notebook, Google Colab GPU, Tensorflow " 
+++

## Background 
Image captioning is the process of generating text description of images and it uses Natural Language Processing  and Computer Vision to generate captions. For this Project I used TensorFlow tutorial, Image Captioning with visual attention. It uses an attention based model which allows us to see what parts of the image the model focuses on to generate a caption. It initially downloads an MS-COCO image dataset and preprocesses it using Inception V3 engine. It is a 13GB size file but we limit the training to 30,000 captions to speed up training. 
## Challenges Faced 
I had not used Google Collab or Jupyter Notebook before so it was challenging to learn and apply technologies. The tutorial walked you through the training process but did not show you how to caption your own image dataset and how to store them in a file you could retrieve later. I managed to run the model on a smaller image dataset that contained about 500 images from the FLICKR 8K dataset. The model does fairly well when there is only one action going on in the image, if there are multiple people and objects the model does poorly since it only goes through 20 Epochs. The tutorial took about 3 hours to train the model and initially I had trouble captioning my image dataset since I had a bug with image paths. 
## Limitations 
These are some examples that the system captioned are incorrect based on the complexity on the image.
![YES](/post/aman.png)
In this example we see that the caption generated is not very accurate since it classifies the woman as a and it confuses DJ disks with Stove tops 
![YES](/post/aman2.png)
In this example we see that the caption generated it confused a woman holding a baby with a man and a smart phone

## Link to project 
[CLICK HERE](http://sergioguerrero.pythonanywhere.com/)

## References: 
[Flask](https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)
[TensorFlow](https://www.tensorflow.org/tutorials/text/word_embeddings)
[Image Captioning](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/eager/python/examples/generative_examples/image_captioning_with_attention.ipynb)
[Tutorial Deep Learning](https://hackernoon.com/begin-your-deep-learning-project-for-free-free-gpu-processing-free-storage-free-easy-upload-b4dba18abebc)