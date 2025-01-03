# Computer Infrastructure Repository
***
This repository contains the assessment task, scripts, and project related to this module. This module was 
focused on creating, managing, navigating directories, downloading data from an external source, and generating 
timestamps. This was done using command-line tools in the Codespase GitHub environment, Bash scripting and 
Python. The dataset used for this module and project has been  downloaded from the **Met Eireann** (Irish 
Meteorological Service) website. The Met Eireann provides monitoring and forecasting of the Irish weather 
forecast.

The purpose of the assessment of this module is to demonstrate competence in the following areas:

1.	Use, configure, and script in a command line interface environment.
2.	Manipulate and move data and code using the command line.
3.	Compare commonly available software infrastructures and architectures.
4.	Select appropriate infrastructure for a given computational task.

## Getting Started

To get started with this project, you will need to download the necessary software/application in case you don't 
have it:

 - **[Anaconda](https://www.anaconda.com/)** - it is a platform which is used to share a code design for machine 
learning and data science. It is open-source distribution of the Python and R programming languages. Modules 
required for this project are Pandas and Matplotlib.

 - **[Visual Studio Code](https://visualstudio.microsoft.com/downloads/)** - it is integrated development 
environment (IDE) designed by Microsoft which can be used for writing, editing, debugging and building the code.

 - **[GitHub](https://github.com/)** - is cloud base platform which allows developers to store, manage and share 
their code. Git is open source and free to use control system which GitHub uses for small and large project to 
track any change you make in GitHub.

<ins>The Jupyter notebook can launched using two options:</ins>

- **Option 1:**&emsp;&emsp;your local device
- **Option 2:**&emsp;&emsp;GiHub Codespaces

## Option 1

To execute a Jupyter Notebook from a GitHub repository on your local machine using Visual Studio Code (VS Code) or Anaconda, follow these steps:

### Clone the GitHub Repository

Open a terminal or command prompt, navigate and execute:

`git clone https://github.com/UWASIKLK/computer-infrastructure.git`

### Set Up the Python Environment

- **Anaconda Environment:** Open Anaconda Navigator, navigate to the 'Environments' tab, and create a new environment with the required Python version.
- **Install Dependencies:** Use the terminal to navigate to the cloned repository's directory and execute:

`conda install --file requirements.txt`

This installs the necessary packages listed in requirements.txt.

### Open notebook in Visual Studio Code (VS)

- **Launch VS Code:** Open VS Code and use the 'Open Folder' option to navigate to the cloned repository.
- **Open Notebook:** Locate the .ipynb file within the repository and open it.
- **Select Python Interpreter:** Press `Ctrl+Shift+P (or Cmd+Shift+P on macOS)`, type `Python: Select Interpreter`, and choose the Anaconda environment you set up earlier.
- **Select Jupyter Kernel:** Click on the kernel picker in the top-right corner of the notebook and select the appropriate kernel associated with your Anaconda environment.

### Execute the Notebook

To run cells use the run button next to each cell or execute all cells sequentially to run the notebook.

Useful information can be found: [VS - Jupyter Notebook](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

## Option 2

GitHub Codespaces is a cloud-based development environment that allows a user to code from any device with 
internet access. To start using codespaces, you'll need to have a personal GitHub account, which has a monthly 
quota of free use of GitHub code spaces. The codespace can be created directly from your GitHub repository or 
you can select an existing template. 

### Create GitHub Codespaces:

-	Clone the repository by using following link: `https://github.com/UWASIKLK/computer-infrastructure.git`
-	Navigate to your GitHub repository
-	Click on the green `<>Code` button on the right top side and select `Codespaces`
-	Select `Create codespace on main`

![Codespaces](./img/Codespaces.png)


The contents of your repository will immediately load into the online version of Visual Studio Code in your 
browser, and you can start writing your code. <br>
After development, commit and push your changes back to the repository directly from the codespace.

More information can be found on: [GitHub Docs](https://docs.github.com/en/codespaces/overview)

## Tasks Summary

**Task 1: Create Directory Structure** - create a directory and subdirectories using the Linux command `mkdir`.

**Task 2: Timestamps** - create a file named **now.txt** that contains the output of current date and time from 
the command `date` using the `‘>>’` redirect operator. Contents of the file are verified with the command `more`.

**Task 3: Formatting Timestamps** - a file named **formatted.txt** that contains the output of current date and 
time in the format `YYYYmmdd_HHMMSS` using the command `date +”%Y%m%d_%H%M%S”`.

**Task 4: Create Timestamped Files** - create a file with the name of the current date in selected format using 
the **backticks** for the `date` command. The `ls -al` and `more` command is used to confirm that file is empty.

**Task 5: Download Today's Weather Data** - command `wget – O` is used to download data from URL and saved as 
*weather.json* file.

**Task 6: Timestamp the Data** - download data from URL with a timestamped name in the format `YYYYmmdd_HHMMSS.
json`.

**Task 7: Write the Script** - automate the download process using the bash script **weather.sh**  and make it 
executable.

**Task 8: Notebook** - create a Jupyter notebook **weather.ipynb** with a description of each task and 
completion. 

**Task 9: pandas** - load data from a URL into an existing Jupyter notebook **weather.ipynb** and explore and 
summarize the data. 

## Project

In this project, I automated weather.sh script using GitHub Actions with the following workflow:

-	Run the script every day at 10:00 UTC and include workflow_dispatch
-	Use the Ubuntu Linux Virtual Machine
-	Clone a repository
-	Execute weather.sh
-	Commit and push weather data back to the repository

## Getting Help

If you have any difficulties or questions, please feel free to contact me.

## Contribute

Any contributions are more than welcome. Feel free to clone the repository if you want to make any changes or 
improvements.

## References:

[How to Create Directory in Linux | mkdir Command - GeeksforGeeks](https://www.geeksforgeeks.org/mkdir-command-in-linux-with-examples/) (Task 1)

[Linux Date Command: Set, Change, Format and Display Date](https://phoenixnap.com/kb/linux-date-command) (Task 3)

[Guide to Linux wget Command With Examples | Baeldung on Linux](https://www.baeldung.com/linux/wget-examples) 
(Task 5)

[Bash Scripting Tutorial: How to Write a Bash Script - LinuxConfig](https://linuxconfig.org/bash-scripting-tutorial) (Task 7)

[Bash Scripting - Introduction to Bash and Bash Scripting - GeeksforGeeks](https://www.geeksforgeeks.org/bash-scripting-introduction-to-bash-and-bash-scripting/) (Task 7)

## Author

Katarina Siklodyova, student at Atlantic Technological University (2024 -2025)