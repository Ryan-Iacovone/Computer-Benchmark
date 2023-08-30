# Computer-Benchmark
Analyzing the performance of my custom built PC using a variety of gaming and synthetic benchmarks. 

I measured several varaibles as I tested my computer (such as but not limited to GPU/CPU temperature, power draw, utilization, and clock speed) to see if my PC was performaing as I'd expect for the componenets I bought. In addition, getting a baseline performance analysis of my computer will help me in the future if something starts to act up on my computer. For example, I'll have a good idea when my the thermal compound on my CPU cooler needs to be replaced once the CPU starts going significantly above the baseline temperature I measured while all the componenets were new.

The two programs I used to measure these variables were Nvidia's Frameview and HWiNFO64 which saved the data as CSV's that I could then import into R. 
 
I compiled all the data I collected into line and bar graphs using ggplot2 in R. 

My current test suit of games includes: GTAV, Overwatch, Rainbow Six Seige, Apex Legends, Destiny 2, Rocket League, Battlefront 2, Halo Infinite, Fortnite, and Call of Duty: Warzone. For each game I tested the following variables as I ran my benchmark:  Frametime, GPU and CPU temperature, GPU and CPU utilization, GPU and CPU clock speed, GPU and CPU power consumption, Fan speed for CPU & GPU coolers, fan speed for the case fans, and Averge FPS, 1% low FPS, and .1% low FPS. 

The synthetic benchmarks I tested with are 3D Mark's Timespy and Fire Strike Extreme, Heaven, and Cinebench R23. I tested the same varaibles with the synthetic benchmarks as I did with games excpect I did not measure frametime or any FPS measure. 

For more on my testing methodologies please see the document titled "Computer info -July 1 Tests.docx".  

Once I made all the graphs, I used a python program to sort them into their relavent folders by game/synthetic benchmark name.  