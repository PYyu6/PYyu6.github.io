---
layout: post
title:  I Design a Interactive Music Visualization
date:   2020-10-19 15:01:35 +0300
image: musvis.png
tags:   Sense Tech Art
---

This web app is buiilt with __react hooks__, __HTML Canvas__ and 
__Firebase__
You can check out the <a href="https://vinyl-record-maker.web.app/"> live Demo</a>.

***

## How to play
1. Be sure to use the full screen. Refresh if you haven't :)
2. Click one of the top-left buttons, then get the piano octave.
Press keys from the list **a,w,s,e,d,f, t,g,y,h,u,j** on the keyboard, which corresponds to notes from a chromatic scale
3. Then, as you play along, you will hear the best fit chords will sound. And for each note in the chord, you can see a white circle jumping around the corresponding area on the record.

***

## Why I built
In university, Psychology is my minor. During the first psychology course, a <a href="https://en.wikipedia.org/wiki/Synesthesia">Synesthesia</a> patient is invited as a guest speaker. He said he could hear the violet colour and tastes the shape.  I still remember when my classmates asked him what "love" and "lies" tastes like, everyone raised their heads and silently waited for his answer. Yeah, it is magical.

I start to ponder what normal people's experience would change when their senses intertwine. Will they feel more connected to things around them since they can perceive the world with an additional dimension?
As a result, I am inspired to make such a music visualization app so that people can (bold) see music like <a href="https://en.wikipedia.org/wiki/Chromesthesia#:~:text=Chromesthesia%20or%20sound%2Dto%2Dcolor,associations%2Fperceptions%20in%20daily%20life...">Chromesthesia</a>

***
## Concept Design

To better mimic the sense translation, I need to carefully think about how to display the music note. 
Firstly, how to let users know which note they just played and how many times they have played them. After a few attempt, I decided to use the idea of the vinyl record as the background. Each octave is a ring shape and each note is equally distributed there. When users type keys to play notes, the sections on the record corresponding to those keys get colours, which makes users they are creating a melody on the traces on the record. 
Also, I need to choose how to decide how to select the colour to make each octave connected with as well as distinguishable from others. For example I have tested a few plans for the colour choice.

1. same key(such as key D#) in all octaves get the same colour but different opacity
2. all keys in each octave share the same colour

Besides, I tried to use a few ways to represent the chord. In the first version, for every note in the chord, a ring changes its shape like a progress bar moving there. Since it looks a little messier. Then I use animated circles jumping around the corresponding area to each note in the chord


*** 

## Programming journey


Last but not least, I would love to talk about I have learned in the programming perspective. You can check the <a href="https://github.com/PYyu6/create-vinyl-record">code</a>

* Learn how to use canvas to draw and make animation on the web. It is quite different from styling and functioning as the normal CSS component.
* Learn how to use react hook, which is a much cleaner way than react-native to structure codes.
* Get deep understanding of javascript components such as array and promises since I need to design how the data would be stored. Also, it need to provide output based on users' input that might quickly change.
I would like to talk about the libraries I have used and thoughts in future posts. Stay tuned!

***

I have just accomplished stage 1 and I plan that different users can interact with others in the future. Please stay tuned. If you have any thoughts, feel free to discuss with me.

