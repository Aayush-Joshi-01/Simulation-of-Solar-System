# Solar System Simulation with PyGame

This Python project simulates the inner solar system based on Newton's law of gravity using the PyGame library. The simulation is modular, allowing you to easily incorporate other celestial bodies by specifying their coordinates. It accurately mimics the solar system when accurate planet coordinates are provided.

## Features

- Accurate simulation of the inner solar system.
- Modularity for adding additional celestial bodies.
- Customizable time constraints to adjust simulation speed.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Modifying the Simulation](#modifying-the-simulation)
- [Equations and Concepts](#equations-and-concepts)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/solar-system-simulation.git
```

2. Install the required dependencies using pip:

```bash
pip install pygame
```

## Usage

1. Navigate to the project directory:

```bash
cd solar-system-simulation
```

2. Run the simulation:

```bash
python main.py
```

3. Use the following controls to interact with the simulation:

   - **Mouse Click**: Add celestial bodies (e.g., planets) with specified coordinates.
   - **Arrow Keys**: Adjust the simulation speed (up/down arrows).
   - **Spacebar**: Pause/Resume the simulation.
   - **Esc**: Exit the simulation.

## Modifying the Simulation

### Adding Celestial Bodies

To add celestial bodies like planets, asteroids, or moons, modify the `celestial_bodies` list in `main.py`. Each body should be represented as a dictionary with the following properties:

- `name`: Name of the celestial body.
- `mass`: Mass of the celestial body (in kilograms).
- `radius`: Radius of the celestial body (in meters).
- `color`: Color of the celestial body (in RGB format).
- `position`: Initial position of the celestial body as a tuple `(x, y)` in meters.
- `velocity`: Initial velocity of the celestial body as a tuple `(vx, vy)` in meters per second.

### Customizing Time Constraints

You can customize the time step used in the simulation for better accuracy or to speed up the simulation. Modify the `time_step` variable in `main.py`. Smaller time steps improve accuracy but may slow down the simulation, while larger time steps can make it faster but less accurate.

## Equations and Concepts

### Newton's Law of Gravitation

The gravitational force between two objects is calculated using Newton's law of gravitation:

\[
F = \frac{{G \cdot m_1 \cdot m_2}}{{r^2}}
\]

Where:
- \(F\) is the gravitational force between the two objects.
- \(G\) is the gravitational constant.
- \(m_1\) and \(m_2\) are the masses of the two objects.
- \(r\) is the distance between the centers of the two objects.

### Centripetal Force

The centripetal force required to keep an object in circular motion is calculated as:

\[
F_{\text{centripetal}} = \frac{{m \cdot v^2}}{r}
\]

Where:
- \(F_{\text{centripetal}}\) is the centripetal force.
- \(m\) is the mass of the object.
- \(v\) is the velocity of the object.
- \(r\) is the radius of the circular path.

In the simulation, this centripetal force is used to calculate the necessary velocity adjustments for objects in orbit.

## Contributing

Feel free to contribute to this project by opening issues or creating pull requests. Your contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Enjoy exploring the inner solar system through this Python simulation! If you have any questions or encounter issues, please don't hesitate to contact us.
