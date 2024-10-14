# PracticalDL_fastai
Hey, welcome, it's just me attending the Practical Deep Learning for Coders Course to review general ML concepts and coding alongside the course videos. 

### [1. Is it a bird?](https://github.com/nemat-al/PracticalDL_fastai/blob/main/1.Is_it_a_bird.ipynb)
In the notebook we use duckduckgo_search library for creating a dataset of birds and forests images. Within the notebook and the corresponding course lesson, the library fast.ai is introduced as a library above Pytorch.
Here are some of the concepts and functions from fast.ai:
- DataBlock: High level API to quickly get the data in a DataLoaders, which are used by Pytorch library to grap batch of the data at a time. Mainly, it helps quickly build Datasets and DataLoaders. 
- Learners in fast.ai: we pass the model and datablock to train. By default, the models are downloaded with weights (for example from training over ImageNet dataset).
- The function `fine_tune` its job is given by its name :) Baiscally it  adjust the weights for the specific task.
 
### [2. Classifying Bears](https://github.com/nemat-al/PracticalDL_fastai/blob/main/2.1.Classifying_bears_train_then_clean.ipynb)

Through the notebook and the corresponding course video, it was introduced that augmentation processes can be applied through the `DataBlocks`.

The main idea presented here is: Before you clean the data, train the model!

The idea is that once we know where the model is suffering to classify the data, we can either find a better way to gather the data, or find an automatic way to clean the data.

Note: High loss is either when the model is wrong and confideint or when the model is right and not confidient

### [3. Classifying Cats and Dogs](https://github.com/nemat-al/PracticalDL_fastai/blob/main/2_2_dogs_cats_deployment.ipynb)
How to put a model into production?
- Find out the problem to solve, what data is needed and then gather the data.
- Process the data and clean it, consider training the model before cleaning the data.
- Training, testing, and adjusting if needed.
- Deployment: It's done using HuggingFace spaces and Gradio

### Sources
[Course Link](https://course.fast.ai/)
Original Notebooks for the Course [here](https://github.com/fastai/course22) or [here](https://github.com/fastai/fastbook/tree/master)

