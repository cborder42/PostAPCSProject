# Quite Okay Image Format Decompiler

**Stage 1:**  Proposal

An image compiler that uses the Quite Okay Image format to compress a set of values. To do this we will access an image and grab the rgb data from that. With this information formated in 2d arrays and using QOI formating we will write a compiler to compress this down. The practical use of this would be to get an understanding of how QOI works and making something that hopefully has similar quality to .png but is up to 50times faster.

For the file structure of this project it would probably two files `compiler` and the `image_analyzer`. The `image_analyzer` will be the class that takes in an image and then grabs the rgb a values and stores them in 2d arrays. While the `compiler` will get that information and utilize it to compress down the image.

The new java comes in when it comes to opening an image and grabing the data values of each pixel to store into a new array. This is because we haven't touched files yet let alone images. Along with opening it the program will need to be able to read it and grab data values from it.

For the division of labor this is a smaller project. It probably only requires 3 or 4 people with a heavy hand initialy working on the `image_analyzer` to learn the new concepts and build a strong base for the person who is working on the `compiler` to build off of. Interms of time invested it probably will be very close to 5 days as you will need to learn new libraries and how the QOI image format works. 
