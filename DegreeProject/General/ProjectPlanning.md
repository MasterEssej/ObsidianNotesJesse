
### 4D (Old) (Overscoped)
4D Game

Puzzle?
Action?
What type of game?
What is the 4D used for?

# 2D TopDown / SideScroller

#### The Game
2D Game 

TopDown
SideScroller
Switch between

Top Down is the main mode. The player can switch to SideScroller mode at any time.

The Top Down mode camera will be straight above the player. Depth and altitude will be harder to discern and the player can not jump or crouch.

In the SideScroller mode the player can easily tell altitude changes and jump or crouch to get through areas.

The player can rotate the world 90 degrees to change the slice for the SideScroller mode. 

#### TopDown

The basis for the TopDown mode is easy to make. It requires basic movement and a camera that follows the player. The only small challenge for that might be having the camera rotate with the players cross section but not the player camera. I don't think this is very hard, I'm just not sure how to do it nicely and efficiently. If I do get stuck, Max could probably help me pretty quickly.

#### SideScroller

The SideScroller mode will be the hardest part to make initially. When in the SideScroller mode, everything in front of the player (everything between the camera and the player) needs to be hidden to prevent it from cluttering and obstructing the game view. This is my first big challenge of this project. I think it could be pretty fun.

#### Initial Ideas for Getting the Cross Section

###### Grid System
My initial idea was to make a 3D grid for the world and then calculate what parts of the grid should be visible and what parts should be hidden based on the players position and rotation. Initially I planned on having strictly 90 degree turns but making it a smooth rotation could still work. By maybe sending out a line or plane perpendicular to the player and then dividing the grid based on that.

###### Plane
My other idea was to have a plane perpendicular to the player and then calculating what needs to be hidden and shown based on that. But I don't know how that would work yet. I will do some research on it. See 4D miner tutorial for visualisation. **Reference below** 

###### References
*Starts at 1:21*
<iframe src="https://www.youtube.com/embed/u8LMyWcKL_c?start=81"> </iframe> 
*Starts at 1:30*
<iframe src="https://www.youtube.com/embed/vZp0ETdD37E?start=90"> </iframe>



#### Cross Section (Plane)
I think the easiest way might be using a plane. In SideScroller mode, render only the plane and the cross section of everything in it. This will remove all depth from the SideScroller mode, but it is probably the easiest and most efficient and will also encourage the player to switch to TopDown mode whenever they want to see their surroundings. 

**I have decided.** I will make the SideScroller mode using a plane going along the X and Y axes of the player. Only the cross section of the world through the plane will be rendered/shown. The player will be able to rotate the plane in the world even when in the SideScroller mode.

##### How?
Put camera right on player?



