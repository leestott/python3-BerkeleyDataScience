# Berkeley DataScience

This repository contains a container build for Berkeley DataScience Library and Otter Grader. This VScode container can be utilised to teach the concepts of DataScience, and the DataScience Python Library.

## Before You Start

The Visual Studio Code Remote - Containers extension lets you use a Docker container as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. A .devcontainer folder in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack. This container can be used to run an application or to sandbox tools, libraries, or runtimes needed for working with a codebase.

Workspace files are mounted from the local file system or copied or cloned into the container. Extensions are installed and run inside the container, where they have full access to the tools, platform, and file system. This means that you can seamlessly switch your entire development environment just by connecting to a different container.

# Running the container within VSCode on Windows, Mac or Linux

You can run this container from VSCode locally see <a href ='https://code.visualstudio.com/docs/remote/containers?WT.mc_id=academic-0000-leestott' target='_blank'>https://code.visualstudio.com/docs/remote/containers?WT.mc_id=academic-0000-leestott</a>.

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

You can run this container from VSCode locally see <a href ='https://code.visualstudio.com/docs/remote/containers?WT.mc_id=academic-0000-leestott' target='_blank'>https://code.visualstudio.com/docs/remote/containers?WT.mc_id=academic-0000-leestott</a>.

## Quick Start Installation

To get started, follow these steps:

Install and configure [Docker](https://www.docker.com/get-started) for your operating system.

Windows / macOS:

Install Docker [Desktop for Windows/Mac](https://www.docker.com/products/docker-desktop)

Right-click on the Docker taskbar item and update Settings / Preferences > Shared Drives / File Sharing with any source code locations you want to open in a container. If you run into trouble, see [Docker Desktop for Windows](https://code.visualstudio.com/docs/remote/troubleshooting?WT.mc_id=academic-0000-leestott#_docker-desktop-for-windows-tips) tips on avoiding common problems with sharing.

Linux:

Follow the official [install instructions for Docker](https://docs.docker.com/install/#supported-platforms) CE/EE for your distribution. If you are using Docker Compose, follow the [Docker Compose](https://docs.docker.com/compose/install/) directions as well.

Add your user to the docker group by using a terminal to run: sudo usermod -aG docker $USER

Sign out and back in again so your changes take effect.

Install [Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=academic-0000-leestott)

Install the [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension)

## Loading the Docker container in Visual Studio Code

Let's start by using a sample project to try things out.

Clone one of the repository

Start VS Code and click on the quick actions Status Bar item in the lower left corner of the window.
![VScodeStatusBar](https://code.visualstudio.com/assets/docs/remote/common/remote-dev-status-bar.png?WT.mc_id=academic-0000-leestott)

Quick actions Status bar item

Select Remote-Containers: Open Folder in Container... from the command list that appears, and open the root folder of the project you just cloned.

The window will then reload, but since the container does not exist yet, VS Code will create one. This may take some time, and a progress notification will provide status updates. Fortunately, this step isn't necessary the next time you open the folder since the container will already exist.

![ContainerProgress](https://code.visualstudio.com/assets/docs/remote/containers/dev-container-progress.png?WT.mc_id=academic-0000-leestott)

Dev Container Progress Notification

After the container is built, VS Code automatically connects to it and maps the project folder from your local file system into the container. Check out the Things to try section of README.md in the repository you cloned to see what to do next.

Tip: Want to use a remote Docker host? See the Advanced Containers article for details on setup

# Running the container in Visual Studio Online (Browser Experience)

install this in Visual Studio Online <a href='https://visualstudio.microsoft.com/services/visual-studio-online/?WT.mc_id=academic-0000-leestott' target ='blank'>https://visualstudio.microsoft.com/services/visual-studio-online/?WT.mc_id=academic-0000-leestott you'll need the following:

- A Microsoft Azure subscription. If you don't already have one, you can sign up for a free trial at <a href ='https://azure.microsoft.com/?WT.mc_id=academic-0000-leestott' target='_blank'>https://azure.microsoft.com/?WT.mc_id=academic-0000-leestott</a> or a Student Subscription at <a href ='https://aks.ms/azureforstudents' target='_blank'>https://aka.ms/azureforstudents</a>.
- A Visual Studio Online environment. This provides a hosted instance of Visual Studio Code, in which you'll be able to run the notebooks for the lab exercises. To set up this environment:
    1. Browse to <a href ='https://online.visualstudio.com/?WT.mc_id=academic-0000-leestott' target='_blank'>https://online.visualstudio.com/?WT.mc_id=academic-0000-leestott</a>
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
