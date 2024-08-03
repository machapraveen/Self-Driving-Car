# Self-Driving Car Simulator Project

This project implements an autonomous driving system using a neural network model to control a car in the Udacity Self-Driving Car Simulator.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Prerequisites](#prerequisites)
3. [Project Structure](#project-structure)
4. [Installation and Setup](#installation-and-setup)
5. [Running the Simulator](#running-the-simulator)
6. [Model Training](#model-training)
7. [Troubleshooting](#troubleshooting)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview

This project uses a trained convolutional neural network (CNN) to predict steering angles for a car in a simulated environment. The model takes images from the car's "camera" as input and outputs appropriate steering commands, allowing the car to navigate autonomously around a track.

## Prerequisites

- Python 3.8
- Udacity Self-Driving Car Simulator (Download from [here](https://github.com/udacity/self-driving-car-sim))
- Conda (recommended for environment management)

## Project Structure

```
self-driving-car-sim/
│
├── drive.py           # Script to run the model in autonomous mode
├── model.h5           # Trained Keras model
├── training.py        # Script used to train the model (if applicable)
├── utils.py           # Utility functions
├── requirements.txt   # List of required Python packages
└── README.md          # This file
```

## Installation and Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/self-driving-car-sim.git
   cd self-driving-car-sim
   ```

2. Create and activate a new conda environment:
   ```
   conda create --name sdcar python=3.8
   conda activate sdcar
   ```

3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Running the Simulator

1. Ensure your `model.h5` file is in the project directory.

2. Start the drive script:
   ```
   python drive.py
   ```

3. Launch the Udacity Self-Driving Car Simulator.

4. Select the desired track.

5. Click the "Autonomous Mode" button.

The car should now drive autonomously using the trained model.

## Model Training

The `model.h5` file contains a pre-trained CNN model. If you wish to train your own model:

1. Collect training data using the Udacity simulator in training mode.
2. Use the `training.py` script to train the model:
   ```
   python training.py
   ```

Adjust hyperparameters in `training.py` as needed for optimal performance.

## Troubleshooting

- If you encounter "ModuleNotFoundError", ensure all required packages are installed:
  ```
  pip install -r requirements.txt
  ```
- For issues with TensorFlow, try installing a specific version:
  ```
  pip install tensorflow==2.4.1
  ```
- If problems persist, try using a virtual environment instead of conda:
  ```
  python -m venv sdcar_venv
  source sdcar_venv/bin/activate  # On Windows use: sdcar_venv\Scripts\activate
  pip install -r requirements.txt
  ```

## Contributing

We welcome contributions to improve this project! Here's how you can contribute:

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

Please ensure your code adheres to the project's coding standards and include tests for new features.

## License
