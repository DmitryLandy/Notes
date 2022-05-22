# V&V Final
## Scenario
-   Robot Following a line.
-   3 sensors 
-   2 black lines 
-   Task: Follow between the lines 
-   Sensors "see" via voltage. 4 options: 
    -   OnLine: <80 
    -   SpaceInsight: 81 - 120  
    -   LineInsight: 121 - 190 
    -   InSpace: > 191

![](Pasted%20image%2020220423120112.png)
Given three sensors the design is the following: 
1) Determine the state of each sensor (online, spacelnsight, linelnsight, inSpace) 
2) If middle sensor sees the line just go forward 
3) If middle sensor does not see the line then use a combination of logic to determine subtle moves (veer 
left or right) or make hard turns (hard left or right) based on what the left and right sensors are seeing

## Defect Table
![[Pasted image 20220423120609.png]]![[Pasted image 20220423120639.png]]

## Question 1
![[Pasted image 20220423121231.png]]
### Q1 Answer
The rover's purpose is to follow a path between two black lines so that this system could be applied to vehicles to provide an autonomous steering feature. Operational scenarios to test this should be those that could be encountered on the road such as those in residential areas, city, and highways.

**Standard Straight Lane:**
![[Pasted image 20220423123426.png]]
This a standard straight lane where the rover should stay between the lines.

**Standard Curved Lane:**
![[Pasted image 20220423124554.png]]
In a curved lane, the rover should recognize the curvature of the lanes and stay between the lines as it adjusts.

**Merge:**
![[Pasted image 20220423123027.png]]
This scenario deals with a common merge that is found on most roads. The rover must be able to merge from the right lane and into the main lane. 

**Roundabout:**
![[Pasted image 20220423123807.png]]
In the roundabout, the rover needs to recognize that it should follow the right-hand side until it finds the exit lane.

**T-Intersection:**
![[Pasted image 20220423124020.png]]
In the T-Intersection, the rover must recognize the path forward ends, and be able to turn in a right direction.

**Cul-de-sac:**
![[Pasted image 20220423124336.png]]
In a Cul-De-Sac, the rover must recognize the single black line and follow it around until it exits where it came from.

## Question 2
![[Pasted image 20220423121257.png]]
### Q2 Answer


## Question 3
![[Pasted image 20220423131234.png]]
### Q3 Answer

## Question 4
![[Pasted image 20220423131252.png]]
### Q4 Answer
1. Is Main() method in a file by itself?

2. Do conditionals use `=` instead of `==`?

3. Are there switch constructs with no breaks?

4. Is Initialization performed in one place?

5. Is there redundant code that is eligible for subroutine?