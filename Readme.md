# Berkeley DataScience

This repository contains a container build for Berkeley DataScience Libary and Otter Grader. This VScode container can be utilised to teach the concepts of DataScience, and the DataScience Python Library.

## Before You Start

The Visual Studio Code Remote - Containers extension lets you use a Docker container as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. A .devcontainer folder in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack. This container can be used to run an application or to sandbox tools, libraries, or runtimes needed for working with a codebase.

Workspace files are mounted from the local file system or copied or cloned into the container. Extensions are installed and run inside the container, where they have full access to the tools, platform, and file system. This means that you can seamlessly switch your entire development environment just by connecting to a different container.

## Running the container within VSCode on Windows, Mac or Linux

You can run this container from VSCode locally see <a href ='https://code.visualstudio.com/docs/remote/containers' target='_blank'>https://code.visualstudio.com/docs/remote/containers</a>.

## The following Requirements are installed as part of the container build

- jupyter
- datascience
- otter-grader
- numpy
- pandas
- scipy
- folium==0.2.1
- matplotlib
- ipywidgets>=7.0.0
- bqplot
- nbinteract==0.0.12
- otter-grader
- okpy  

## Runing the container in Visual Studio Online (Browser Experience)

install this in Visual Studio Online <a href='https://visualstudio.microsoft.com/services/visual-studio-online/' target ='blank'>https://visualstudio.microsoft.com/services/visual-studio-online/ you'll need the following:

- A Microsoft Azure subscription. If you don't already have one, you can sign up for a free trial at <a href ='https://azure.microsoft.com' target='_blank'>https://azure.microsoft.com</a> or a Student Subscription at <a href ='https://aks.ms/azureforstudents' target='_blank'>https://aka.ms/azureforstudents</a>.
- A Visual Studio Online environment. This provides a hosted instance of Visual Studio Code, in which you'll be able to run the notebooks for the lab exercises. To set up this environment:
    1. Browse to <a href ='https://online.visualstudio.com' target='_blank'>https://online.visualstudio.com</a>
    2. Click **Get Started**.
    3. Sign in using the Microsoft account associated with your Azure subscription.
    4. Click **Create environment**. If you don't already have a Visual Studio Online plan, create one. This is used to track resource utlization by your Visual Studio Online environments. Then create an environment with the following settings:
        - **Environment Name**: *A name for your environment - for example, **MSLearn-Datascience**.*
        - **Git Repository**: leestott/python3-BerkeleyDatascience
        - **Instance Type**: Standard (Linux) 4 cores, 8GB RAM
        - **Suspend idle environment after**: 120 minutes
    5. Wait for the environment to be created, and then click **Connect** to connect to it. This will open a browser-based instance of Visual Studio Code.
    6. Wait for a minute or so while the environment is set up for you. It might look like nothing is happening, but in the background we are installing some extensions that you will use in the labs.
    7. Copy your notebooks files and data and undertake your learning

> **Tip**: you can change the color scheme back to a dark background if you prefer - just click the **&#9881;** icon at the bottom left and select a new **Color Theme**.
