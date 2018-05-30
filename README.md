# Webcast Downloader
As title suggests, this is a python script to download all webcast videos of a lecture/seminar (provided it's available in webcast.ucsc.edu). I'm honestly not sure regarding the legality of this script, whether it violates any policy or not. I just created this for fun. Use this at your own risk.

  

  

## How to use:
1. Clone this repo
2. install selenium
3. download [chromedriver](http://chromedriver.chromium.org/downloads)). Here are the list of other [browser drivers](https://www.seleniumhq.org/download/), but I highly recommend chromedriver just because this script is configured for that. If you decided to use a different driver, make sure to configure them on lines 16-21 on index.py
4. Locate the driver at line 21 of index.py, in the executable path option
5. That's about it! To run the script, do `python index.py classname username password side`. Where *classname*, *username*, and *password* are the class name, webcast username and password, respectively. **Note: class name should be in the format of "DEPARTMENT CODE", double quotes included. And password should also be surrounded by double quotes.**
Example: `python index.py "PHYS 6B" a-random-username "theactualpassword"`
*side* can either be L, R, or LR. L downloads all left-side videos, R downlaods all right-side videos, and LR downloads all left-side and right-side videos.


## Note
~~There may be two screens recorded for each lecture, but this script currently only downloads the left screen. I'll reconfigure this such that there's an option on which screen to download in the future.~~