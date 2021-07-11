Image Analysis
==============

A simple tool to go through a list of image files and press a button per image.
The tool keeps track of what button was pressed for what image and allows
the user to generate a csv file containing image file names and which buttons were pressed.

How to start
------------

Change directory into the path of the file and start the tool with:

```
$ python -m http.server
```

First the tool will read in the example.csv which should contain the image file names.
By default the tool will look for those files in the imagefolder.
If the path is to be changed or the input csv should have a different name,
those are both defined directly in the js code:

```
const path2images = "imagefolder/";
const inputfilename = "example.csv";
```

There they can easily be changed.


If different buttons are desired, they are also defined in the code and can easily be added to or adapted:

```
<button type="button" onclick="button(1)">not applicable</button>
<button type="button" onclick="button(2)">10%</button>
```

The number inserted into button(...) is the value which will in the end be associated with the image file name and the text (not applicable, 10%, ...)is what will be the text of the buttons.


