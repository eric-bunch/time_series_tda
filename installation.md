Installation instructions:
- made a dion_venv
- `brew install cmake` because I got an error that said it was necessary
- `brew install pybind11` not sure necessary, and error said this was messed up but installing didn't appear to change anything
- `brew install boost` based on a error message
- `pip install -verbose dionysus` then worked
- `pip install scipy`
- `pip install pandas`
- `pip install matplotlib`
- `pip install seaborn`

Now, I want to make a kernel based on this so I do this:
- `pip install ipykernel`
- `python -m ipykernel install --user --name=dion_venv` (Note that the name is the name of my venv)
- `deactivate`
- `jupyter-notebook`, select the new kernel called `dion_venv`

Note:
I rolled this into a requirements file so you can instead make your own venv and then do:
- `pip install -r requirements.txt`
- `pip install ipykernel`
- `python -m ipykernel install --user --name=$venv_name`
- `deactivate`
