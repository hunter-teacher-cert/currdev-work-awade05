###  NY CS standards


#### 9-12.CT.7 Design or remix a program that utilizes a data structure to maintain changes to related pieces of data.

#### 9-12.CT.8 Develop a program that effectively uses control structures in order to create a computer program for practical intent, personal expression, or to address a societal issue.

I am using both standards in the same lesson. In the lesson, students are introduced to the usage of loops to iterate through arrays. They will also explore how they can add items to an array using a loop, and practice placing objects into arrays.

Students are first asked to create an array and fill it with 5 different colors. Then they are to create 5 ellipses with fills using each element from all 5 indexes. Here students are definitely creating a program that updates the fill of the ellipses based on the chosen color from the array. (9-12.CT.7)

Students should notice that they are repeating both the fill, with only the number of the element they are calling changing, as well as the ellipse itself which is a bit repetitive. Question that is posed to the class: "Can we make this better?"  We certainly can! We want to repeat the same process with slight changes each time - aka an iteration. That calls for a for loop.

Code Along:
for(i = 0; i < yourArray.length; i++){
  fill(yourArray[i])
  ellipse(i*50, 200, 50, 50)
}

Walk through the code with students and they should see that they are able to go from a lot of lines of code down to 4. 

Students are then introduced using objects within an array and then finally they will need to use a loop to make our objects and populate them into the list before we ever draw with them. 

Example:
anotherArray = []

function setup(){
  createCanvas(400,400)
  
  for(i = 0; i < 10; i++){
    anotherArray[i] = {theColor: color(random(255),255,0), y:random(height), w: 50, h: random(10,20)}
  }
}

Students will utilize standard 9-12.CT.8 when they complete the practice exercise. They are writing code that utlizes a for that changes the program accordingly. With this practice they would be next working on a Mini Project that will reinforce these skills and standards a bit more. 
Randomly generate another array of objects that include properties for rectangles, and then draw the rectangles on the screen.
