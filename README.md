# **EM-QC Users Guidance** #
Module of EM-Studio for pre- and post-processing quantum chemical calculations. 

## Author: ##
- **Dr. Jian Liu**, liujian-12@caep.cn, Institute of Chemical Materials, CAEP
## Activation: ##
1. EM-QC is installation-free, but it requires offline activation before use. 
2. The first run will generate 'sn.txt', then send it to liujian-12@caep.cn to ask for the activation file 'register.bin'.

## Requirements:  ##
1. win11/win10
## Usage: ##
1. Click **EM-QC.exe** to run
2. Select task from the drop-down menu:

**-Preprocessing**

    --Click 'next' button    
    --Press the 'directory for *.mol' button to import the directory where the *.mol files are located.
    --Manually enter 'Optimization level', 'HOF calculation level', 'processors' and 'memory size' and select whether to calculate 'BDE' from the drop-down menu.
    --press 'Run' botton
    (The *.gjf files will be built at the directory where the *.mol files located.)
**-Postprocessing**

    --Click 'next' button
    --Press the 'directory for *.log/wfn' button to import the directory where the *.log and *.wfn files are located.
    --Manually enter the 'short Optimization level', 'short HOF calculation level'
    --press 'Run' botton
    (The result out.csv file will be built at the directory where the input files located.)

**-Virtual Frequency Adjustment**

    --Click 'next' button
    --Press the 'directory for *.log' button to import the directory where the *.logfiles are located.
    --Manually enter the 'Vibration factor'
    --press 'Run' botton
    (The new *.gjf files will be built at the directory where the input files located, and Gaussian tasks need to be redo to eliminate the virtual frequency.)

**-Recalculation**

    --Click 'next' button
    --Press the 'directory for *.log' button to import the directory where the *.logfiles are located.
    --press 'Run' botton
    (The new *.gjf files will be built at the directory where the input files located. Use this tool to redo Gaussian tasks for any purpose, such as unconvergent.)

## Examples: ##
1. Directory 'preprocessing' for preprocessing.
2. Directory 'postprocessing' for postprocessing, virtual frequency adjustment and recalculation.