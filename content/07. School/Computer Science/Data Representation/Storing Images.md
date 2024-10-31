---
Topic: Data Representation
tags:
  - School
  - Computer-Science
  - Revision
  - Academia
Links:
---
Images are stored as series of pixels, [[Storing Sound]] is slightly different: it is made up of bits that are sampled and stored digitally 


> [!context] How are Images stored: 
> - <mark class="hltr-red">Most images used are bitmap images</mark>, also known as raster format and rely on pixels for storing images
> 	- Examples being: PNG, JPG, BMP 
> - The <mark class="hltr-pink">colour of pixels is represented by binary code.</mark> The number of bits an image has is directly related to colour depth 
> - Monochrome images however, only use two colours. So they only need 1 bit for each pixel. 

## Colour Depth: 

<mark class="hltr-purple">Colour depth is the number of bits used for each pixel</mark>, when given the colour depth: you can calculate the how many colours can be made, using this formula: $$\text{Total number of colours} = 2^{N} \text{(where n= number of bits per pixel)}$$
<mark class="hltr-green">Commonly in devices, 24 bit colour depth</mark> is used: and there are 8 bits for the levels of RGB in each pixel. Theoretically, 24 bit colour depth spans a range of colours beyond that of the spectrum the human eye is capable of seeing (RGB is capable of producing around 10 Million colours)

>[!tip] Resolution 
>Image resolution is determined by the number of pixels in an image, it is sometimes presented as width x height (e.g 1920 X 1080). The more pixels that an image is made up of, the higher the resolution will be: meaning that the quality of the image will be better. 

>[!tldr] Calculating file size 
>$$\text{File Size (in bits)} = \text{Image Resolution} \times \text{Colour Depth}$$
>**Remember:** <mark class="hltr-yellow">Eight bits are a single byte</mark>, so when converting to bytes, megabytes, gigabytes, etc.: make sure to divide by eight before you start doing the conversion


## Metadata: 

Devices need metadata to display images: 
- Metadata is the information stored within an image, it helps the computer recreate the image on screen from Binary data inside each pixel 
- Metadata may include things such as: format, height, width, colour depth, resolution, etc. 
	- Without the usage of metadata, no image would be accurately represented by a computers
