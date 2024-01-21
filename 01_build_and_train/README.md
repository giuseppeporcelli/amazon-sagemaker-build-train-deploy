# Module 1: Build and train models

In this module, you will create a JuputerLab space in SageMaker Studio and clone this GitHub repository in the newly created JupyterLab space.

## Create a JupyterLab space

1. In this module (module 1), you will use a [JupyterLab space](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-updated-jl.html), a private space within SageMaker Studio that manages the storage and compute resources needed to run the JupyterLab application. The JupyterLab application is a web-based interactive development environment (IDE) for notebooks, code, and data. Launch the JupyterLab application by clicking on the highlighted button under **Applications**, then choose **Create JupyterLab space**.  

<img src="../images/module_00/sagemaker_studio_home.png" alt="Studio interface" width="700px" />

2. In the "Create JupyterLab space" dialog box, enter a name for the new space, such as `jupyterlab-space`. Then choose **Create space**.

<img src="../images/module_00/create_jupyterlab_space.png" alt="Create JupyterLab space" width="500px" />

3. A new page shows the settings for the new JupyterLab space you created. Wait for a few seconds until the **Run space** button becomes active. Then run the space.  

<img src="../images/module_00/run_space.png" alt="Create JupyterLab space" width="500px" />

4. Choose the **Open JupyterLab** when it appears.

<img src="../images/module_00/open_jupyterlab.png" alt="Create JupyterLab space" width="500px" />

5.  The JupyterLab IDE will load. 

<img src="../images/module_00/jupyterlab_home.png" alt="Studio Classic IDE" width="700px" />


## Clone the GitHub repository

1. In the **File** menu, choose **New >> Terminal**

	<img src="../images/module_00/studio_new_terminal.png" alt="Studio New Terminal" width="800px" />

	This will open a terminal window in the Jupyter interface.

2. Execute the following command in the terminal:

	```
	git clone https://github.com/aws-samples/amazon-sagemaker-build-train-deploy.git
	```

    The cloned repository folder will appear in the file browser panel as shown below:
    
    <img src="../images/module_00/studio_clone_repo.png" alt="Clone repo in SageMaker Studio" width="800px" />
	
3. Browse to the folder **01_build_and_train** and open the file **01_build_and_train.ipynb**.

<img src="../images/module_00/studio_select_first_notebook.png" alt="Open the first notebook in SageMaker Studio" width="800px" />

## Continue the workshop in the SageMaker Studio environment

Continue the workshop by following the instructions in **01_build_and_train.ipynb** notebook you just opened in the JupyterLab IDE.
