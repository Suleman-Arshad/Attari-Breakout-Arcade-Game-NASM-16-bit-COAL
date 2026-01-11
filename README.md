🎮 Atari Breakout Game – 16-bit NASM

A classic Atari Breakout–style arcade game developed entirely in 16-bit x86 assembly language (NASM) as part of the Semester 3 Computer Organization & Assembly Language (COAL) course.

📌 Project Overview

This project recreates the famous Breakout game using low-level system programming concepts. The game runs in DOS text mode (80×25) and directly interacts with hardware for graphics, keyboard input, and sound. It is implemented as a .COM program with origin 0x0100.

🛠️ Technologies Used

Language: NASM (16-bit x86 Assembly)

Execution Environment: DOS / DOSBox

Graphics: Direct video memory access (0xB800:0000)

Keyboard Input: BIOS Interrupt INT 16h

Sound: PC Speaker + Programmable Interval Timer (PIT)

Program Type: .COM executable

🎮 Gameplay & Controls

Controls

⬅️ Left Arrow → Move paddle left

➡️ Right Arrow → Move paddle right

␣ Space → Launch ball

⎋ ESC → Exit game

Rules

Break all bricks to win 🧱

Start with 3 lives ❤️

Each brick gives 10 points

Losing all lives ends the game

✨ Features

Smooth non-blocking keyboard input

Ball & paddle collision detection

Brick collision and destruction logic

Score and lives display

Retro sound effects:

Paddle hit

Brick break

Life lost

Win and Game Over screens

🔊 Sound System

Sound effects are generated using the PC Speaker by programming the PIT (Ports 0x43, 0x42, 0x61), creating an authentic retro arcade experience.

▶️ Build & Run Instructions

Assemble the program using NASM:

nasm breakout.asm -f bin -o breakout.com


Run the game in DOSBox or a real DOS environment:

breakout.com


⚠️ Make sure DOSBox allows speaker and port I/O access for sound.

📚 Learning Outcomes

This project helped us understand:

Assembly-level programming

Memory addressing & registers

BIOS & DOS interrupts

Hardware-level graphics and sound

Real-time game loops and collision logic

👥 Contributors

Muhammad Suleman

Abdur Rehman

🎓 Course: Computer Organization & Assembly Language (COAL)
📘 Semester: 3
🏫 Program: BS Computer Science
