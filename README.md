Welcome to Advanced Topics of Artificial Intelligence Winter 2024-2025
==============================

The material of this course has been created originally by Raoul Grouls for the MADS (Master in Advanced Data Science in HAN) and it is being adapted to be used in the course of Advanced Topics of Artificial Intelligence at [**Rhine-Waal University of Applied Sciences (HSRW)**](https://www.hsrw.eu/). 
As part of a collaboration project funded by the DAAD, we are planning a Hackathon in Deep Learning at HAN for the students of MADS (HAN) and MIE (HSRW)

This course is part of a series of modules for data science.
This course assumes you have done the introduction in Python and something similar to the Data Analyses & Visualisation course https://github.com/raoulg/MADS-DAV


The lessons can be found inside the `notebooks`folder.
The source code for the lessons can be found in the `src`folder.

The book we will be using is Understanding Deep Learning. It is available as pdf here: https://udlbook.github.io/udlbook/ but it is highly recommended to buy the book.


Project Organization
------------

    ├── README.md          <- This file
    ├── .gitignore         <- Stuff not to add to git
    ├── .lefthook.yml      <- Config file for lefthook
    ├── pyproject.toml     <- Human readable file. This specifies the libraries I installed to
    |                         let the code run, and their versions.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── processed      <- The processed datasets
    │   └── raw            <- The original, raw data
    │
    ├── models             <- Trained models
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is xx_name_of_module.ipynb where
    │                         xx is the number of the lesson
    ├── presentations      <- Contains all powerpoint presentations in .pdf format
    ├── references         <- background information
    |  └── codestyle       <- Some code Code style standards
    |  └── leerdoelen      <- Learning goals per lesson, including pages to read and videos to watch
    │
    ├── reports            <- Generated analysis like PDF, LaTeX, etc.
       └── figures         <- Generated graphics and figures to be used in reporting

--------

For this project you will need some dependencies.
The project uses python 3.10, and dependencies are defined within the `pyproject.toml` file. You will also find `requirements.lock` files, but they are generated for a Mac so they will miss cuda specific dependencies.

The `.lefthook.yml` file is used by [lefthook](https://github.com/evilmartians/lefthook), and lints & cleans the code before I commit it. Because as a student you probably dont commit things, you can ignore it.

I have separated the management of datasets and the trainingloop code. You will find them as dependencies in the project:
- https://github.com/raoulg/mads_datasets
- https://github.com/raoulg/mltrainer

Both of these will be used a lot in the notebooks; by separating them it is easier for students to use the code in your own repositories.
In addition to that, you can consider the packages as "extra material"; the way the pacakges are set up is something you can study if you are already more experienced in programming.
## Installing python with Rye

### Installation for Linux [Recommended]
1. watch the [introduction video about rye](https://rye.astral.sh/guide/)
2. You skipped the video, right? Now go back to 1. and actually watch it. I'll wait.
3. Open your Terminal
4. install [rye](https://rye.astral.sh/) with `curl -sSf https://rye.astral.sh/get | bash`

run through the installer like this:
- platform linux: yes
- preferred package installer: uv
- Run a Python installed and managed by Rye
- which version of python should be used as default: 3.10
- should the installer add Rye to PATH via .profile? : y
- run in the cli: `source "$HOME/.rye/env"`

### Installation for Mac
1. watch the [introduction video about rye](https://rye.astral.sh/guide/)
2. You skipped the video, right? Now go back to 1. and actually watch it. I'll wait.
3. Open your Terminal
4. install [rye](https://rye.astral.sh/) with `curl -sSf https://rye.astral.sh/get | bash`

run through the installer like this:
- platform macos: yes
- Run the old default Python (provided by your OS, pyenv, etc.)
- should the installer add Rye to PATH via .profile? : y

5. run in the terminal: `source "$HOME/.rye/env"`
6. install python 3.10 as follow: `rye fetch 3.10`


### Installation for Windows

1. watch the [introduction video about rye](https://rye.astral.sh/guide/)
2. You skipped the video, right? Now go back to 1. and actually watch it. I'll wait.
3. Activate "Developer Mode" on Windows. Follow the instruction of **Windows Developer Mode** [See this page](https://rye.astral.sh/guide/faq/#windows-developer-mode)
4. Download and install the latest release of [rye](https://rye.astral.sh/) 


## add the git repo
run in the cli:

`git clone https://github.com/Clein2312/Advanced_AI_Applications_WS24-25_MADS_HSRW.git`

## add your username and email to git
1. `git config --global user.name "Mona Lisa"`
2. `git config --global user.email "m.lisa@pisa.com"`

## install all dependencies
1. `cd MADS-MachineLearning-course/`
2. `rye sync`

## add your own ssh key
1. copy your local ssh key, see [github docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Follow the steps of [Test SHH Key](https://gist.github.com/xirixiz/b6b0c6f4917ce17a90e00f9b60566278) and run the command to set your remote repository
3. Add the key to the ssh-agent as described above. 

## Still watch the video.

I know some of you still skipped the video. Ok, I get that, but now actually watch it... [introduction video about rye](https://rye.astral.sh/guide/)
