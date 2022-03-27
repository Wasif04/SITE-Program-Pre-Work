# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Wasif Khan**

Time spent: **4** hours spent in total

Link to project: https://glitch.com/edit/#!/pond-woolen-thunder?path=index.html%3A17%3A41

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

1.) Game is functional and shows message that you have won after completing all turns. This also shows the patterns getting progressively faster.
http://g.recordit.co/fYlPQ5BmVE.gif

2.) Game shows "you lose" message when you click on the wrong button and stops the game.
http://g.recordit.co/XbEY0f6vb9.gif

3.) Game starts with a new pattern every time you start a new game.
http://g.recordit.co/5NzFVYUVVy.gif

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

W3 Schools, Stack Overflow, mdn web docs, freshman.tech.com

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

While I was doing the speed it up challenge, I was having a hard time trying to figure out how to update playSequenceClue. I set the variable to 200 and the clueLength to 5. I kept doing  delay += clueHoldTime - 40 to test how fast it would go and nothing changed. I then did delay += cluePauseTime - 40 and saw a difference, however, the difference was just a one time change and did not change each round. I looked up ways to speed up a game and found a site that had a similar project with a simon says game. I was looking through it and found out that I just had to return the variable and add 1. So I got rid of any changes I made and in the beginning of the function I put clueHoldTime = clueHoldTime - 50 to see if there was any drastic change that I would see. After doing this, I saw that each round got significantly quicker. To now make this game be within a reasonable time, I did 200 divided by 5 to get 40 for the number of milliseconds I needed to subtract. After changing the 50 to 40, I noticed that each round got quicker however, the last round was too fast and I was not able to see any of the colors that were pressed. I then changed the number to 35 and thought this was a perfect number to use as it would still make the final round doable.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

After completing this project. I was wondering what other tags there are for html and how it would further improve this game for the pre-work. From doing this project, I realized that the backend part seems more easy for me since it is similar to what I did in previous CS classes. However, the frontend part was very confusing for me since I never did any type of frontend before. I would like to learn more about frontend coding and become more experienced in it. I also wondered if it was possible to make certain functions run faster through different variations in writing the code to make certain parts more smooth and fast.


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)

I would have liked to add some additional designs to make this web app feel less generic. I would have liked to make it a certain theme and make every button design be in that theme. This would have made the web app more appealing. In addition, I wanted to add an area where the user gets to make their own settings for the game such as number of rounds preferred, amount of time per round, and a hint button to replay to clues one more time with some type of penalty such as a time penalty or an extra round added on. 




## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright [Wasif Khan]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
