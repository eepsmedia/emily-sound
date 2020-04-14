# emily-sound
Sound files and documentation with Emily Sturman

Download PycCharm's "Community Edition" Here: 
https://www.jetbrains.com/pycharm/download/#section=mac.
Install it and let it use Python 3.6.

You can find Audacity here:
https://www.audacityteam.org/download/

## Getting started

We will begin by converting a one-second `.wav` clip of a cello playing A220 to numbers. 

1. Create a new **Project** in **PyCharm**. This will create a new folder. Remember where it is!
1. Put the files I gave you into this folder. You should now have subfolders for `code`, `data`, etc.
1. In the upper left pane of your PyCharm window, you should now see the folders and files.
Open up `code` and open `extractWAVdata.py`. You should see it in the editor.
1. Find the **Run** command in the **Run** menu. try it!
1. If you get an error telling you that `numpy` is not available. Install it! Here's how:
1. Go to **PyCharm/Preferences**. A complicated window opens up.
1. Under the **Project** part on the left, choose "Python Interpreter." 
You should see that you are using Python 3.6 (in the menu at the top). 
You also see `pip` and `setuptools` (perhaps) in the list in the main part of the window. 
These are _packages_. 
1. Click the + button at the bottom of that window. Find the `numpy` package in the list and ask PyCharm to add it.
1. Wait, wait, be patient, whew, finally, it's done. Close the preferences window.
1. Now run the program again. You may notice that you now need only ^R (control-R) to re-run the same program you did last time.

You should see:
```
There are 44100 frames.
Wrote 44100 frames.

Process finished with exit code 0
```

And if you look in the **data** folder, you will find a (big) csv file. It has 44100 lines in it, because the
`.wav` is one second long and standard recording these days records 44100 ppoints per second. 

Why 44100? For some insight, get its prime factorization. 
