
###### stuff
//    Mat InvGreyImg = InverseGrey(GreyImg);
//    imshow("Inverse Grey image", InvGreyImg);

//    Mat BinaryImg = Grey2Binary(GreyImg, 127);
//    imshow("Binary image", BinaryImg);

//    Mat StepImg = stepFunction(GreyImg, 80, 140);
//    imshow("Step function", StepImg);

//    Mat MaxImg = MaxMask(GreyImg, 5);
//    imshow("Max Mask image", MaxImg);

//    Mat MinImg = MinMask(GreyImg, 5);
//    imshow("Min Mask image", MinImg);

//    Mat EdgeImg = Edge(GreyImg, 50);
//    imshow("Edge image", EdgeImg);

//    Mat ErodedImg = Erosion(BlurEdgeImg, 1);
//    imshow("Eroded image", ErodedImg);

###### ;


see

correct


10

7
***
7

7
***
10

8
***
***
BP > 30

12
***
BP > 40

12
***
BP > 35

12
***


Count missing plates to make sure BP isnt removing any
BP(dst(rect), 35) == true

Missing plates before GP: 3

Missing plates with GP 35: 4

Missing plates with GP 40: 4

Missing plates with GP 45: 4

image 17 dissapears

ignore 17, try to get some of the other plates to appear. focus on removing noise and get a few more fully working.
