# Operating Systems Seminar Prompts

<p align="center">
Department of Engineering, Cal Poly Pomona
</p>

## Table of Contents
- [Overview](#overview)
- [Seminar 1: Shell Application](#seminar-1-shell-application)
- [Seminar 2: Scheduler in C](#seminar-2-scheduler-in-c)
- [Seminar 3: Memory Virtualization Slides](#seminar-3-memory-virtualization-slides)
- [Seminar 4: Producer-Consumer Threads & Driver](#seminar-4-producer-consumer-threads--driver)
- [Seminar 5: User Space Sample Application](#seminar-5-user-space-sample-application)
- [Appendix](#appendix)
- [Acknowledgement](#acknowledgement)

---

## Overview

This repository contains all prompt details for the Operating Systems Seminar course at Cal Poly Pomona. Each seminar addresses a major topic in operating systems through hands-on programming, scheduling, concurrency, and kernel interaction projects.

---

## Seminar 1: Shell Application

Create a shell application that can run simple commands from `/usr/bin` and at least 2 custom commands:

- **exit**: Terminates your application.
- **close**: Terminates your application (same as exit, but must be implemented separately).
- **help**: Displays details about your application.

Your shell must support running any command from `/usr/bin` and handle the above custom commands.

---

## Seminar 2: Scheduler in C

Create a scheduler in C. Choose one of the following options:

- **Option 1:** Multilevel Feedback Queue (**MLFQ**) Scheduler
- **Option 2:** **Lottery** Scheduler

Implement the scheduler logic and be prepared to discuss your design.

---

## Seminar 3: Memory Virtualization Slides

Create your own slides (PowerPoint) for the current unit: **memory virtualization**.

- Slides must be submitted by **Tuesday 04/08/2025 @ 5PM.**
- **Optional:** If you use Overleaf to create these slides, extra seminar questions are waived. In this case, submit both the source files and the exported PDF.

---

## Seminar 4: Producer-Consumer Threads & Driver

Create a loop in `main()` that generates multiple consumer threads and multiple producer threads.

Requirements:

- **Condition Variables:**  
  - One for stock empty
  - One for stock full (100 units)
- **Consumers:**  
  - Can purchase between 1 and 5 units (randomized)
  - If insufficient units, consumer waits for supply
- **Producers:**  
  - Can deliver up to 20 units (randomized)
  - If insufficient space, producer waits for space
- **Status Updates:**  
  - Print messages showing who is waiting, current stock level
- **Thread Timing:**  
  - Consumers and producers show up every TBD seconds (each is a new thread)
- **Driver:**  
  - Include `unlocked_ioctl` functionality (add file operation besides `read` and `write` as shown in slides)
  - Demonstrate communication with user space application (minimum: `read`, `write`, `ioctl`)

---

## Seminar 5: User Space Sample Application

For 8/10 credit: Present the second example from the slides (the one with `read` and `write`) on your Linux machine.  
- Must include the user space sample.


