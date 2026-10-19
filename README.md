# Side Channels & Algorithmic Complexity, Visualized

SE/CprE 4210, Software Analysis and Verification, Learning Sprint 3, Problem 5.

Team 7, TEAMHacker: Mekhi San (sanm20), Ash Bhuiyan (mbhuiyan), Aaron Dais (dais0006), Luke Olsen (ltolsen)

## What this is

A small, single page, interactive teaching tool built to make two ideas from this sprint easier to understand:

1. **Timing side channels.** A simulation of the vulnerable password checker from Problem 2. Instead of only telling you right or wrong, the program leaks how many characters in your guess are wrong. You can type guesses yourself, or click "Run Automatic Attack" to watch it crack the password one character at a time in real time, the same strategy used in the actual Problem 2 exploit.

2. **Algorithmic complexity.** A slider driven chart comparing how the amount of work grows for a linear operation, a quadratic operation, and an exponential blowup as input size increases, the same shape of problem behind the ReDoS regex in Problem 3, where a small increase in input size can cause a massive increase in work. The shapes catalog bug in Problem 4 is a related but distinct failure, a shared static pointer bug that turns a list traversal into a non-terminating loop rather than one that gets exponentially more expensive, and we explain that distinction inside the app itself.

## How to run it

This is a single self contained HTML file with no build step and no external dependencies. Just open `index.html` in any modern browser.

## Files

- `index.html`, the full app (markup, styles, and JavaScript all in one file)
- `reflection.md`, our writeup for Problem 5 about building this

## Notes

No external data is collected. Everything runs client side in the browser. No API keys, secrets, or credentials are used anywhere in this project.
