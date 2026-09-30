---
layout: project
title: Matrix Arcade
course: ENSC 351
date: 2025-12-01
summary: A real-time multiplayer game console on a BeagleY-AI, driving a 64×32 RGB LED matrix, with an Android app as the controller.
tags: [C++, Embedded Linux, BeagleY-AI, UDP, Android, Multithreading]
# image: /assets/img/projects/matrix-arcade/cover.jpg
---

## Overview

Matrix Arcade is an embedded multiplayer game console. Games render on a 64×32 RGB LED matrix and an LCD,
and players control them from their phones through a custom Android app.

## What I did

- Wrote a C++ hardware abstraction layer (HAL) on the BeagleY-AI to drive the 64×32 RGB LED matrix and the LCD.
- Built an Android app that sends joystick and accelerometer input to the console over UDP with low latency.
- Designed a framebuffer for drawing shapes and text, and optimized updates to reduce flicker.
- Wrote multi-threaded packet handling and a UDP bridge so the games stay responsive in real time.
