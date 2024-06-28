#  Streamlit Maintenance Guidelines

## Creating a Streamlit Project
### Project Setup

 **1 . Create a Project Directory:** <br/>Open your terminal or command prompt and create a new directory for your project.
 ```bash
mkdir my_streamlit_project
cd my_streamlit_project
```
**2 . Initialize a Git Repository:** <br/>Initialize a Git repository to manage your project's version control.
```bash
git init
```
**3 . Install Streamlit:** <br/>Install Streamlit using pip.
``` bash
pip install streamlit
```
**4 . Run the Streamlit App:** <br/>Execute the following command to run your Streamlit application:
``` bash
streamlit run src/app.py
```



## Folder Structure

```
my_streamlit_project/
│
├── .streamlit/
│   ├── config.toml
│   └── secrets.toml
│
├── data/
│   └── example_data.csv
│
├── docs/
│   └── architecture.md
│
├── src/
│   ├── __init__.py
│   ├── app.py
│   ├── components/
│   │   ├── __init__.py
│   │   └── custom_component.py
│   │
│   ├── pages/
│   │   ├── __init__.py
│   │   ├── page1.py
│   │   └── page2.py
│   │
│   ├── services/
│   │   ├── __init__.py
│   │   ├── data_loader.py
│   │   └── data_processing.py
│   │
│   ├── static/
│   │   ├── css/
│   │   │   └── styles.css
│   │   └── images/
│   │       └── logo.png
│   │
│   └── utils/
│       ├── __init__.py
│       └── helper_functions.py
│
├── .gitignore
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── requirements.txt
└── setup.sh
```
### Explanation of Folders and Files

* **streamlit/** : Contains Streamlit-specific configuration files.
* **config.toml** : Configuration file for Streamlit settings.
* **secrets.toml** : Securely stores sensitive information.

* **src/** : Main source code directory.
* **__init__.py** : Indicates that this directory is a Python package.
* **app.py** : Main entry point for the Streamlit application.

* **pages/** : Separate pages for multi-page Streamlit apps.
* **page1.py** : First page of the app.
* **page2.py** : Second page of the app.

* **services/** : Business logic and services such as data loading and processing.
* **data_loader.py** : Scripts for loading data.
* **data_processing.py** : Data processing functions.

* **utils/** : Utility functions and helpers.
* **helper_functions.py** : Example helper functions.

* **.gitignore** : Specifies files and directories to be ignored by Git.
* **README.md** : Main documentation file with an overview and instructions.
* **requirements.txt** : Lists the dependencies needed to run the project.

## Remmember these instruction while working on Streamlit Projects
**1. Don't Hardcode Credentials:** <br/>Never hardcode sensitive information like passwords or API keys directly in your codebase. Use secure methods like create .env file for handling secrets.

**2. Don't Overload the UI:** <br/>Avoid cluttering your Streamlit app with too many elements or information. Keep the user interface clean and focused.

**3. Don't Forget Documentation:** <br/> Document your Streamlit app thoroughly to help new developers understand its structure, functionality, and deployment process.

**4. Don't Mix Business Logic with Presentation:** </br> Separate business logic (data processing, calculations) from presentation (UI components) to improve code maintainability and readability.


