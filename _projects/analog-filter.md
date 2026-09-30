---
layout: project
title: Analog Signal Processing Filter
course: ENSC 320
date: 2025-08-01
summary: A cascaded 4th-order Sallen-Key low-pass and 120 Hz notch filter for audio, simulated in LTspice/MATLAB and validated on the bench.
tags: [Analog Filters, LTspice, MATLAB, Oscilloscope, Circuit Build]
# image: /assets/img/projects/analog-filter/cover.jpg
---

## Overview

An anti-aliasing filter for audio signals that also removes 120 Hz power-line noise. I built it as a cascaded
4th-order Sallen-Key low-pass stage followed by a notch filter.

## What I did

- Designed and built the cascaded 4th-order Sallen-Key low-pass and notch filter.
- Simulated the frequency response in LTspice and MATLAB, reaching **40 dB attenuation at the 22 kHz Nyquist frequency**.
- Validated the physical circuit with an oscilloscope and signal generator; passband ripple stayed within the **< 2 dB** spec.
- Troubleshot and replaced components by hand to improve signal-to-noise ratio and stabilize the response.
