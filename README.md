**Density-Based Traffic Light System**

**Purpose:**  
This project develops a traffic light system that operates based on vehicle density. Its primary goal is to give priority to the road with more vehicles, improving traffic flow efficiency.

**Materials Used:**  
- 2x CD4017 (Decade Counter)  
- 2x CD4511 (7-Segment Decoder)  
- 5x 555 Timer (TLC555)  
- 1x 74HC85 (Comparator)  
- 2x 74AC08 (AND Gate)  
- 3x 74AC32 (OR Gate)  
- 2x CD4013 (D Flip-Flop)  
- Various resistors  

**How It Works:**  
1. **Vehicle Detection:** Buttons are pressed to count vehicles on each road.  
2. **Counting Vehicles:** A 555 timer in monostable mode works with the CD4017 decade counter to register button presses, which represent vehicle counts.  
3. **Storing Counts:** The CD4017 counters maintain the counts for two roads separately.  
4. **Comparison:** The 74HC85 comparator compares the outputs from the two counters to determine the busier road.  
5. **Priority Activation:** Based on the comparison result, a 555 timer activates the green light for the road with more traffic.  
6. **Traffic Light Control:** A sequential circuit using D flip-flops, AND gates, and OR gates handles the light switching process.  

This setup ensures that the road with higher traffic density receives priority, minimizing delays and improving traffic management..
