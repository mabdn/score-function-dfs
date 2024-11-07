# Score Function DFS for Path Planning in Autonomous Racing

## Summary

Here, I present a path planning algorithm I developed at KA-RaceIng for its autonomous electric race car, the KIT24.
Given a map of cones marking the track, the algorithm finds the path through the race track.
It superseded KA-RaceIng's previous approach to path planning because it can tolerate mistakes in the map (e.g. false positive or false negative cone detection).

<p align="center" float="left">
  <a href="https://www.ka-raceing.de/"><img src="assets/ka-raceing_logo.png" height="166px"></a>
  &nbsp;
  &nbsp;
  &nbsp;
  &nbsp;
  &nbsp;
  &nbsp;
  <a href="assets/ka-raceing_kit23.jpg" target="_blank">
  <img src="assets/ka-raceing_kit23.jpg" height="166px">
  </a>
</p>

## Demo

Witness our race car in action: executing precise maneuvers with path planning on the race track (first) and employing cornering velocity planning, another technique I contributed to (second).

<https://github.com/mabdn/score-function-dfs/assets/93079021/66038b40-8097-43d2-b00d-ff6f92832168>

<https://github.com/mabdn/score-function-dfs/assets/93079021/85f6e870-fdb0-4f2b-966b-64d09f0ee609>

This RVIZ visualization showcases how my path-planning algorithm performs. It was recorded during real-world driving.

<https://github.com/mabdn/score-function-dfs/assets/93079021/54c0ab32-bf42-401e-b637-bb3fde20ae58>

## Description

This repository presents one part of my contribution to KA-RaceIng's autonomous racing software during a 7-month part-time (15h/week) position as **Autonomous Driving Software Engineer** at Karlsruhe Institute of Technology's Formula Student team KA-RaceIng.

### Results and Experience Gained

- Re-designed the path planning algorithm to improve **path planning safety** to have fewer laps with planning mistakes
- Finished code others started for **reducing the autonomous lap time** by estimating the cornering stability of the car and accelerating to drive at its stability limit
- Automated the project’s GitLab CI pipeline to check **code style and formatting rules automatically** with a custom Docker Linux image

### What is KA-RaceIng and Formula Student?

KA-RaceIng is a racing team of students from *Karlsruhe Institute of Technology* competing in *Formula Student*.
*Formula Student* is an international engineering competition. 50-member teams from universities around the world design, build, and code autonomous electric full-sized race cars.

KA-RaceIng is one of the world's best formula student teams in autonomous racing. E.g.,

- 2nd place in Formula Student Germany 2023 (driverless)
- 1st place in Formula Student Hungary 2022 (driverless)
- 1st place in Formula Student Germany, Hungary, and Czech 2021 (driverless)

### Technologies Used

- **C++17** Programming Language
- **ROS** Robotics Software Framework
- **Docker Containers** for Continuous Integration
- **GoogleTest** Unit Test Framework

## License

The code I wrote in this project is private. The KA-RaceIng team actively uses it. It is the core of path planning at KA-RaceIng and contributes its part to our success in autonomous racing. Hence, I cannot publish any of this code here. I can give you more insights in a personal discussion, though.
