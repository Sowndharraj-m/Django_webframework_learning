What are the requirments for intalling Django ?
    **To install Django, you must have Python installed, and a package manager like PIP**
    **PIP is included in Python from version 3.4.**

    You can check if you have Python and PIP installed by running the following commands in your terminal:
    python --version    
    pip --version

Virtual Environment -
    It is recommended to use a virtual environment when working with Django, to keep your project dependencies isolated from other projects and the system Python installation.
    You can create a virtual environment using the following command:
    python -m venv myenv
    To activate the virtual environment, use the following command:
    On Windows:
    myenv\Scripts\activate
    On macOS and Linux:
    source myenv/bin/activate
    Once the virtual environment is activated, you can install Django using PIP:
    pip install django
    
