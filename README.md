# TensorClick
System and toolchain for easy model creation and archiving, with drag-and-drop interface

### Application description - at glance

entire project consists of simple backend neural network "assembly" + archive manager, while frontend
attempts to simplify model creation, elevating it from pure code-based, to no-code or low-code version
for ease of everyday use.

Everything is connected up with browser-based application (based on Django framework)

#### nn_backend

this sub-application manages neural network creation behind the scenes, as well as hold models, that
connect to database, in order to retrieve information about training process of each neural network
created, architecture info (without the need to re-instantiate entire model), performance metrics
(for example reports from scikit-learn classification performance evaluation functions), and more

#### frontend

this sub-application manages templates, web interface of the tool (frontend) as well as other 
functions/classes that are involved in this part of the project.


### Application goals

Suppose you have a system that could use some bits of machine learning, or neural network creation
You are not that adept at NN framework selection, or you just don't want to code your data collecting 
project, and at the same time machine learning solutions, both from scratch. There are some tools already
available online that could possibly help you, but you are not a huge company with zillions of dollars,
or you simply want something less complex, for quick prototyping, and don't want to store everything in 
just plain jupyter notebooks all the time, while making several notebooks, only to evaluate a handful of models

If this is your case, i think you are at the right place. You will be able to store models, as well
as performance metric for all of them, while the only need that you would need to write, would be 
some sort of function that loads the data. The model creation, automated training with the loaded data,
as well as periodic model performance results with checkpointing (I know this from Tensorflow; 
If this is something from other libraries, let me know and i will edit the very text you now read) are
alse available from one browser page away.


At least that is the goal of the application.




