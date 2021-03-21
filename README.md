# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Sumi Kolli**

Time spent: **3.5** hours spent in total

Link to project: [Project Page](https://glitch.com/edit/#!/memory-match-codepath)

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [X] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [X] Font change
- [X] Background Color Change
- [X] Text Color Change
- [X] Alert Change
- [X] Button Background and Text Color Change

## Video Walkthrough

Here's a walkthrough of implemented user stories:
[GIF](http://g.recordit.co/Ie1HdcuTRD.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

https://fonts.google.com/

https://www.w3schools.com/

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

A challenge I had when creating this submission was thinking through the logic of how HTML elements appeared on the page, and how adding or removing elements would affect the layout of the rest of the page. An example of this happened when I was working on adding images to the game buttons as one of the optional features. I was confused about where to put the img tags in the HTML code, so as to have them appear only when the button was pushed. It was hard to visualize this, especially since the images could not be visible until the button was pushed. I was able to think through the solution by looking back at how the div tag works in HTML. Considering that the div tag wraps around all of the elements inside it, I realized that I needed to have the button element wrap around the image, so that the image would not take up extra space on the page when made visible. Then, I had to consider what property to use to make the image hidden. I initially used the display: none property, but soon realized that because this property makes the selected element not take up any space on the page, clicking on the button made the image suddenly appear and take up space. This changed the alignment of all the other buttons and made the appearance messier. I decided that I needed to use a property that only hid the elements but kept their allocated space on the page, which is why I settled for the visibility: hidden property instead. Another challenge I faced was when I was implementing the logic for the optional feature to give the user 3 strikes before the game ends. I was not sure where to increment variables, like gameFeatures, and progress and when to call the playClueSequence() in relation to changing the game logic. In this instance, I went back and looked at the provided flow chart of the game logic, and I added in the additional pathway of having strikes. Expanding on the visualization allowed me to pinpoint what I needed to change in my logic.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

A question I have about web development after I completed the project is how to use Javascript to create more complex user interactions. In the game, we mainly used the onclick function to change properties of the elements, such as clicking the game buttons to darken the color, make the image visible, and create a tone, but I want to learn more about how else onclick and other functions can be used to make a webpage more interactive, rather than static. I want to explore how scrolling up or down a webpage can impact the layout or view of elements, how hovering over elements can change their appearance, and how a user can interact with a web page with more than clicking. Another question I have is how the alert function works to bring up a dialog box on the browser. I understand that this is built-in with Javascript, but I want to learn more about how Javascript interacts with the browser’s API to create this event. I would also like to explore other ways in which Javascript can alter the browser environment to make a web page more functional. Overall, I hope to gain a more in-depth understanding of making more interactive web pages and adding more utilities to them.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours to work on this project, I would mainly like to add more features and functionality to the game, which would mean integrating backend elements to the web page as well. The first change I would make is to let the game continue infinitely, and only end when the user makes a mistake, or 3 mistakes. This would mean that instead of winning the game, the user would have a score that would correspond to their memory response. Along with this change to the game logic, I would like to add a feature that lets users type in a username or password, so they can save their scores and see their statistics when they return to the game later. Adding this feature would require the development of modal pop-ups or more pages. Databases would also be involved to save user information, which comes under backend development. Additionally, I would like to add an option that lets users see how their score compares to other user’s scores. This could be done through a leaderboard of user scores. This feature would again require the use of databases to track multiple users and their scores, as well as have sorting and live updating functions for the rankings. The leaderboard feature would also constitute the development of another page on the site. With all of these features, there needs to be more backend development and making the web page into a multipage website.



## License

    Copyright [Sumi Kolli]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
