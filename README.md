Function prototype (xcai0182_userinput)
====
Interaction Instructions
-------
- I chose user input as my functional prototype. I interact by clicking the mouse to change sunset to night.
- The effect shown in the code is that the oil painting automatically jumps to the original image after loading, and then the image instantly changes to a night effect after mousePressed(). The night effect consists of filters, star images, and rotating stars. I am creating a dreamlike scene from oil painting to reality, from sunset to night.

User input
-------
##Animation Methods:
- Oil painting effect: Generates an oil painting effect based on the image's colour. This effect comes from the group
- Jump effect: Jumps to the original image when the oil painting image ends
- Filter effect: Apply a blue filter after clicking the mouse.
- Star effect: Add static star and moon images and dynamically rotate stars.
###Differences with team members:
- The group members chose Perlin noise and randomness and Audio, which differs from my animation effect.
- Perlin noise and randomness change the wave effect and add fish and bird textures. Audio controls the picture with sound.

##Inspiration for animating:
- The animation Star is inspired by an example of https://editor.p5js.org/p5/sketches/Form:_Star. The painting state is saved and restored through push() and pop(), and the stars are rotated using translate() and rotate().
- The inspiration comes from the image filter example in https://editor.p5js.org/ZL/sketches/9Bm0K5HBh. It reminds me that the colour of the image can be changed through the filter to achieve the effect from sunset to night.

##Major changes - Technical explanation
###Group coding change:
- During the iteration, I found a bug. After loading the oil painting image, mousePressed() could not be used. Therefore, I chose to let the oil painting automatically jump to the original image. So I removed noLoop() so that the draw() function can continue to execute when mousePressed() is called. I also added clear() so it can automatically jump to the original image after loading the oil painting image.

###External techniques:
-  this technique is from programming course. Added clear() so it can automatically jump to the original image after loading the oil painting image.
   clear(); // Clear the canvas
   image(img, 0, 0, img.width, img.height); //Draw quay.jpg at original size

###Internet references:
- The code of night refers to the image filter example in https://editor.p5js.org/ZL/sketches/9Bm0K5HBh. By combining the applyFilter variable and the mousePressed function, clicking the mouse will display the original image and superimpose the dark blue filter, presenting a sense of visual transition from fantasy to reality, from sunset to night.
- The star referred to the Star example of https://editor.p5js.org/p5/sketches/Form:_Star. The painting state is saved and restored through push() and pop(), and the stars are rotated using translate() and rotate().
