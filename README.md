# Phoenix-Mount-Celestron-AVX

## Introduction
A project to revive my Celestron AVX mount (the hard way..). Outside of using it for knowledge gathering, this project was all curated by hand and does not involve any AI code generation during the process.

The Phoenix Mount Celestron AVX is my first big project where I attempt to revive my old [Celestron AVX mount](https://www.celestron.com/products/advanced-vx-mount-and-tripod?srsltid=AYCX9vKO-Kc0GtgO9L3rahw95UFZhhkRPsfBb8JOQWuHxbPSsJ-XUwPr "Celestron AVX Mount and Tripod"). After many years of use, my telescope mount stopped working with a likely short somewhere on the motor control board... This project will be a fun way to (attempt to) rebuild the motor control board, along with the hand-controller unit and tracking capabilities that the old mount had. Luckily for me, the motors themselves still work, so i will largely be reusing the mechanical assembly and motors for this project!

A little about me, I am a mechanical engineer working in the automotive field. I spent around a decade working in vehicle motion and embedded controls for thermal controls and diagnostics. I have some background in controls, software, and electronics that will hopefully help me out a little along the way as i tackle this project!

As i go along through this learning adventure, i also want to share my findings with the world! I find often when i look for resources either in blogs or on youtube for some of the objectives i have below, there aren't very good/practicle examples online.. only theoretical. I want this project to give back to the community both through a blog i will keep on some of my learnings, as well as via video series i will eventually make to document some of the cool parts in my journey. You can find the links below to these media:

- [Youtube](https://www.youtube.com/playlist?list=PLSRuyE-O5PDQ "Phoenix Mount Youtube Playlist")
- [Github Blog](https://a-dot-n.github.io/ "A-DoT-N Github Pages")
- [Phoenix-Mount-Celestron-AVX Repo](https://github.com/A-DoT-N/Phoenix-Mount-Celestron-AVX "Phoenix Mount Repo")

## Learning Objectives
1. C++ Programming
    - I have largely only worked with C in my career with a short stint in the chip industry working in C++ and Python. I want to leverage some of those learnings and enhance them as i go through this project.
    - I could use FreeRTOS or Zephyr for this project which im sure would speed things up a lot for me, but instead i want to go back to first principles and understand how tools like these work. I will be attempting to bare-metal code this project as my primary objective.
2. Microcontroller Architecture
    - As a mechy, CPUs are really cool. But also kind of magic... This objective focuses on really hardening my understanding on how microcontroller architectures work.
    - I will be working with the ESP32C6 which is a RISC-V architecture. I hope to learn a little about how RISC-V works as well as how to turn technical reference guides into hardedned requirements i can implement.
3. Electronics and PCB design
    - This is the area I have the least experience with... To say the least, i've seen the forbidden smoke (and lightning bolts at times) escape my electronics...
    - I want to build up some fundamental knowledge on how electronics work at the electrical level, and use this knowledge to eventually build my own custom PCB that will act as my motor controller and UI to the mount.
4. Control Theory
    - The cool thing about this project is that it is a practical entry-point into controls engineering. I have some background in controls from my job and schooling, but i've never applied it across a full stack that i built.
    - I will be designing a multi-axis control system that will track the night-sky to at least somewhere in the ballpark of what the original mount was capable of... I know i have succeeded if i can capture a photo for ~4 seconds without stars trailing in the shot.
5. UI design
    - The original celestron UI design from years back used a handheld unit to interact with the mount. At a minium i want to re-create this along with perhaps some improvements for the user to interact with the mount.