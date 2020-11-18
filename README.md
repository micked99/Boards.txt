# Boards.txt
Drop this file in Arduiono IDE, it will ad the possibility to run the board at any speed of the following: 1, 2, 4, 8 & 16Mhz 

Set the prescaler, in this setup the XO is dived with 4, so if you run a 8Mhz xo the board will run at 2Mhz
  //clock_prescale_set(clock_div_2);
  clock_prescale_set(clock_div_4);
  //clock_prescale_set(clock_div_8);
  
edit this line: #define WSPR_CTC  1334   // CTC value for WSPR - 10672 @ 16Mhz //5336 @ 8Mhz //2668 @ 4Mhz //1334 @ 2Mhz //667 @ 1Mhz
and last shoose the correct Speed under Tools - Boards in IDE which should be 2Mhz
