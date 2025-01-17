---
layout: post
title:  "Understand Reinforcement Learning with a simple example"
description: An example of reinforcement learning.
date:   2019-09-24 00:17:00 +0530
categories: Reinforcement Python
---

When I started learning about Reinforcement Learning, I read an example which helped me understand the situations where one should use **reinforcement learning**. So, in this blog post I am sharing that example with you guys...

Imagine a simple game wherein you have a robot that runs from left to right and must avoid obstacles by jumping over them at the right time. If your robot successfully clears an obstacle, it gets 1 point, but if the robot runs into it, it loses points. The goal of the game, is to make sure that robot clear the obstacles without getting crashed. Although it sounds simple in concept, this is a great starting point for understanding how reinforcement learning works and how you can use it to solve the problem.
![RL](https://user-images.githubusercontent.com/23660137/63797534-e1285300-c925-11e9-81e6-483b3a0ffc49.gif)

In applying reinforcement learning to this problem, you could first give the robot the ability to jump at various distances while approaching an obstacle.
For an instance, it could jump from 20 feet away, 10 feet away, 3 feet away, or even 0 feet away and crash into the obstacle before actually launching upwards. After a lot of trial and error experimenting with situations like when to jump, your robot will eventually learn that it will receive a point by jumping just before hitting an oncoming obstacle (maybe that's 3 feet away) - because that jumping-off point leads to a successful clearing of the obstacle. Your robot will also learn that it will quickly lose points by jumping too early (say, 20 feet away) or too late (say, 1 foot away) - as jumping-off points that are too far from or too close to an obstacle will lead to a crash. The reward and punishment, in the form of points, positively reinforces the action of jumping at that ideal point, eventually making your robot quite skilled at clearing the obstacles.

Of course, this game can get more complicated if the goal becomes, for an instance, how quickly the robot can clear 10 obstacles in a row, or how well it can clear obstacles that require changing its direction. In this more complicated game, the robot could gain control over its speed and its ability to move in different directions.

By using reinforcement learning to help your robot succeed at this game the robot is now not only experimenting with different timings of its jumps, but the speed at which it runs and the specific direction of its jumps. Like the timing of jumps, the robot will receive rewards and punishments for the speeds and directions that result in more points and less points, respectively. Again, through a lot of trial and error, your robot will eventually learn the right mix of jumping time, speed, and direction to successfully clear a whole series of obstacles.
