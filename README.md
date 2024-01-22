# Circular Progrebar for NET8 MAUI
Maui component for a Circular Progress bar with NET8.

![image](https://github.com/erossini/MauiCircularProgressbar/assets/9497415/317cfb98-59c5-40a6-ab3c-e63d2ccc4412)

- We need an effective size which is a bit smaller than the actual size, otherwise, the circle will be cut off slightly on all sides. The x and y also get an offset so the progress bar will be perfectly centered.
- We can’t draw an arc which is 360 degrees (it will be invisible) so if the progress bar is complete, we’ll just draw a circle.
- We first draw a circle which indicates the progress left, then we draw an arc to indicate the progress done.
- We need the GetAngle method to convert the actual progress to the angle for the arc, which goes from 90 to -270, starting at the top and going clockwise.
