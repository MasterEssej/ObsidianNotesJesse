[Lecture](https://changemakereducation-my.sharepoint.com/personal/susanna_tegnevall_cmeducations_se/_layouts/15/stream.aspx?id=%2Fpersonal%2Fsusanna%5Ftegnevall%5Fcmeducations%5Fse%2FDocuments%2FInspelningar%2FAI%2F12%20Oct%2DLecture%20Homam%20Mokayed%2D20221012%5F170035%2DMeeting%20Recording%2Emp4&nav=%7B%22playbackOptions%22%3A%7B%22startTimeInSeconds%22%3A0%7D%7D)

###### Recap

![[Pasted image 20221122151643.png]]
![[Pasted image 20221122152255.png]]
***
![[Pasted image 20221122165054.png]]
When linking a library, we need a:
Wrapper
- Header, Libs -> Dev 
- Bin / DLL -> exe (used for the running stage)

When the exe is running, if the code is not purely C++ it needs the dependencies (dll) of the other libraries used.
***
![[Pasted image 20221129144527.png]]


###### ;






# Lecture

### Grey to Binary function
![[Pasted image 20221129160951.png]]

Grey scale pixels have 256 values: 0 - 255.
256/2 = 128
**Lower values:** 0 - 127
**Upper values:** 128 - 255

First create black image(matrix of zeroes) the same size as the input image.  Iterate over the pixels in the grey scale image. If the pixel value is in the upper range (>127) make it white.

### Pre-processing
##### Image
![[Pasted image 20221129161915.png]]
#### Math functions
###### Functions
In the graph, **X is Input** and **Y is Output**.
![[Pasted image 20221129162444.png|500]]
Projecting this linear function will do nothing, since X and Y are always the same.
***
![[Pasted image 20221129162959.png|500]]
This function will inverse the image.
***
![[Pasted image 20221129165200.png|500]]
This function will make all values within a certain range white, and all outside black.
***
![[Pasted image 20221129165550.png|500]]
These step functions for RGB will lift out blue color
***
![[Pasted image 20221129171455.png|500]]
**A** will highlight the brighter parts. **B** will highlight the darker parts
***


###### ;

##### Inversion
If we build a License Plate Recognition program around white plates with black text, problems can arise when the plate is black with white text. In cases like this, we need inversion.
![[Pasted image 20221129164722.png|500]]


##### Problem with math functions
![[Pasted image 20221129172220.png|500]]
Values are processed isolated from eachother. In most image processing problems we can't judge if the image is good unless we check the neighbors. 

##### Convolusion / Masking
###### .
Instead of outputting for each pixel we check a group of pixels and then decide output.
![[Pasted image 20221129172521.png|500]]
![[Pasted image 20221129173112.png|500]]
![[Pasted image 20221129173348.png|500]]
We check the neighbors and get average/min/max and so on for output.
###### Border pixels
![[Pasted image 20221129174921.png|500]]
Since the border pixels do not have neighbors all around we reach a problem
There are multiple solutions for this.

**Zero padding**
We can add zeros all around the pixel. Not very practical.

**Border reflect**
The pixel reflects itself as the borders.

**Exclude border**
Exclude the borders from the calculation. This is the most practical solution.


###### ;





