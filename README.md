# LED Flashing Scheduling Task

This project is an implementation of a system based on STM32 that scheduling LED flashing task.

## Description

This project provides a practical example to understanding about multitasking. That involves:
1. Task timing and scheduling
   - Define and enforce temporal connstrains of tasks
   - Validate periodicity and execution times of tasks, ensuring tasks meet their specified timing requirements 
2. Task Prioritazion
   - Observing impact of assigning different prioririty to task
   - That higher priority tasks will preempt lower priority tasks, and causing delay
   - Priority can influences task execution and system behvior
3. Task Preemption
   - Task preemption affects the actual run time of lower priority tasks, causing run time to be much longer than specified
   - Due to longer runtime, leading lower priotity tasks not meet the deadline

Lower priority task missing its deadline can be fatal in hard-real time systems. So when designing, it is important to think before doing.

## Task Overflow
1. **Initialization**
   - Configure GPIO of LED
    
2. **Start Green Flashing Task**
   - Turn the Blue LED ON
   - Toggle Green LED for x seconds
   - Turn Green and Blue LED OFF
     
3. **Start Red Flashing Task**
   - Turn the Orange LED ON
   - Toggle Red LED for x seconds
   - Turn Red and Orange LED OFF


## Hardware Used
- STM32 Microcontroller
- LED
- Resistor

## Demo Video
https://github.com/user-attachments/assets/e408f3b2-f77f-4042-869b-3023f2d8d1c4

