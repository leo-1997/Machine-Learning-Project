# Machine-Learning-Project
# Development
Upon cloning, download the python packages by running: (for Linux)
```
cd Machine-Learning-Project
python3 -m venv ./env
env/bin/pip install -r requirements.txt
``` 

To create a new requirement file upon installing more packages, run: (on Linux)
```
cd Machine-Learning-Project
env/bin/pip install pandas
env/bin/pip freeze > requirements.txt
``` 

# Arts Project

# Motivation
Art is the highest expression of a culture, especially that in the form of drawings and paintings. Each artist has his or her own unique style of painting, an area which has drawn great curiosity and research. By detecting and analysing the colors used and the geometric pattern inside a picture, the artist and the genre of the painting can be predicted. This technology could help people to dig into the magic of the arts, giving people an opportunity to have a deeper understanding and more thorough cognition of the famous artists of the world. Even though some artists may not be alive anymore, they live through their art, and studying this will allow us to appreciate these gems that we have lost to time.  
   
# Statement of the Problem/Task
Our project is a problem of image recognition. Our main task is to develop a model to accurately classify over 8,000 paintings into the correct genres and artists by analysing a collection of artworks of the 50 most influential artists of all time. We will tentatively use Convoluted Neural Networks (CNN) to approach the problem. The key questions and challenges that we will be addressing are:
* What attributes are to be extracted from the images to classify the paintings’ genre and artists respectively?
* How do we classify paintings of artists with works of very different styles?
* Capturing attributes of the paintings may require high resolution of the image, but this increases the training time drastically. How do we strike a balance between the two?
* What is the best model or algorithm to classify the paintings optimally?
Extension:
* Is it possible to predict the year of the painting?

# General Approach	
Our project falls in the domain of supervised machine learning, given a Kaggle dataset of 50 famous artists and their paintings. We will firstly process our raw data, ie the full-sized images of paintings, by resizing and removing noise from the dataset. For example, some paintings are sketchwork and hence not very relevant for the purpose of this project.
Secondly, we will extract helpful attributes of the paintings based on observation and research on artworks.
Meanwhile, the dataset has class imbalance problem. For example, Van Goh had 800+ paintings whereas Pollock only had 24. We will tackle this problem through some data augmentation to improve performance on the test set.
We will train a variety of models to fit and test on the dataset which includes but is not limited to CNN. Other algorithms such as k-nearest neighbors algorithm, shift-invariant neural network may also be used to compare performance. We will then evaluate which model gives the best performance and analyse why it is the ideal model for our project.
Last but not the least, we will continue to improve our model and summarize what could be the limitations of our project.

# Evaluation	
We aim to achieve a high accuracy in classifying the paintings.
Satisfactory outcome: To train a neural network model that hits a 60% accuracy benchmark for both predicting the genre and the artist. 
Excellent outcome: To achieve a ~90% accuracy in painting identification, and provide a detailed analysis on the performance of different models in our project.

# Resources:
Resource and Tools:
Dataset of full image of labelled paintings from Kaggle:https://www.kaggle.com/basu369victor/style-transfer-deep-learning-algorithm
Keras: https://keras.io/
Readings:
Flexible, High performance CNN for image classification:
https://www.aaai.org/ocs/index.php/IJCAI/IJCAI11/paper/view/3098/3425
CNN-RNN: A Unified Framework for Multi-Label Image Classification:
https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Wang_CNN-RNN_A_Unified_CVPR_2016_paper.html
