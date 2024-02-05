# Self-Driving Car Simulation
# Follow the steps defined in the Functionality section to get the desired results.

## Overview

This project demonstrates a self-driving car simulation using JavaScript and HTML5 Canvas. The simulation includes multiple components such as cars, road boundaries, traffic, neural networks for AI control, and user-interaction buttons for saving and discarding the AI's progress.

## Demo
https://musman12529.github.io/Self-Driving-Car/

## Functionality 

- **Save Button**: Triggers the `save()` function, which stores the current best AI brain configuration into the browser's local storage as a JSON object. So when you restart the Simulation the car will follow the best path that was saved using the save button and it should be pressed when the user thinks that the car has covered more distance than the last time. The user should try to press the save button as soon as possible after the car crashes and the other iterations of AI cars takes over, other wise simply reload the page to start over from the previously saved iteration.
- **Discard Button**: Executes the `discard()` function, removing the saved AI brain data from the local storage.

## Components

### Car Class

- **Attributes**: Defines the car's position, dimensions, speed, controls, and AI brain for autonomous control.
- **Methods**: Manages movement, damage assessment, drawing on the canvas, and updates based on road and traffic conditions.

### Control Class

- **Attributes**: Handles control inputs for the car.
- **Methods**: Sets up keyboard event listeners to control the car's movement.

### Neural Network Class

- **Attributes**: Represents a neural network structure with multiple levels.
- **Methods**: Implements feedforward logic for neural network activation and mutation for evolving AI behavior.

### Road Class

- **Attributes**: Defines the road's position, width, lane count, and borders.
- **Methods**: Renders the road with lane dividers and boundaries on the canvas.

### Sensor Class

- **Attributes**: Implements a sensor system for obstacle detection.
- **Methods**: Casts rays to detect intersections with road borders and traffic objects.

## Interactions

### HTML/CSS

- **Canvas**: Displays the simulation environment.
- **Buttons**: Provides options to save and discard AI progress.

### JavaScript

- **`animate()` Function**: Controls the simulation loop, updating car positions, handling traffic, and rendering components on the canvas.
- **`save()` Function**: Saves the best AI brain's progress into the browser's local storage as a JSON object.
- **`discard()` Function**: Removes the saved AI brain data from the local storage.



This project integrates various classes, methods, and event handling in JavaScript to create a comprehensive simulation of a self-driving car environment. Users can interact with the simulation by saving or deleting the AI's learned behaviors through the provided buttons.
