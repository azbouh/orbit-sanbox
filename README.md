# Orbit Sandbox

A gravity simulator that runs in the browser. Load a system, drag on the field to launch a new body, and watch every mass pull on every other.

## Run it

Open `index.html` in a browser. There is nothing to install or build.

## What it does

- Presets: solar system, figure eight (three equal masses on one curve), binary stars with planets, debris disc, and an empty field.
- Drag to launch a body. Time holds while you aim, and a dotted line previews the body's next few seconds, including its pull on the other bodies.
- Controls for the mass of the next body, speed, trails, and merge on contact.
- A readout of body count, simulation time, and energy drift.

## How it works

- Velocity Verlet integrator with a fixed step of 0.1.
- Softened gravity (epsilon = 2), with the same softened potential used for the energy readout so the drift number is meaningful.
- The launch preview copies the whole system and runs it forward at a larger step.
- Units: G = 1, one world unit is 1 u, range rings every 100 u.

Plain HTML, CSS and JavaScript on one canvas. No libraries.

## License

MIT. See `LICENSE`.
