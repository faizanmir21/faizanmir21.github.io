---
layout: default
---

# Cooperative Air-Ground Robot Localization


![Kalman Filter](../Images/Ball_Balancer/State_Estimation.png)

The UGV’s motion is modeled kinematically here as a simple 4-wheeled steerable Dubin’s car 
![Kalman Filter](../Images/Ball_Balancer/estdyn1.png)

The fixed-wing UAV motion is modeled kinematically as a simple Dubin’s unicycle 
![Kalman Filter](../Images/Ball_Balancer/estdyn2.png)

## System Model
The nonlinear equations of motion describing the Cooperative Air-Ground Robot Localization system is defined as: 
![Kalman Filter](../Images/Ball_Balancer/estmodel1.png)

The combined system state, control inputs, and disturbance inputs are 
![Kalman Filter](../Images/Ball_Balancer/estmodel2.png)

The measurement model for the system is given by a combination of noisy ranges and azimuth angles of the UGV relative to the UAV and noisy UAV GPS measurements 
![Kalman Filter](../Images/Ball_Balancer/estmodel3.png)

## Linearization
The continuous-time nonlinear dynamics and measurement models can be linearized by first assuming that the system stays near a nominal trajectory x*(t) for some nominal control input u*
![Kalman Filter](../Images/Ball_Balancer/estlin1.png)
![Kalman Filter](../Images/Ball_Balancer/estlin2.png)

Using Taylor Series expansion near x∗, the CT linearized system is approximated as:
![Kalman Filter](../Images/Ball_Balancer/estlin3.png)
![Kalman Filter](../Images/Ball_Balancer/estlin4.png)
![Kalman Filter](../Images/Ball_Balancer/estlin5.png)
