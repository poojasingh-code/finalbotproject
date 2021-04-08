# finalbot
 rasa chatbot with nodejs, mongodb connectivity

To Run the project, we need three enviornment to be installed 
1. For Node support :- install node.js
2. For Mongo Db Connectivity :-  install mongodb and it's compass
3. For RASA, please read below :-

# Steps to set the environment for RASA:  
1. Install Anaconda latest version  

2. Install the latest python version 3.8.5 

3. Install visual code studio c++ build tool 

4. Create a conda environment in Anaconda prompt by command  
# (before executing make sure you are inside the rasa folder which is cd <your directory>/finalbotproject/rasa)
 
 Once you are inside the rasa folder, please execute below commands

# conda create --name (any name)  python==3.8.5 ( for creating virtual env to run rasa)

# conda activate (a name which you have provided in the previous command)  ( for activating virtual env)

# conda install TensorFlow ( for installing dependency)

# pip install rasa  ( for installing rasa)

 

To run the rasa code: 

-> First step is training, to train the bot and generate a model, please run this command ---> rasa train

once the bot is trained, please run this command to hit the api from frontend ---> rasa run -m models --cors "*" --debug

->  then in another terminal to run the action server please write command---> rasa run actions

this shall load the bot and you can chat via frontend. 


Summary

There should be three separate terminals
1. to run node server --> node server.js
2. to hit API --> rasa run -m models --cors "*" --debug
3. to run action server --> rasa run actions

 
 

