# Lightweight cooperative multitasking.

main.c is at Core/Src/main.c.

## Setup
1. Use the built-in cubeMx to generate code.

## Non-blocking wait

1. See flashLEDTask. It appears CNT
 needs re-initializing otherwise the double
 flash does not occur.
 This is due to a race-condition as the timer
 overflows and the task yields to main.

1. This implies other tasks cannot share the
 timer.

1. Work OK at millisecond, but is racy at
 microsecond resolution.
