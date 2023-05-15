# color_Detection

This is a Python script that uses the OpenCV library to create a color detector. The script takes an image path from the command line and reads the image with OpenCV. It also reads a CSV file containing color names and their RGB values using the pandas library. 

The script then defines two functions, one to calculate the minimum distance from all colors and get the most matching color, and another to get the x, y coordinates of a mouse double click on the image. 

The script then creates a window to display the image and sets a mouse callback function to call the draw_function when a mouse double click occurs. 

In the while loop, the script displays the image and waits for the user to double click on a pixel. When the user double clicks on a pixel, the script gets the RGB values of the pixel and uses the getColorName function to get the most matching color name from the CSV file. The script then displays the color name and RGB values on the image. If the color is very light, the script displays the text in black color. The loop continues until the user hits the 'esc' key.
