# Lightweight cooperative multitasking.

main.c is at Core/Src/main.c.

## Setup
1. Use the built-in cubeMx to generate code.

## Non-blocking wait
1. See flashLEDTask. It appears CNT
 needs re-initializing otherwise the double
 flash does not occur.
