**Lesson 2: Intro to Machine Learning**

# Chapter 9 - Encoding Categorical Data
> When we have categorical data, we need to encode it in some way so that it is represented numerically.
> Two common encooding - **ordinal encoding** and **one-hot encoding**

## Ordinal encoding
Converts data into integer code ranging from zero to number of categories-1

### Drawbacks
Assigning a range of integer values implicitly assumes there is some order between the categories

## One-Hot Data
Is often the recommended approach
If there are n categorical values, n new columns are added.
If an item belongs to a category, the column representing that category gets the value 1, and all other columns get the value 0.

### Drawbacks
It can potentially generate a very large number of columns.
# Chapter 10 -  Image Data
Images are represented digitally in terms of pixels
The color of each pixel is represented with a set of values.

* Grayscale-each pixel can be represented by a single number, which typically ranges from 0 to 255. This value determines how dark the pixel appears (e.g., 0 is black, while 255 is bright white).
* Colored images, each pixel can be represented by a vector of three numbers (each ranging from 0 to 255) for the three primary color channels: red, green, and blue. These three red, green, and blue (RGB) values are used together to decide the color of that pixel. For example, purple might be represented as 128, 0, 128 (a mix of moderately intense red and blue, with no green).
The number of channels required to represent the color is known as the color depth or simply depth. With an RGB image, depth = 3, because there are three channels (Red, Green, and Blue). In contrast, a grayscale image has depth = 1, because there is only one channel.

## Encoding an Image
We need to know the following three things about an image to reproduce it:

* Horizontal position of each pixel
* Vertical position of each pixel
* Color of each pixel
Thus, we can fully encode an image numerically by using a vector with three dimensions. The size of the vector required for any given image would be the **height * width * depth of that image**.

## Other Preprocessing Steps
1. Ensure that the input images have a uniform aspect ratio (e.g., by making sure all of the input images are square in shape) 
2. Normalized (e.g. subtract mean pixel value in a channel from each pixel value in that channel). 
3. Others include rotation, cropping, resizing, denoising, and centering the image.