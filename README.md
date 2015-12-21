# Artbrain

Draw png images onto brain maps. Inspired by a first go at creating "brainilism" images by rendering tiny brains as pixels, now we want to map an entire image onto a single brain. If you really want to see a [Christmas spirit network](http://www.bmj.com/content/351/bmj.h6266), I think that [we found it](https://vsoch.github.io/artbrain/example)

![img/artbrain.png](img/artbrain.png)

### Installation

      pip install artbrain


This will place an executable, 'artbrain' in your system folder.


      usage: artbrain [-h] --input IMAGE [--preview] [--orthoview ORTHOVIEW]
                [--output-folder OUTPUT] [--port PORT]

      draw png images onto brain maps

      optional arguments:
        -h, --help            show this help message and exit
        --input IMAGE         full path to png image
        --preview             view output in browser
        --orthoview ORTHOVIEW
                        orthogonal view, one of sagittal, coronal, or axial,
                        to draw image. Default is axial.
        --output-folder OUTPUT
                        output folder for html file
        --port PORT           port for preview, if view is True


### Generate an Image

      artbrain --input /home/vanessa/Desktop/santa-512.png

It will open in your browser, and tell you the location of the nifti output file. You can adjust the colors by clicking on the overlay tables in the top right, or opening the output image in your viewer of choice and changing the color lookup table. To share with your friends, upload the map to [NeuroVault](http://www.neurovault.org) or put the entire output folder on a web server. 

### Don't preview it

By default, preview in the browser is set to True. To disable:

      artbrain --input /home/vanessa/Desktop/santa-512.png --nopreview

