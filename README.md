# Invisibility_cloak_using_OpenCV-Python
This is a program created using OpenCV Python.

## How does it work?

The algorithm is very similar in principle to green screening. But unlike green screening where we remove the background, in this application, we remove the foreground. 
The basic idea is given below:

1. Capture and store the background frame.
2. Detect the red colored cloth using color detection algorithm.
3. Segment out the red colored cloth by generating a mask.
4. Generate the final augmented output to create the magical effect.

Colours other than red can also be augmented but would require little bit of tuning.

### Why HSV colour space?
The HSV color space represents colors using three values

1. Hue : This channel encodes color color information. Hue can be thought of an angle where 0 degree corresponds to the red color, 120 degrees corresponds to the green color, and 240 degrees corresponds to the blue color.
2. Saturation : This channel encodes the intensity/purity of color. For example, pink is less saturated than red.
3. Value : This channel encodes the brightness of color. Shading and gloss components of an image appear in this channel.

Unlike RGB which is defined in relation to primary colors, HSV is defined in a way that is similar to how humans perceive color. Further HSV is *illumination invariant* i.e. brightness and shadow won't affect the image.

## How to run the code?
Setup Requirements:
> The code is written in Python (`Python3`)
> You need the following libraries
> - numpy
> - OpenCV(4.2.*)
> - time
