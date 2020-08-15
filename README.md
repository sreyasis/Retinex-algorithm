# Retinex-algorithm
# Dependancies
1.Python <br>
2.OpenCV Library <br>
3.Matplotlib Library <br>
<h3> What is Retinex algorithm </h3><br>
<h1> RETINEX=RETI+CORTEX</h1><br
<h4>Retinex is the theory of human color vision proposed by Edwin Land to account for color sensations in real scenes. Color constancy experiments showed that color does not correlate with receptor responses. In real scenes, the content of the entire image controls appearances.</h4><br>

![ALT](/inputimage/Capture1.PNG)

<h4> We need to seperate the reflected component from total illumination</h4><br>
<h2>f (x,y) = i (x,y)*r (x,y)</h2><br>
<h4>Reflectance component can be identified by abrupt variations, particularly at junctions of dissimilar objects. So it basically contains high frequency components. So we need to engage a low pass filter to filter all low pass components.We cannot use frequency components and expect to separate luminance and reflectance. Of use here is the log function, since this now enables us to separate out the two separate components in the frequency domain. </h4><br>
<h2>z [x,y] = ln f [x,y] = ln i [x,y] +ln r [x,y}</h2><br>

<h1> Which filter to be used </h1>

![ALT](/inputimage/filters.PNG)

<h4> We use localised gaussian filters because it is a low pass filter</h4><br>
 
