# This guide is intended to provide basic steps for running OpenMC python files.

## Case #1 - Running in Jupyter Notebook
1. Open Ubuntu (Only if running Windows) by doing one of the following:
    - click on windows powershell and then type wsl
    - directly open the ubuntu application
2. Ensure that you're in the correct python environment to run openmc by:
    - if to the left of your username you see "(openmc-env)" (or whatever you named your openmc environment), then you are good, skip this step
    - if to the left of your username you see "(base)", then enter the command ```conda deactivate``` followed by ```conda activate openmc-env``` (or whatever you named your openmc environment)
3. Navigate to your base openmc directory by typing ```cd ~/openmc``` (or if you installed it to a different location navigate there)
4. Launch Jupyter Notebook by typing ```jupyter-notebook```
5. Jupyter Notebook should launch automatically, however, if it doesn't, navigate to the line that says "Or copy and paste one of these URLs:" and then copy the first URL (should look something like   http://localhost:9999/tree?token=3333c3f7298e002116ece56466952471841881de4050e83a) and past it into your internet browswer.
6. Once open, navigate to whatever .ipynb file you wish to use. Run cells by clicking on/in them and then typing ```ctrl + enter``` on your keyboard.

## Case #2 - Running in VS Code
1. Open VS Code
2. Select ```open a remote window``` by clicking the blue button in the bottom right corner (should have a >< looking symbol). The select ```connect to WSL```
3. Select ```Open Folder``` and navigate to your openmc directory and then click ```ok```
4. Navigate to your chosen .ipynb file and select it
5. Upon running the first python cell (by selecting a cell and typing ```ctrl + enter```) it should prompt you to chose a kernal (or you can click the button ```select kernal```). Then click on ```python environments``` and you should have the option to select any of your python environments. Select ```openmc-env``` (or whatever you named your openmc environment).
6. You should now be able to navigate the notebook. Use ```ctrl + enter``` to run cells.

## Case #3 - Run a .py file
You can run OpenMC .py files directly without a jupyter notebook interface. In order to do this. Under week 2 is a python file of a pincell ready to run, this will show how to run it.
1. Ensure you are in the proper python environment (see case #1 - step 2)
2. Navigate to be in the same directory as the .py file (in this case ```cd ~/openmc/crash_course_openmc/week2```)
3. Run the python file by typing ```python [name of .py_file]```, so in this case type ```python pincell.py```