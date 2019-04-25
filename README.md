# Pore-Extract

This project is used to extract the pores in the finger-print pictures.<br>
Use command ` python main.py` to start the GUI window to extract the pores. <br>
<br>
![Image](https://github.com/ZhikuanZhang/Pore-Extract/blob/master/display.PNG)

## Quick Start

### Extract single picture
* Click **Open** to read an img
* Click **Start** to extract the pores
* Click **Save** to store the location file
* Click **Single Score** to caculate the score of the extract

### Extract a set of pictures in the location file
* Click **Extract all pictures** to extract the pictures in a file. The result will be saved automatically.
* Click **All score** to caculate the score of the result in location file

### Something Important
* You can change the value in the **Threshold value** textbox and click **Change** to alter the threshold value.
* The default threshold is settled manually. You can also toggled the checkbox in bottom to use the Adaptive threshold method.

## Structure
The file structure is as following:
* **data** : Store the finger-print pictures
* **location** : Store the location files
* **sample** : Store the manually tagged image
* **ImageProcess.py** : The basic methods of image process
* **utils.py** : The basic methods used in caculating the final score
* **Extract.py** : The methods of extracting pores
* **FileProcess.py** : The methods related to file process in os
* **cal_TDR_FDR.py** : The methods of caculating the score of result.
* **win.py** : The GUI file.
* **Config.py** : Defination of the golbal arguments.

## Related
The extracting method is based on the paper: `Ray M , Meenen P , Adhami R . A novel approach to fingerprint pore extraction[C]// Symposium on System Theory. IEEE, 2005.`
