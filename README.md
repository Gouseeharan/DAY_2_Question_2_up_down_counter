Question — Programmable Up/Down Counter

Design a 4-bit programmable up/down counter.

Inputs :
clk
reset
enable
up_down
limit[3:0]


Output :
count[3:0]


Expected behavior :

reset = 1 → count = 0 on the next rising edge.
enable = 0 → hold current count.
enable = 1 and up_down = 1 → count up.
When counting up and count == limit:
limit → 0
enable = 1 and up_down = 0 → count down.
When counting down and count == 0:

0 → limit
The counter must never go above limit or below 0.
Reset has priority over counting.
