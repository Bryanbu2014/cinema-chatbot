# Assistant System Project - KI-B-3, TH Deggendorf

## Table of Contents

1. [Project Title](#project-title)
1. [Introduction](#introduction)
1. [Version](#version)
1. [Installation](#installation)
1. [Training](#training)
1. [Usage](#usage)

### <u>Project Title</u>

Assistant system for cinema website/application

### <u>Introduction</u>

An assistant system which assists user to fetch information from cinema website/app such as movie description, availability of a movie, schedule, sitting plan, etc.

### <u>Version</u>

- Python: 3.7 or 3.8
- Rasa: 2.8.12
- Flask: 2.0.2

### <u>Installation</u>

1. Clone the repository with either HTML or SSH using the command

```bash
git clone <repo>
```

2. Open any terminal and cd into the folder. Create a virtual environment using the following command

```bash
python3 -m venv <venv_name>
```

3. After the virtual environment is created, activate the virtual environment

```bash
<venv_name>\Scripts\activate.bat
```

4. Install Rasa
   After the virtual environment is activated, user is requried to install Rasa. In order to have a faster and smooth installation, user is recommended to have the latest pip installed. Upgrade pip using the following command

```bash
<venv_name>\Scripts\python.exe -m pip install --upgrade pip
```

Then now install Rasa

```bash
python -m pip install rasa==2.8.12
```

5. Install Flask

```bash
pip install Flask==2.0.2
```

6. Install requests

```bash
pip install requests
```

### <u>Training</u>

After activated the virtual environment with the required library installed, direct to where the assistant system files are located.
Type `rasa train` to start the chatbot model training.
Example is shown below.

```bash
(venv) ...Cinema-Chatbot\Cinema-Chatbot-Main>rasa train
```

Trained models will be stored in the folder named "models".

### <u>Usage</u>

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
