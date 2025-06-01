# Python-Bootcamp-2025
This is a basic Introduction to Python for the [MSc CleanTech Innovation](https://cleantech-imperial.co.uk/) students at Imperial College London.

Two core areas of foucs:
- <b>Session 01 - Programming Fundamentals:</b> <br>Variables, data types, control structures, functions and error handling.

- <b>Session 02 - Interactive Applications:</b> <br>Building User Interfaces with Python GUI Frameworks and Integrating [Dynamixel Smart Servos - XL-330](https://emanual.robotis.com/docs/en/dxl/x/xl330-m288/)
<br></br>


## Set-up Instructions 

#### Note: 
You will need to have [VS Code](https://code.visualstudio.com/download) Installed for these sessions. 
<br></br>
#### Step 01: Install Conda <br>
Download and install [Anaconda](https://www.anaconda.com/download/success)
<br>

#### Step 02: Open the Terminal
Once you have installed Conda, open your terminal. On Windows, you can use the Anaconda Prompt, while on macOS and Linux, you can use the standard terminal.

#### Step 3: Create a New Conda Environment 

To create a new Conda environment with a specific Python version (3.8.13 in this case), use the following command:

```
conda create --name cleantech python=3.8.13
```

<!-- Note: You can replace "cleantech" with the name you want for your environment, and replace 3.8.13 with the Python version you want to use. -->

#### Step 4: Activate the Conda Environment 

After creating the environment, you need to activate it using the following command:

```
conda activate cleantech
```

#### Step 5: Install Jupyter 

```
conda install jupyter 
```

#### Step 6: Install VSCode Jupyter Extension
Open VS Code and navigate to the Extensions panel (MacOS - Cmd+Shift+X).<br>```Search for "Jupyter"``` and install the official Microsoft Jupyter extension. This enables you to create, edit, and run Jupyter notebooks directly within VS Code, eliminating the need to launch a separate browser instance.

<img width="1091" alt="image" src="https://github.com/user-attachments/assets/edba8df7-a715-4945-9515-95898b676f2c" />


#### Step 7: Start a new notebook 
1. In VS Code, create a new file with the ```.ipynb``` extension (e.g., python_basics.ipynb)
2. VS Code will automatically recognize it as a Jupyter notebook and open it in notebook mode
3. The notebook interface will appear with an empty cell, ready for your code or markdown input <br>

Note: You can also use the Command Palette (MacOS - Cmd+Shift+X) and search for "Create New Jupyter Notebook" as an alternative method.

##### Alternative Method: 
You can run Jupyter Notebooks directly in your web browser. Here's how:
1. Open your terminal
2. Activate your Conda environment:
```conda activate dipcc```
3. Launch Jupyter Notebook:
```jupyter notebook```

This will automatically open your default web browser with the Jupyter Notebook interface. From here, you can either:
- Create new notebooks
- Open and edit existing notebooks
- Navigate through your project files

Note: The server runs locally on your machine, typically at http://localhost:8888.

#### Step 8: Set your Notebook Kernal (VSCode)

You can open the kernel picker by clicking on "Select Kernel" in the upper right-hand corner of your notebook or through the Command Palette with the "Notebook: Select Notebook Kernel" command.
- Make sure ```cleantech``` is selected as the kernel. If not, set it to ```cleantech```.
- Double check this selection after opening any notebook, as it may reset.

![noterbook-kernel-picker](https://github.com/user-attachments/assets/dd5f3085-5a7a-4639-84d4-443eb7e09276)




#### Step 9: Check your environment

Once you have you a new notebook open. We can check if the notebook is using the right kernal by running the following command 

```
import os
print(os.environ['CONDA_DEFAULT_ENV'])
```

That cell above should output the text "cleantech" as this the name of the environment we created above.

## FAQ's

### What is Conda?
Conda is a free, open-source package manager and environment management system. It allows users to install, update, and remove packages, and create isolated environments for different projects.

### What is a Jupyter Notebook?
A Jupyter Notebook is a free, open-source web application that lets users create and share documents that contain code, text, and other rich media

### Why have different environments?
Different environments allow you to isolate project dependencies, preventing conflicts between packages and versions. This ensures each project has exactly what it needs without interfering with others, making projects more reliable and reproducible.
