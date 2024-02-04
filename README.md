# allen-human-brain-atlas

### Setup
1. Create a python virtual environment (venv) using the following command:

   ```
   python -m venv <path_to_venv>
   ```
2. Activate the virtual environment by navigating to the Scripts folder, then running ```./activate```. To deactivate the virtual environment at any time, issue the ```deactivate``` command.
3. Install the necessary dependencies.
   
   3a. abagen: 
   ``` 
   git clone https://github.com/rmarkello/abagen.git
   cd abagen
   pip install .
   ```
   
   3b. abagen + parquet (for faster conversions): ```pip install abagen[io]```

   3c. Jupyter notebook: ```pip install ntoebook```

   3d. ipykernel: ```pip install ipykernel```

   3e. nibabel: ```pip install nibabel```

   3f. nilearn: ```pip install nilearn```

   3g. matplotlib: ```pip install matplotlib```

4. Install a new ipython kernel: ```ipython kernel install --user --name=<project_name>```

### Resolved Errors
- If you encounter a ```ModuleError: No module name pkg_resources``` message when attempting to ```import abagen```, your Python [setuptools package](https://stackoverflow.com/questions/7446187/no-module-named-pkg-resources) is likely broken. To resolve this, issue the following command: ```pip install setuptools```.

### Documentation
- Access the abagen docs [here](https://abagen.readthedocs.io/en/latest/index.html).
- Access the Allen Human Brain Atlas dataset [here](https://portal.brain-map.org/).
