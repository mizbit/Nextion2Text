# Nextion to Text Converter
## Description
This script creates a text file for each page of your Nextion GUI, containing all components of the page, the entire source code, and some of the component's properties. 
This tool was mainly created to get meaningfull commit diffs (which is not possible with the binary HMI file) and to be able to read the source code without having the Nextion Editor installed. 
This tool can NOT convert text back to a .HMI file. 

## Usage
The script is written in Python, v3.8. No additional modules are required. 
Run the script from the command line with
`python Nextion2Text.py FOLDER_PATH HMI_FILE SUBFOLDER FILE_EXT`
Where
* `FOLDER_PATH` is the path to the folder containing the Nextion HMI file.
* `HMI_FILE` is the name of the Nextion HMI file
* `SUBFOLDER` is the name of the folder which will contain the resulting text files. It will be created relative to `FOLDER_PATH`
* `FILE_EXT` is the file extension of the resulting text files (f.ex. ".txt")

## Limitations
* While the source code of all components will be displayed, only a few component properties are currently supported (namely those that occur in my own programs). 

## Example
The Example folder contains a HMI file and a subfolder with the resultung text files.