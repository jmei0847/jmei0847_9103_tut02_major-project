# jmei0847_9103_tut02_major-project

## 1. Instructions on how to interact with the work
- Click the "Original/Refresh" button at the top to refresh the canvas directly or reset the current canvas
Click 
- Click the "Random Draw" button to randomly generate different patterns on the canvas
- Click the "Rotate & Random draw" button to rotate the canvas and randomly generate  patterns
- Click the "Clear" button to clear the current canvas

## 2. Details of your individual approach to animating the group code.
### 2.1 Which method do you choose to drive your individual code?
User Input:Incorporate mouse or keyboard inputs for animation.

### 2.2 Which properties of the image will be animated and how?
I add a randomCircles() function to make the canvas to reveal only a few drawing patterns at a time. Also, I add a rotateCircles() function to make the canvas rotated and at the same time can also generate random patterns.
The canvas is refreshed each time the corresponding button is pressed, and random generaiton works. Also, random generation also works when the canvas is rotated.

### 2.3 References to inspiration
My design's inspiration comes from the kaleidoscope and collage builder. 
When the rotate the kaleidoscope, each rotation brings a different visual picture. When the canvas rotates, it revolves around a rotating central point, constantly generating various shapes, and as the canvas rotates, each shape gradually changes color or appears or disappears, producing a dreamlike visual effect.
When random draw the patterns on canva, it is like the random appearance of various graphics on a fixed canvas, different colors, random combinations, so that each frame has a new sense of abstract art.

![picture](READMEImage/kaleidoscope%20inspiration.jpeg)
![picture](READMEImage/kaleidoscope%20inspiration%202.jpeg)
![picture](READMEImage/collage%20builder%20inspiration.jpeg)

  [Reference of picture 1](https://www.google.com/imgres?q=%E4%B8%87%E8%8A%B1%E7%AD%92&imgurl=https%3A%2F%2Fimage.uisdc.com%2Fwp-content%2Fuploads%2Fcovers%2F201604%2Fai-design-kaleidoscope-effect-b.jpg&imgrefurl=https%3A%2F%2Fwww.uisdc.com%2Fai-design-kaleidoscope-effect&docid=Z7V1h715u6gV4M&tbnid=z4vics_LKk7JfM&vet=12ahUKEwi-uYLCwtSJAxXkyjgGHWtiFVAQM3oECGMQAA..i&w=440&h=280&hcb=2&ved=2ahUKEwi-uYLCwtSJAxXkyjgGHWtiFVAQM3oECGMQAA)
[Reference of picture 2](https://www.google.com/imgres?q=%E4%B8%87%E8%8A%B1%E7%AD%92&imgurl=https%3A%2F%2Fwww.shutterstock.com%2Fimage-vector%2Fgeometric-design-mosaic-vector-kaleidoscope-260nw-1110979655.jpg&imgrefurl=https%3A%2F%2Fwww.shutterstock.com%2Fzh%2Fimage-vector%2Fgeometric-design-mosaic-vector-kaleidoscope-abstract-1110979655&docid=1tURNfBB2xztvM&tbnid=DuLLRdFvDFIZmM&vet=12ahUKEwi-uYLCwtSJAxXkyjgGHWtiFVAQM3oECDgQAA..i&w=462&h=280&hcb=2&ved=2ahUKEwi-uYLCwtSJAxXkyjgGHWtiFVAQM3oECDgQAA)
[Reference of picture 3](https://www.google.com/imgres?q=collage%20builder&imgurl=https%3A%2F%2Fpixlr.com%2Fimages%2Fcollage%2Fendless.webp&imgrefurl=https%3A%2F%2Fpixlr.com%2Fphoto-collage%2F&docid=2LfZ4OHlCV_o7M&tbnid=7mFtBiwyTmbgMM&vet=12ahUKEwjf4PbZwtSJAxWDxDgGHT6fFD4QM3oECCgQAA..i&w=1024&h=1024&hcb=2&ved=2ahUKEwjf4PbZwtSJAxWDxDgGHT6fFD4QM3oECCgQAA)

### 2.4 Short technical explanation
In the functions which acts on the buttons, I referred to The Coding Train's tutorial that talking about how to save the current transformation, then restore that transformaiton. In the function rotateCircles(), randomCircles(), and reset(), I use push() and pop() function to save their individual transformation to make each button can be separated from the function of other buttons.

- Therefore, the button "Original/Refresh" is used to only change the canva back to the original drawing or just refresh the page. I add random color changes to some of the patterns‘s function, which makes the image slightly different every time you click the button.
- The button "Random Draw" is used to randomly generate these patterns without changing the initial position of each pattern.
- The button “Random Draw" is used to make the entire canvas pattern to rotate, and each click will rotate the canvas and randomly generates these patterns.
- The button "Clear" can clear all the transformaiton at any time. And this time, when you click the "Original/Refresh" button again, the canva will back to the original state.

 [Link to The Coding Train: How to Rotate Shapes in p5.js (translate, rotate, push, pop)](https://www.youtube.com/watch?v=o9sgjuh-CBM&ab_channel=TheCodingTrain)


### 2.5 Changes to the group code
Based on the group code, I changed the color settings in these funcitons: ConcentricCircle, ComplexCircleWithDotsAndShapes,RadiantCircleWithRays. The colors in these three graphs now change randomly each time when you refresh the canvas. This makes the image look less stiff and more randomly generated.
