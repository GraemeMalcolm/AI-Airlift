# Exercise 1: Exploring Images

In this exercise, you will set up a *Data Science Virtual Machine* (DSVM) in Azure, and import the code from this GitHub repo into its *Jupyterhub* environment. You'll then use a Python notebook to generate and explore some image data.

## 1. Create a DSVM

1. In the Azure portal, create a new **Data Science Virtual Machine for Linux (Ubuntu)** resource with the following settings:
    - Resource Group: _Create a new resource group_
    - Virtual Machine Name: _Any unique name_
    - Region: _Any available region_
    - Virtual Machine Image: Data Science Virtual Machine for Linux (Ubuntu)
    - Size:  _NC6_ Standard (GPU Family)
    - Authentication type:  _Password_
    - Username: _(Specify a **lowercase** user name of your choice)_
    - Password: _(Specify a complex password)_
    - OS Disk Type: Standard SSD
2. View the properties of your DSVM and determine its IP address.

## 2. Explore Jupyterhub

1. In a new browser tab, navigate to Jupyterhub on your DSVM at https://*YOUR.DSVM.IP.ADDRESS*:8000. You will need to click through the certificate validation warning messages that are displayed.
2. Sign into Jupyterhub using the user name and password you specified when creating the DSVM. If the home page doesn't open after a few seconds, click the ***jupyter*** logo to open it. 
3. Note that the DSVM already contains notebooks for you to explore. Then on the **New** menu, click **Terminal** and click through the certificate warnings once again until you open a terminal window.
4. In the terminal window, enter the following command to change the current directory to the **notebooks** folder:
    ```shell
    cd notebooks
    ```
5. Now enter the following command to clone this GitHub repository to this folder:

    ```shell
    git clone https://github.com/GraemeMalcolm/AI-Airlift
    ```
6. After the repo has been downloaded, switch back to the tab containing the folder tree, refresh the view if necessary, and verify that the **AI-Airlift** folder has been downloaded.
7. Open the **AI-Airlift** folder and note that it contains the files and folders from this repo.

## 3. Use Python to Explore Images

1. In the **AI-Airlift/code** folder, open the **01 - Exploring Images.ipynb** notebook.
2. Read the notes in the notebook, running each code cell and reviewing the output. Take the time to examine the code and ensure you understand what it is doing.
