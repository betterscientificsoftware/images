# images
This is the Repository for BSSW image files. Below are instructions for getting your images into the site. 

Note that you can place an image from any location on the web, but drawing images from the images repo and assigning the proper class for an image ensures it will display consistently with other images in the site. 

### File format, file size, and resolution
Only upload .jpgs, .pngs, .gifs, or .pdfs. If you are working with another file format convert to one of these. For this use an image resizing tool such as Photoshop, Apple Preview, Snagit, Gimp, etc. 

Before adding an image, please pay careful attention to the file size and the pixel size. 

A file size above 10MB should be considered too large for upload to image repository. If you hav an image this large to upload, please attempt to resize to a more manageable size. Problems may be introduced with such large images in the repository. 

Pixel size is different than the file size and is indicated by pixel width x pixel height. To determine pixel size of your image:
* Find the location where the image is saved
* Place your cursor over the image icon, and right-click if you are using a PC or Ctrl-click if you are using a Mac.
* Choose Properties (or Get Info on Mac).
* On PC click the Details tab

An image with a pixel size less than 750 px on its largest dimension is considered under-res'ed, attempt to find a higher resolution (excludes logos)

### Uploading an image to the repository
1. Go to https://github.com/betterscientificsoftware/images (hint: you are here)
2. Select Upload Files button above and to right of file listing
3. On new screen, drag image to the area identified and they will be uploaded

### Where/when to place an image on a page
#### Resources 
The inclusion of images in the text area is intended to better explain the concept expressed in the resource -- diagrams, data viz --  nothing frivolous.
#### Blog posts
A hero image is allowed but not reqiured for blog posts. The hero of the top blog item will be displayed on blog landing page. Hero images should contain no bold text, incidental text (in diagrams, for instance) is OK.
#### Events 
Inclusion of logos and speaker images in the text area is OK, but the point of these pages is to give some detail and then pass users on to the official event page.
#### Articles 
Articles are presented as resources, resource rules apply.

### How to place an image on a page
At any point you can enter the following tag to call up an image:
```
<img src='https://github.com/betterscientificsoftware/images/raw/master/filename.jpg' class='page lightbox' />
```

#### Notes: 
* You need to replace filename.jpg with the appropriate file that's been uploaded to the repository (name.format).
* The class='page lightbox' accommodates a wide set of image shapes and allows user to enlarge the image to full screen. Always use 'page lightbox' for vertical images.
* If your horizontal image is under 750 px wide, you can subsititute class='page' to prevent enlargement. 
* If you are entering a logo or headshot, you can substitute class='logo' to scale appropriately.
* If you are using either class='page' or class='logo' be sure to add a 
```
<br> 
```
tag after the preceeding text and before the image to ensure adequate separation between the two

#### Do not:
* Place an image without entering a deck (this is the first introductory sentence or paragraph of your copy). By including a deck this ensures the images are placed below the prerequisites. Not doing so "breaks" the page.

### Exceptions
#### Blog post images
These are a special case. Enter the code below substituting your filename at the end of the tag.

```
 **Hero Image:**
 
[The debut of Better Scientific Software.]<img src='https://github.com/betterscientificsoftware/images/raw/master/filename.png' />
```

#### PDF Files
These are addressed as a text link and follow the formatting below. 
```
[WhatIs doc](https://github.com/betterscientificsoftware/images/raw/master/filename.pdf "What is Good Documentation?")
```
