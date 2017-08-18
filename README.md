# 7-Segment
Arduino library to print numbers on a 7 segment display

Required: Arduino, 2-digit 7-segment display, SIPO shift register

Example:
```c++
#include <_7SEG.h>
 
#define S1_PIN 4
#define S2_PIN 3
#define SR_CLK 13
#define ST_CLK 12
#define D_PIN 2
 
_7SEG disp(S1_PIN,S2_PIN,SR_CLK,ST_CLK,D_PIN);
void setup() {
 
}
void loop() {
  for(double i=0;i<99;i=i+0.1)
    disp.print(i);
}
```

Schematic: 
<p align="center">
  <img src="https://hobbytronicsblog.files.wordpress.com/2017/08/schematic2.png?w=609&h=527" width="609"/>
</p>
