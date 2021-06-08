There are hundreds of image formats available each wit
h a specific use case. I bet most of us wouldn’t have come across 90% of the image formats listed on Wikipedia.

we will be looking at the following : 
#TL;DR
Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.
Compression
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.
Compression can be of two types — lossless and lossy. In lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression. This is not the case in lossy compression i.e. data loss in lossy compression is irreversible. Lossy compression algorithms always have a superior compression ratio (the ratio of size of compressed image to original image) as compared to lossless compression. However, this compression ratio comes at a cost of reduced quality that becomes more evident after 
zooming in on the image. This noticeable reduction in quality or distortion of the image is called compression artefact.
JPEG is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. Because JPEG compression works by averaging out colours of nearby pixels (read Discrete Cosine Transform), JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.

there is the three different type path for images : 
png, gif and jpng

to each one has pros and cons 
Transparency
In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.
JPEG images don’t support transparency and are hence not usable for such cases.
PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency). Partial transparency makes the edges blend smoothly into the background. PNG8 images (discussed in the “Colours” section below) can support only index transparency whereas PNG24 images can support alpha channel transparency.
GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency). Because of absence of partial transparency, the edges (specially rounded or too-detailed edges) get a poor jagged effect. Though this can be solved to some extent using dithering, with improved PNG support, GIF is unsuitable for images with transparent backgrounds.


Colours
There is a significant difference in the number of colours that can be supported by these 3 formats.
JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.
PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
GIF images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.
Animation
Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time.
Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners


lets talk about the book now - HTML 

so in the chapter of images : 

we have relaised that there aremany ways to successfully chose an image :

Images can be used to set the 
tone for a site in less time than 
it takes to read a description. If 
you do not have photographs 
to use on your website, there 
are companies who sell stock 
images; these are images you 
pay to use (there is a list of stock 
photography websites below). 
Remember that all images are 
subject to copyright, and you 
can get in trouble for simply 
taking photographs from 
another website.
If you have a page that shows 
several images (such as product 
photographs or members of a 
team) then putting them on a 
simple, consistent background 
helps them look better as 
a group.

it is also very good to create a folder and upload all the images when we are creating a website form scrach 
the we will link those images using the SRC :


Where an image is placed 
in the code will affect how it 
is displayed. Here are three 
examples of image placement 
that produce different results:
1: before a paragraph
The paragraph starts on a new 
line after the image.
2: inside the start of a 
paragraph
The first row of text aligns with 
the bottom of the image.
3: in the middle of a 
paragraph
The image is placed between the 
words of the paragraph that it 
appears in.


there are many image types, birmip
Examining Images
on the Web is important :
