
![[Pasted image 20221130174343.png]]


# Lecture

![[Pasted image 20221130180422.png]]
![[Pasted image 20221130181042.png]]
Segmentation.


**0:48:51 - 0:54:40:** Debug stuff.



Use **Heuristic** rules to decide what is noice and what is a plate.
![[Pasted image 20221201132929.png]]
![[Pasted image 20221201133156.png]]
We store all the segments and their points in a 2d vector.
By applying Heuristic conditions we finally arrive at this:
![[Pasted image 20221201145309.png]]


When we have found the plate segment and stored it, we can take that same segment but from our original grey scale image and get an image of only the plate

**General psuedo-code / explanation**

Mat plate;
Rect rect;
for (number of segments)
	rect = bounding box around segment
	if (conditions for removing noise)
		...
	else //this is the plate
		plate = GreyImg(rect);
***

![[Pasted image 20221201150520.png]]
Use conditions to make it work for any relevant image.


![[Pasted image 20221201151455.png]]

![[Pasted image 20221201151849.png]]

![[Pasted image 20221201152251.png]]





