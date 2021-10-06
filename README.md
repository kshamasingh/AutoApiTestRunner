# AutoApiTestRunner
Automation Command Line Tool for https://www.drone.io/ CI/CD Pipeline
Trigger .drone.yaml file from command line 

## Installation
### Method-1: Using https://pypi.org/project/AutoApiTestRunner/1.0.1/

Installation Command:

    sudo -H pip install AutoApiTestRunner==1.0.1

### Method-2: Using pip

Installation Command:
NOTE: you must have a working git over ssh configuration.

    ssh -T git@github.com

    “Hi kshamasingh! You've successfully authenticated, but GitHub does not provide shell access.”

    sudo -H python -m pip install --no-cache-dir "git+ssh://git@github.com/kshamasingh/AutoApiTestRunner.git"

Validate the installation by running

    auto --help

## Configuration
you need to configure it before it can access Drone API.
You are going to need a Drone Token and Drone server URL.
Now head over to https://drone-url/account, under *Example CLI Usage* section you will see the token and server URL.
Copy both of them and keep them safe.

You can start initialisation process by executing

    auto init

and provide the information on prompt.
* Drone token:your personal token (https://drone-url/account)
* Drone host:https://drone-url/
* Full name: Your Name
* Github org [Company-Tech]:Company-Tech


## Trigger API Sanity

 Command:

    auto runner
    Repo name:Name of GH repo
    Branch:Custom branch name