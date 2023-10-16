# Computer-Benchmark
Analyzing the performance of my custom built PC using a variety of gaming and synthetic benchmarks. 

## Compiling Data

I measured several variables as I tested my computer (such as but not limited to GPU/CPU temperature, power draw, utilization, and clock speed) to see if my PC was performing as I'd expect for the components I bought. In addition, getting a baseline performance analysis of my computer will help me in the future if something starts to act up on my computer. For example, I'll have a good idea when my the thermal compound on my CPU cooler needs to be replaced once the CPU starts going significantly above the baseline temperature I measured while all the components were new.

The two programs I used to measure these variables were Nvidia's Frameview and HWiNFO64 which saved the data as CSV's that I could then import into R. 

In the case of frameview, the program created a new CSV file for every game tested with the name of the game being included in the CSV's file name. So, instead of manually compiling each of the separate game files together I built a python program called “Organize Excel” to automatically sort through all the CSV files in the frame view folder and combine them together as individual sheets within a single excel file for easy analysis in R. 
 
I compiled all the data I collected into line and bar graphs using ggplot2 in R. 

## Gaming Benchmarks

My current test suit of games includes: GTAV, Overwatch, Rainbow Six Siege, Apex Legends, Destiny 2, Rocket League, Battlefront 2, Halo Infinite, Fortnite, and Call of Duty: Warzone. For each game I examined the following variables as I ran my benchmark:  Frametime, GPU and CPU temperature, GPU and CPU utilization, GPU and CPU clock speed, GPU and CPU power consumption, Fan speed for CPU & GPU coolers, fan speed for the case fans, and Average FPS, 1% low FPS, and .1% low FPS. Analysis and graphs made for the gaming test suite was this was done in the “neat_game” program. 

For all the variables above except Average FPS, 1% low FPS, and .1% low FPS each game was tested one time. For the Average FPS, 1% low FPS, and .1% low FPS I tested each game three times and then averaged the results together to get a more accurate measure of real world FPS while playing games.  

## Synthetic Benchmarks 

The synthetic benchmarks I tested with are 3D Mark's Timespy and Fire Strike Extreme, Heaven, and Cinebench R23. I tested the same variables with the synthetic benchmarks as I did with games except I did not measure frametime or any FPS measure. Analysis and  graphs made for synthetic benchmarks test suite was this was done in the “neat_synthetic” program.     

## Sorting Graphs by Name 

Once all the graphs from the "neat_game" and "neat_synthetic" programs were made and automatically saved into their specific "unsorted" folders, I used built a python program called "Graph File Organization" to sort each graph into relevant folders designated by the specific game/synthetic benchmark name.  

## More Information 

For more information on the configuration and specifications of my computer please see the document titled "Computer info -July 1 Tests.docx".  

"Problems are opportunities in disguise." - Charles F. Kettering
