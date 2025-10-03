---
layout: project
title: Linear Actuator Max Height
description: Statics Project
technologies: Desmos
image: /assets/images/Screenshot 2025-09-30 103823.png
---

For statics class, we were asked to design a structure with a linear actuator, a rod, and 3 pins, in a 2D space of 50cm by 150cm to lift the greatest load to the highest height possible.

I ended up choosing a design of a lever to allow me to lift the load to the max height of 50 cm, while still applying the maximum load possible to the side without the linear actuator being applied.

 ![Photo of linear actuator]({{ "assets/images/Screenshot 2025-10-02 103830.png" | relative_url }}){: .inline-image-r style="height: 250px"}
Assumptions/Given: I assumed that the linear actuator was 10 cm tall when it was fully retracted. I chose to use the RSH hygenic rod-style actuator, which had a force of up to 35 kN.

Based on this, I drew out a free body diagram for the entire system, using the full design space possible, including a 150 cm long bar, using the pins to pin the linear actuator to the ground and the rod, and to pin the rod to the ground to make the lever. The starting configuration with the linear actuator fully extended is on the left, while the ending configuration with the linear actuator fully retracted is on the right.
![Photo of starting configuration]({{ "assets/images/Screenshot 2025-10-02 104413.png" | relative_url }}){: .inline-image-l style="width: 220px"}![Photo of ending configuration]({{ "assets/images/Screenshot 2025-10-02 105109.png" | relative_url }}){: .inline-image-r style="width: 300px"}

Based on these free body diagrams, I solved for the equilibrium equation,

$$
\Sigma M_B =0= x \, cm \cdot F_{Load} - F_{LA} \cdot (150-x)\,cm
$$

and the equation

$$
\arctan\left(\frac{x \sin(\theta)\, cm - 10\, cm}{(150-x)\cos(\theta)}\right) = \theta'
$$

with

$$
\theta = \arcsin\left(\frac{50\,cm}{150\,cm}\right) = 19.5\degree
$$

so

$$
\arctan\!\left(\frac{x \sin(19.5\degree)\,\text{cm} - 10\,\text{cm}}{(150-x)\cos(19.5\degree)}\right) = \theta'
$$

The max height that can be reached is then given by

$$
\text{H}_{Max}=150\sin(\theta')+10\text{cm}
$$

where the maximum height is equal to 50cm, so &theta;'=15.47 degrees. Plugging these values into the arctan equation gets an x value of 82.61096, and plugging that value into the original sum of moments equation gets a max load of 28.55089 kN, being able to be raised 50 cm.

![Photo of Desmos solving the equations]({{ "_site/assets/images/Screenshot 2025-10-03 142115.png" | relative_url }}){: .inline-image-l style="width: 220px"}

This value is slightly less than the max load that the linear actuator can raise, but it allows the load to be lifted to the maximum height, which maximizes both values to the best of my ability.