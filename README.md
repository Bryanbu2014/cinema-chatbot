# Assistant System Project - KI3, TH Deggendorf

## Table of Contents
* Project Title
* Introduction
* Version
* Installation
* Training
* Usage


A. Project Title
----------------
Assistant system for cinema website/app


B. Introduction
---------------
An assistant system which assists user to fetch information from cinema website/app such as movie description, availability of a movie, schedule, sitting plan, etc.


C. Version
----------
- Python version - 3.7 or 3.8
- Rasa version - 2.8.12
- Flask version - 2.0.2


D. Installation
---------------
For Windows:
Required Python 3.7 or 3.8

1. Download the file Rasa Projects.zip and extract it

2. Create a virtual environment
In Command Prompt (CMD), direct to the folder named AS inside the Rasa Projects folder, and create a virtual environment inside the Cinema-Chatbot-Main folder using the following command:  

--- python3 -m venv venv ---  

For example, in this instance:  

--- Cinema-Chatbot\Cinema-Chatbot-Main>python3 -m venv venv ---

3. Activate the virtual environment
To activate the virtual environment, type in the command line shown below.  

--- venv\Scripts\activate.bat ---  

For example, in this instance:  

--- Cinema-Chatbot\Cinema-Chatbot-Main>venv\Scripts\activate.bat ---

4. Install rasa
After activated the virtual environment, user is required to install rasa. 
In order to have a faster installation, user is recommended to have latest pip installed.
Upgrade pip using the following command:  

--- venv\Scripts\python.exe -m pip install --upgrade pip ---  

For example, in this instance:  

(venv) ...\Cinema-Chatbot\Cinema-Chatbot-Main>venv\Scripts\python.exe -m pip install --upgrade pip

To install rasa, type in the command line shown below.  

--- python -m pip install rasa==2.8.12 ---  

For example, in this instance:  

(venv) ...\Cinema-Chatbot\Cinema-Chatbot-Main>python -m pip install rasa==2.8.12

5. Install flask
Command line shown below.  

--- pip install Flask==2.0.2 ---

6. Install requests
Command line shown below.  

--- pip install requests ---


E. Training
-------------------
After activated the virtual environment with the required library installed, direct to where the assistant system files are located.
Type rasa train to start the chatbot model training.
Example is shown below.
(venv) ...Cinema-Chatbot\Cinema-Chatbot-Main>rasa train
Trained models will be stored in the folder named "models".


F. Usage
--------
1. Start a flask server
After a model is trained, user is required to start a flask server before running the chatbot.
To start a flask server, activate the virtual environment in CMD and direct to where the assistant system files are located.
Type startflask.bat to start flask server.
Example is shown below.
(venv) ...Cinema-Chatbot\Cinema-Chatbot-Main>startflask.bat

2. Rasa run actions
In a new CMD, activates the virtual environment and direct to where the assistant system files are located.
Type rasa run actions.
Example is shown below.
(venv) ...Cinema-Chatbot\Cinema-Chatbot-Main>rasa run actions

3. Start the chatbot
In a new CMD, activates the virtual environment and directs to where the assistant system files located.
Type rasa shell to start the chatbot.
Example is shown below.
(venv) ...Cinema-Chatbot\Cinema-Chatbot-Main>rasa shell

User is expected to ask the chatbot anything related the cinema such as 
- description of a movie
- what movie is available on a day
- sitting plan
- schedule of the movie 
- ticket price
