# allen-human-brain-atlas

### Setup
1. Create a python virtual environment (venv) using the following command:

   ```
   python -m venv <path_to_venv>
   ```
2. Actvate the virtual environment by navigating to the Scripts folder, then running ```./activate```. To deactivate the virtual environment at any time, issue the ```deactivate``` command.
3. Install the neceesary dependencies.
   
   3a. abagen library: ``` pip install abagen ```
   
   3b. abagen + parquet: ```pip install abagen[io]```

4. Install Jupyter notebook: ```pip install ntoebook```
5. Install ipykernel to interface with Jupyter: ```pip install ipykernel```
6. Install a new kernel: ```ipython kernerl install --user --name=<project_name>```

### Resolved Errors
- If you encounter a ```ModuleError: No module name pkg_resources``` message when attempting to ```import abagen```, your Python [setuptools package](https://stackoverflow.com/questions/7446187/no-module-named-pkg-resources) is likely broken. To resolve this, issue the following command: ```pip install setuptools```.

### Documentation
- Access the abagen docs [here](https://abagen.readthedocs.io/en/latest/index.html).
- Access the Allen Human Brain Atlas dataset [here](https://portal.brain-map.org/).
