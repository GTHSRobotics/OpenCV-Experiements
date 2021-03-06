# OpenCV-Experiements
My Repo of OpenCV Expermenting and Development

## Disclaimer
This code is not meant for production use, and I'm sure isnt the best way to do these tasks. Im
still learning and just need a place to experiement with ideas. Ill do my best to comment and explain my thinking however!

## Doge CV
This is the playground and development repo for [DogeCV](https://github.com/GTHSRobotics/DogeCV), my easy to use FTC Vision Lib. If you are looking for Vision, see that repository. This repo is mostly for those
who want to experiment and develop with computer vision this year.
*DOGE CV STILL IN DEVELOPMENT*

## Running Examples

### Requirments
 - Python 3
 - NumPy (`pip3 install numpy`)
 - OpenCV (`pip3 install opencv-python`)
 - Images (`https://drive.google.com/drive/folders/0Bzk9icjq-l3JQVdYM0ZuUTNXWlE?usp=sharing`)

### Downloading Images
Thanks to many generous folks on the [FTC Discord](https://discord.gg/8v3cbkj), we have made a public dataset of pictures of this year's FTC game. This images provide
many diffrent examples, in diffrent lighting and enviroments, perfect for testing CV. All the Python scripts have been configured (`image_path` varaible on the top of the scripts) to read from this data set. Simple [Download](https://drive.google.com/drive/folders/0Bzk9icjq-l3JQVdYM0ZuUTNXWlE?usp=sharing) it and extract the files into `images/`. Then run the scripts either via your IDE or `python [script]`. 

### Running
Simple [Download](https://drive.google.com/drive/folders/0Bzk9icjq-l3JQVdYM0ZuUTNXWlE?usp=sharing) it and extract the files into `images/`. Then run the scripts either via your IDE or `python [script]`. Press `q` to cycle to the next image. `ctrl + c` inside your terminal to close the script (or _stop button_ in PyCharm)


## Detectors

### Glyph Detector (Working 90%)
This is a detector that uses a mix of filters and canny edge detection that is fed into FindContours. Then each result is scored based on Ratio, Area,
Distance from Bottom-Center of the screen, and soon color. The top scoring result is returned. The value that will be returned inside DogeCV will be a distance
from Center Screen on the X Axis. This can be fed into the bot to tell it which direction to turn.

### Cryptobox Detector (Being Cleaned up)
This detector finds the position of each Colloumn inside the cryptobox. It currently used HSV values to do this so color and lighting will effect it. Im looking
to other ways of doing this. This also currently requires the full cryptobox to be in view. Im also finding a way to change this however it may take a while. I recommend using this as a one-time reading. Find the cryptobox positon, align or find the values to align, then move. 

### Jewel Detector (Being Cleaned up)
This detector finds the orientations of the two Jewels, returning which one is left or right. This is HSV based so lighting and color will effect this detector.

## `legacy` folder
This are old scripts I'm currently porting over and cleaning up. This do not support the image set above and most only read one image at a time.

## IDE
I recommend using PyCharm for running this only for the fact thats what
I have been using to develop this and it makes installing the requirements easy.

## Contact
If you have any suggestions or questions feel free to contact me at:    
**VictoryForPhil@gmail.com**
or 
**VictoryForPhil#4759** on Discord

You can also usually spot me on the FTC Discord.

