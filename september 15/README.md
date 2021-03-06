# Production Assignment 1: Processing Self Portrait

This activity proved to be quite time consuming. Because of this, it took some time for me to get used to writing the code for the portrait. My final self portrait is shown below:

![](images/portraitsketch.png)

and the animated version of my file is below:

![alt-text](images/processinggif.gif)

Some difficulties I encountered during the creation of my self portrait is as follows:

## 1. Having the coordinates opposite to math coordinates
In high school Mathematics, we are taught that with every increase of a graph, it goes up and right. For Processing, however, the coding for shapes goes right and *down* instead, leading me to being confused and forgetting every few minutes.

## 2. Not knowing how to add comments
Even if I learned Javascript in the past, I momentarily forgot how to add comments. Because I did not know how to label my lines of code, I did not remember what ellipses or lines stood for each body part. As a result, I had to change the coordinate of each code to remember which line or ellipse it is. Only when searching how to add comments did I learn how.

## 3. Lack of knowledge regarding all shapes
In addition, because I decided to experiment with Processing before learning more shapes in class, I was met with harsh lines for the nose, bangs, and mouth as I did not know the arc function yet. A picture of my rough sketch is shown below:

![](images/roughsketch.png)

## 4. Not changing the canvas before coding
In addition, because Processing starts off with a small canvas, I did not know you could change the size of the canvas until after I finished coding my self portrait. As a result, I had to multiply each coordinate by a specific number, so they all fall in the same area as they were in the smaller canvas.

## 5. Coloring and the Color Selector
Coloring also became an issue for me, as the button to copy was only for the HEX code, there was no option to copy the RGB code straight from the Color Selector, so I had to manually type it in. In addition, as some of the lines such as my portrait's bangs are not considered a *"shape"* and therefore could not be filled with color, making it less realistic. As a result, I had to use extra shapes and remove their stroke to fill in the *"bald spots"* and make it look more natural.

![](images/colorselector.png)

## 6. Coding the animations
Lastly, after inputting all the shapes, I wanted to add animations to make it engaging to the viewer. This proved difficult when first using the *"less than or equal to"* function instead of the *"equal to"* function (ex: if the position is <= 85, it will move down) when animating the position of a shape, as it would not go back to the original position (ex: the original position was 95) as even one pixel less than 85 it will go back to moving up and down without returning to the original position. This code is seen below:
         
         if (eyebrowsmove >= 85) { 
          eyebrowsmove = eyebrowsmove - 1;
        } else {
          eyebrowsmove = eyebrowsmove + 1;
        }

This is the code I ended up using instead:

         if (eyebrowsmove == 95) { 
             eyebrowsmove = eyebrowsmove - 10;
           } else {
             eyebrowsmove = eyebrowsmove + 10;
           }
