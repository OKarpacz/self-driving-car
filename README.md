# AI-Driven Self-Driving Car Simulation 🚗🤖

This project demonstrates a neural network-based self-driving car simulation where AI-powered vehicles learn to navigate a road while avoiding traffic. The goal is to showcase how machine learning techniques can be applied to train cars to drive autonomously in a virtual environment.

## Key Features:
1. **Canvas-Based Simulation**:
   - **Car Canvas**: Visualizes the cars' movement and interaction with the road and traffic.
   - **Network Canvas**: Visualizes the neural network structure of the best-performing car.

2. **Road and Traffic Generation**:
   - The simulation generates a road with multiple lanes, along with various traffic vehicles acting as obstacles.
   - Traffic cars are randomly placed in different lanes to challenge the AI-controlled cars.

3. **AI-Controlled Cars**:
   - Generates a fleet of AI-controlled cars that learn to drive based on a neural network.
   - **Best Car Selection**: The simulation identifies the best-performing car based on its progress on the road and uses it for further training.
   - Neural networks are saved and loaded from `localStorage`, allowing persistent learning across sessions.

4. **Neural Network Mutation**:
   - When previous learning data is loaded, the neural networks of all cars (except the best one) are slightly mutated to explore different strategies.
   - Mutation rate can be fine-tuned for optimal learning.

5. **Visualization and Real-Time Updates**:
   - The car simulation continuously updates and renders the road, traffic, and cars.
   - The neural network visualization provides insights into how the AI processes inputs and makes decisions.

## Functions:
- **Save**: Stores the best-performing car's neural network in the browser's `localStorage` for later use.
- **Discard**: Removes the stored neural network data, resetting the learning process.
- **Generate Cars**: Creates a specified number of AI cars with identical initial setups, all learning in parallel.

## Installation and Usage:
1. Clone the repository:
   ```bash
   git clone https://github.com/OKarpacz/self-driving-car.git
