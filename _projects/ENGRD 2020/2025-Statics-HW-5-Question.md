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

Based on these free body diagrams, I solved for the equilibrium equation, $$\Sigma M_B = x cm * F_{Load} - F_{LA} * (150-x)cm$$
and the equation $$\arctan({{x*sin(\theta) cm - 10 cm}\over {(150-x)cos(\theta)}})=\theta'$$ with $$\theta=\arcsin({{50 cm}\over{150 cm}})=19.5\degree$$ so $$\arctan({{x*sin(19.5\degree) cm - 10 cm}\over {(150-x)cos(19.5\degree)}})=\theta'$$