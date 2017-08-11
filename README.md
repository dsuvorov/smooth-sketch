SpriteKit Smooth Sketch
===============

This project tries to minimize lag with free hand drawing SpriteKit apps by optimizing the number of nodes that are drawn on the screen from finger movement and eliminating the use of SKShapeNodes to output drawings. It uses bezier curves to calculate the movement of your sketch lines to produce very smooth streaks that follow your finger.

1. [Inspiration](#inspiration)
1. [Demo](#demo)

# Inspiration

Freehand drawing is surprisingly difficult to achieve properly on iOS SpriteKit. That's because SKShapeNode is currently plagued with memory leaking bugs, meaning your overall game performance will increasingly degrade as the user continues drawing, until their device inevitably crashes.

I came across this issue when developing my Traffic Simulation education app for iOS, which required free hand drawing. Developing this framework to achieve maximum performance and FPS in my app, I decided to open source the framework so that others can take advantage of what I spent countless hours learning through trial and error.

# Demo
[![Demo](demo.gif)](https://www.youtube.com/watch?v=qU64Cm434h8)
