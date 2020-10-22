---
layout: post
title:  I Design an Interactive Music Visualization
date:   2020-10-19 15:01:35 +0300
image: musvis.png
tags:   Sense Tech Art 
---

This web app is buiilt with __react hooks__, __HTML Canvas__ and 
__Firebase__
You can check out the <a href="https://vinyl-record-maker.web.app/"> live Demo</a>.

***

## How to play
1. Be sure to use Chrome and make the browser window full screen. Refresh if you haven't :)
2. Click one of the top-left buttons to choose the piano octave.
3. Press lowercase keys from the list **a,w,s,e,d,f, t,g,y,h,u,j** on the keyboard, which corresponds to different musical notes.

Then, you will find your melody changes the record. As you play along, you will hear the best fitting chords. Also, for each musical note in the chord, you can see a white circle jumping around the corresponding area on the black record.

***

## Why I built
At the University of Toronto, I have chosen Psychology as my minor. During the first psychology course, a <a href="https://en.wikipedia.org/wiki/Synesthesia">Synesthesia</a> patient was invited as a guest speaker. He said he could hear the violet colour and taste the shape.  I still remember when my classmates asked him what "love" and "lies" tasted like, everyone in the room raised their heads and silently waited for his answer. Yeah, it was magical.

Then, I started to ponder what normal people's experience would change when their senses intertwine. Would they feel more connected to things around them since they could perceive the world with an additional dimension?
As a result, I was inspired to make this interactive music visualization app so that people can see music like <a href="https://en.wikipedia.org/wiki/Chromesthesia#:~:text=Chromesthesia%20or%20sound%2Dto%2Dcolor,associations%2Fperceptions%20in%20daily%20life...">Chromesthesia</a>

***
## Concept Design

To better mimic the sense translation, I need to think carefully about how to display the music note. 
Firstly, I tried to figure out how to let users know which notes they just played and how many times they played those notes. After several attempts, I decided to use the idea of the vinyl record as the background, and let users write melodies on it. Specifically, there are five octaves users can choose from. Each octave has a ring shape and each note in an octave has an equal section. When users type keys on the keyboard to play notes, the area on the record corresponding to those notes change colours. The more they play the musical notes, the opacities of the colour in those areas increase. Thus this will give users a cool visualization of what melodies they have just written. 
Secondly, I hope each octave can be connected with but can be distinguished from others at the same time, so it is important to choose colours to represent musical notes on the record. For example, I have tested a few plans for the colour display.

1. same key(such as music key D#) in all octaves get the same colour but different opacity
2. all music keys in each octave share the same colour

Besides, I tried to use a few ways to represent the chords that best fit users' melodies. In the first version, for every music note in the chord, the corresponding area on the record animates like a circular progress bar. Since it looks a little messier, then I use animated white circles jumping around the corresponding area on the black record disc for each musical note in the chord.


*** 

## Programming journey


Last but not least, I would love to talk about what I have learned from the programming perspective. You can check the <a href="https://github.com/PYyu6/create-vinyl-record">code</a>

* Learn how to use canvas to draw and make animation on the web. Styling and functioning canvas is quite different from the normal CSS component. I need to set canvas's width and height dynamically to display clear strokes on the browser.
* Learn how to use react hook, which is a much cleaner way than react-native to structure codes.
* Get a deep understanding of javascript components such as array and Promise. Since users' input might quickly change and I need to design  the data storage, I need to carefully and efficiently handle Promise and change of state in this interactive web app
I would like to talk about the libraries and techniques that I have used in future posts. Stay tuned!

***

I have just accomplished stage 1. In the future, I hope different users can interact with others in the future. Please stay tuned. If you have any thoughts, feel free to discuss with me.

---
layout: post
title:  I Design an Interactive Music Visualization
date:   2020-10-19 15:01:35 +0300
image: musvis.png
tags:   Sense Tech Art
---

This web app is buiilt with __react hooks__, __HTML Canvas__ and 
__Firebase__
You can check out the <a href="https://vinyl-record-maker.web.app/"> live Demo</a>.

***

## How to play
1. Be sure to use Chrome and make the browser window full screen. Refresh if you haven't :)
2. Click one of the top-left buttons to choose the piano octave.
3. Press lowercase keys from the list **a,w,s,e,d,f, t,g,y,h,u,j** on the keyboard, which corresponds to different musical notes.

Then, you will find your melody changes the record. As you play along, you will hear the best fitting chords. Also, for each musical note in the chord, you can see a white circle jumping around the corresponding area on the black record.

***

## Why I built
At the University of Toronto, I have chosen Psychology as my minor. During the first psychology course, a <a href="https://en.wikipedia.org/wiki/Synesthesia">Synesthesia</a> patient was invited as a guest speaker. He said he could hear the violet colour and taste the shape.  I still remember when my classmates asked him what "love" and "lies" tasted like, everyone in the room raised their heads and silently waited for his answer. Yeah, it was magical.

Then, I started to ponder what normal people's experience would change when their senses intertwine. Would they feel more connected to things around them since they could perceive the world with an additional dimension?
As a result, I was inspired to make this interactive music visualization app so that people can see music like <a href="https://en.wikipedia.org/wiki/Chromesthesia#:~:text=Chromesthesia%20or%20sound%2Dto%2Dcolor,associations%2Fperceptions%20in%20daily%20life...">Chromesthesia</a>

***
## Concept Design

To better mimic the sense translation, I need to think carefully about how to display the music note. 
Firstly, I tried to figure out how to let users know which notes they just played and how many times they played those notes. After several attempts, I decided to use the idea of the vinyl record as the background, and let users write melodies on it. Specifically, there are five octaves users can choose from. Each octave has a ring shape and each note in an octave has an equal section. When users type keys on the keyboard to play notes, the area on the record corresponding to those notes change colours. The more they play the musical notes, the opacities of the colour in those areas increase. Thus this will give users a cool visualization of what melodies they have just written. 
Secondly, I hope each octave can be connected with but can be distinguished from others at the same time, so it is important to choose colours to represent musical notes on the record. For example, I have tested a few plans for the colour display.

1. same key(such as music key D#) in all octaves get the same colour but different opacity
2. all music keys in each octave share the same colour

Besides, I tried to use a few ways to represent the chords that best fit users' melodies. In the first version, for every music note in the chord, the corresponding area on the record animates like a circular progress bar. Since it looks a little messier, then I use animated white circles jumping around the corresponding area on the black record disc for each musical note in the chord.


*** 

## Programming journey


Last but not least, I would love to talk about what I have learned from the programming perspective. You can check the <a href="https://github.com/PYyu6/create-vinyl-record">code</a>

* Learn how to use canvas to draw and make animation on the web. Styling and functioning canvas is quite different from the normal CSS component. I need to set canvas's width and height dynamically to display clear strokes on the browser.
* Learn how to use react hook, which is a much cleaner way than react-native to structure codes.
* Get a deep understanding of javascript components such as array and Promise. Since users' input might quickly change and I need to design  the data storage, I need to carefully and efficiently handle Promise and change of state in this interactive web app
I would like to talk about the libraries and techniques that I have used in future posts. Stay tuned!

***

I have just accomplished stage 1. In the future, I hope different users can interact with others. Please stay tuned. If you have any thoughts, feel free to discuss with me.

