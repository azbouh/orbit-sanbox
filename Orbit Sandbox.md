# Orbit *Sandbox*

Every body pulls on every other body. Pick a system, then throw something into it.

Drag to launch

Systems

Next body

Mass8

Drag on the field to launch. Time holds while you aim, and the dotted line shows its next few seconds.

Time

Speed1.0×

[x] Trails [x] Merge on contact

Readout

Bodies

0

Sim time

0

Energy drift

0

Drift is the change in total energy since the last reset. It restarts when a body is added, merged or lost.

## Integrator

Velocity Verlet with a fixed step of 0.1. Gravity is softened (`ε = 2`) so a near miss cannot throw a body out of the screen, and the energy readout uses the same softened potential.

## Launch preview

While you drag, the page copies the whole system and runs it forward, so the dotted path includes the pull of every body and the new body's pull back on them.

## A good test

Load the figure eight: three equal masses chase each other along one curve. The energy drift should stay tiny. Then throw a light body through it and watch it fall apart.

G = 1 · world unit u · range rings every 100 u · no libraries, one canvas