---
layout: project
title: Nutcracker Final
description: ENGRD 2020
technologies: ---
image: /assets/images/nutcracker_final.png
---

# Nutcracker design

## Given: 
Dimensions and force to break nut

## Assume:
1) 300 pound force required to break the nut

2) Made of steel

3) Nut acts as a roller support

## Find (a): 
Location of maximum elastic deflection

## Answer:
The point of the linear actuary will be the point of the greatest deflection. Since the force is applied at the end, the further from the pin, the more deformation there will be.

## Find(b):
Beam design where deformation is less than 2% of the length

## Calculations:
max deformation = 0.02 * 9in = 0.18in

Net $$F_y = R_y - F_{la} - 300 = 0$$

Net $$M_pin = 0.5 (300) - F_{la}(9) = 0$$

$$F_{la} = 16.67 lbf$$

$$R_y = 283 lbf$$

Using $$EIy" = M(x)$$ we split the beam into two parts.

For the left part, our equation looks like this:

$$EIy" = F_{la} * (L - x)$$

with boundary conditions y(0) = 0

For the right part, our equation looks like this

$$EIy" = 300x$$

with boundar conditions $$y(0) = 0$$ and $$y(0.5)$$ = 0

Since it's the same beam, the y'(0.5) must be equal for both equations, using this we calculated the equation needed to find inertia


$$y(8.5) = 0.18 = (1/EI) * (0.5(16.67)(9)x^2 - (16.67/6)x^3 - 47.93x)$$

After subbing in 8.5 for x and 29 * 10^6 for E, we get that inertia = 0.0006in^4

Setting our beam as a simple cylinder, using the equation $$I = pi/4 * R^4$$, we find that our diameter is 0.337inch. Ultimately leading to the design of in the following image

## Diagram:
![This is an image of the nutcracker with its dimensions](/sp26-portfolio-caitlyn-c-c/assets/images/nutcracker_final.png)
