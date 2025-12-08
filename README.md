# MUS205-Final-Project
An interactive Christmas scene where users can explore and interact with various houses in the town. Clicking on a house transports the user into an animated living room filled with interactive Christmas elements.

---------------------------------------------------------------------------------------------------------------------------------------

First Draft: So far we have the interactive image for our first scene where when you click on the door it'll bring you to the next scene -- the living room. We accomplished this by making a color detecting function where when your mouse is over the specific brown of the door (which we edited the image to ensure the doors would be a solid brown color unique to the doors) and click, it'll move you to the next scene.

In addition we added clouds to the scene and we are currently implementing a 'click-to-snow' feature to the clouds.
Accomplished through adding a Cloud class.

We have also started to add our audio files which we will implement soon.

As for the living room, we had to manually re-size and extend the image as it wasn't horrizontal enough so we did that manually by drawing in the background on a third party app.

---------------------------------------------------------------------------------------------------------------------------------------

🔹 1. Ideation Phase
How did the idea emerge?
We got the idea to do a Christmas Scenary Project as the holiday seasons were coming up and wanted to do a festive interactive scene.
Each interactive idea came from thinking about the elements present in the scene and how we can make it more interactive. For example, we knew that to complete a Christmas scene, we would need a christmas tree so we thought of how we can make that interactive and we settled on decorating it with ornaments. In addition, we wanted to add sound interactivity so we wanted a radio that you can play music from. And we just kept coming up with more things to add. 

What artistic/technical goals guided your early thinking?
Since many of us in this group are begginer coders, we also stuck with ideas that were within our skill sets (things we've done in class before that we knew we can replicate). This is also why we settled on the 2 scenes thing, boucing off the idea of the interactive storytelling class we had. Then we also took skills from the making-an-image-interactive class to get the idea to detect the door for us to enter to the next scene rather than just clicking 1 or 2. Also the particle effects for our own effects. 

🔹 2. Collaboration Phase
How did you divide responsibilities?
Responsibilities were divided up based on what each team member were going to focus on. Each member completed tasks based on skills, strengths, interest, or curiosity. Once we had an idea what the project will be about, we communicated with each other on what we each plan to create which involved a range of responsibilties. We kept in touch with each other outside of class to make sure we're all on the same page and to fix any issues we run into. With communication, everybody is able to focus on their own thing to eventually bring together.

What was the GitHub workflow like for your team? 
Some members had experience with GitHub while others didn't. Therefore, it was a learning experience. We had the main branch and some people had their own separate branch that they would work on which would eventually merge into the main branch. This allowed people to work on different parts of the project simultaneously and avoid conflicts/issues. When working on their own branch, they can commit their work, pull from main branch to be up to date, and push their own personal branch. Sometimes, when merging, you would have to resolve conflicts and you would use your judgement which version of the code to keep to be able to commit once it is resolved.


3. Coding & Development Phase
Each member of the group should briefly speak about:

Your personal contribution to the project

Your experience working collaboratively

Any specific functions, classes, or features you worked on

What aspects of the code 

worked exactly as you hoped

didn’t work at first, and how you solved or re-designed them

Renee: I created the github repository for everyone to work on and taught the groupmates that were new to this how to use github. I also created the skeleton of the project, creating the initial town scene which would lead you to the living room when you click a door. I helped find the town image and resize/edit the living room image so it would fit a horizontal display nicely. I also helped source some of the images and audio files. I created the function for the mouse to detetct what color the cursor was hovering over so that we can use that to detect where the doors on the image were so that you can click on them and have it bring you to the next scene. For the town scene I also added the twinkling star effect in the background. As for audio, I added the bg music to the town scene. I also modified the door opening sound effect to match more with the visual and the twinkle sound effect to the tree when you placed an ornament. I also just did a bunch of cleanup and small modifications to other team members code to ensure everything was polished. This was my second time working on a github repo with many people and the experience was overall pretty smooth. I was able to see changes and addition to the code that others added and was able to tinker with it. Some specific functions/classes I worked on was detectColor(), displayCurrentPage(), Class star, townText(). The code that works exactly as I'd hope was the detetcColor() function as initially I was nervous on how we would be able to change the scene, so the idea to detect the door color came up as there was 2 doors on the town scene and they were both the same color and that color only appeared on the door. In addition I was proud of the star Class which I think helps bring our image of the christmas town to life. The door actually didnt work initially so I had to go in and edit the doors so they'd be one solid color. In addition the audio didn't work at first, so then I added the feature where you need to click to get the audio started and that helped it.

Diana: I worked on the  moving clouds in the sky with two types, front clouds and back clouds just for it to have a natural look and movement of clouds. A group member assisted me with the images I wanted to use so that it doesn't look out of place and has a transparent background once uploaded. In the home screen, I worked on adding two images which was a "santa with his reindeers" image in the sky and a "reindeer on a sled" image at the floor. Both have the effect that once it was clicked, it will show a snow trail coming out of it and they move towards the direction they intend to. Santa moves towards the left and once he leaves the screen, he comes back the same way, but both inverted and moving towards the opposite direction. Once it leaves the screen on the opposite side, it will do the same thing. It will continue moving like that in a loop and whenever you click it, it will play an audio effect saying "Ho Ho Ho Merry Christmas." When the "reindeer on a sled" image leaves the screen, you will be taken to a new screen where basically it's a game that the character is going down a snow hill(with the background having snow falling to give more of that winter look) with the ability of having a jump function(spacebar). The goal is to not crash into a snowman that will randomly spawn as it comes from the right side of the screen at any coordinate. During this screen, the audio "Sleigh Ride" will be playing in a loop. Once the character crash into a snowman, user will be taken to a new screen displaying a "crash" message (includes shadow text effect)and two buttons offering the option to go home or to retry. While hovering the buttons, it will glow. To add to the winter vibe, snow falling was included. This screen will feature an audio track of "The Most Wonderful Time of the Year" which also plays in a loop. Team members made tweaks and assisted me so that the code was able to function smoothly and dislay the desired outcome. Some specific functions, classes, or features I worked on were class Cloud, class SledTrailFlake, and class SantaTrailFlake. In function draw(), I uploaded my sled and its function in the home screen which was applied for santa as well. When it was in the crash scene (gameOver), my audio was not playing correctly until I realized I had to add some code to make the audio from the screen prior fully stop. Then, the audio from the crash screen was able to play efficiently. For the visual design of the crasch screen, I played around with the fill() and text size to get the outcome. At first, I had my snow hill looking like waves, but it didn't feel realistic enough so in my function drawHill(yOffset), in the "let y =" it was changed from  sin to noise and it created the shape it is now.
