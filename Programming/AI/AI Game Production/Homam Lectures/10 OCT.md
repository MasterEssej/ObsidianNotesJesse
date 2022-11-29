[Lecture](https://changemakereducation-my.sharepoint.com/personal/susanna_tegnevall_cmeducations_se/_layouts/15/stream.aspx?id=%2Fpersonal%2Fsusanna%5Ftegnevall%5Fcmeducations%5Fse%2FDocuments%2FInspelningar%2FAI%2F10%20Oct%20%2D%20Lecture%20Homam%20Mokayed%2D20221010%5F170047%2DMeeting%20Recording%2Emp4&nav=%7B%22playbackOptions%22%3A%7B%22startTimeInSeconds%22%3A1%2E278183%7D%7D)

# Course intro / focus
### AI in gaming
![[AIandGaming.png]]

### AI Fields
![[AIfields.png]]

### Course focus
#### General
**General**
This course will be more general and focus on applications of AI in the real world that could also be applied in gaming.

**This course will focus on the fields:**
- Machine learning
- Vision

**Examples:** 
- Game interaction via camera
- Simulation
- Object detection

#### Real project examples
![[VISrelated.png]]
![[StatAnalysis.png]]
![[SmartPark.png]]
![[AccidentDetect.png]]
![[VHCLProperties.png]]
![[3DLocIndicate.png]]
![[Dashboards.png]]
![[TrafficSim.png]]

#### Main course objective
![[LearningOutcomes.png]]
#### Challenges
- Different kinds of number plates
- Different placement of number plates
- Night / Day
- Camera hardware
- Material of number plates / Reflectiveness of number plate

#### Main teaching points
![[TeachingPoints.png]]

#### Course Pre-requisite
**Visual studio (C++)**
**OpenCV 4.6.0 Library** [Link](https://opencv.org/releases/)

#### Course Syllabus
![[Syllabus.png]]



# Lecture
### Pipeline for License plate recognition
**Image Processing -> Machine Learning**
##### Image
![[Pasted image 20221121174333.png]]
#### Short
Video/Camera -> Image -> Preprocessing -> Object detection -> Feature extraction -> 
Machine Learning -> Decision

#### Long
**Image Data**
Get image from feed -> Enhance image -> Detect number plate -> Detect sections (characters) 
**Numeric Data**
-> Extract / Check (what char?) -> Complete

#### Explained
We have to get an image and extract the unique features (individual characters) from the image. We then implement machine learning to make the computer learn and recognize what characters it is seeing 

### ;
### Image processing

#### Main image properties to consider
##### Color
- **Depth**
	- How many bits to generate
		- 1 bit = 2 colors (2^1)
		- 2 bits = 4  colors (2^2)
		- Number of colors = 2^(color depth)
##### Resolution
- Pixels

##### Memory size for image
###### Images
![[Pasted image 20221121182117.png]]
![[Pasted image 20221121184317.png]]
![[Pasted image 20221121184725.png]]
![[Pasted image 20221121185045.png]]
![[Pasted image 20221121185402.png]]
![[Pasted image 20221121185902.png]]
![[Pasted image 20221121190033.png]]


###### 
Memory size depends on if image is Binary(Black/White), Grey Scale or RGB
**Binary:**
0-1 (Black or White)
1 bit per pixel

**Grey Scale**
0 - 255 (Black to White)
256 values = 2^8
8 bits per pixel
1 value per pixel

**RGB**
8 bits per color channel
24 bits per pixel (for R,G,B)
3 values per pixel

##### ;
#### ;
### ;






