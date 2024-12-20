# PracticalDL_fastai
Hey, welcome, it's just me attending the Practical Deep Learning for Coders Course to review general ML concepts and coding alongside the course videos. 
## Lesson #1
### [1. Is it a bird?](https://github.com/nemat-al/PracticalDL_fastai/blob/main/1.Is_it_a_bird.ipynb)
In the notebook we use duckduckgo_search library for creating a dataset of birds and forests images. Within the notebook and the corresponding course lesson, the library fast.ai is introduced as a library above Pytorch.
Here are some of the concepts and functions from fast.ai:
- DataBlock: High level API to quickly get the data in a DataLoaders, which are used by Pytorch library to grap batch of the data at a time. Mainly, it helps quickly build Datasets and DataLoaders. 
- Learners in fast.ai: we pass the model and datablock to train. By default, the models are downloaded with weights (for example from training over ImageNet dataset).
- The function `fine_tune` its job is given by its name :) Baiscally it  adjust the weights for the specific task.
## Lesson #2
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

## Lesson #3
Few theoritical ideas: 
- Learning rate: finding the right learning rate is a compromise between the speed at which one finds the answer (small learning rate- slow changes through the training) and the possibility that we are actually going to get worse and worse (too big learnign rate).
- Once you get close enough to the optimal values, all functions look like quadratics.
- For data that has extreme distribution, for example money, think of the Titanic fair cost (&0$, 2$,..) we take the log of the values to get somethingmore evenly distributed.
## lesson #4
Few theoritical ideas: 
- ULMfit algorithm: used a RNN langauge model, trained it on data from wikipedia to predict the next word. Then fine-tuned the model from the last step to predict the next word in IMBD reviews about movies. Then the model was fine-tuned to classify the reviews from IMBD as negative or positive.
- Transformers: On the other hand, transformers were trained on data from wikipedia, the data had words deleted randomally from it and the transformers goal was to guess the missing word.
- Underfitting: there's no much complexity in the model to match the data.
- Overfitting: the model has got really good at fitting to the presented data, but if we try iy on more (not trained on) data from the same distribtion, it won't be close to the model.

## lesson 5

### Sources
[Course Link](https://course.fast.ai/)
Original Notebooks for the Course [here](https://github.com/fastai/course22) or [here](https://github.com/fastai/fastbook/tree/master)

