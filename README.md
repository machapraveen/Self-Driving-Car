# Self-Driving Car Simulator Project

This project uses a trained neural network model to autonomously drive a car in the Udacity Self-Driving Car Simulator.

## Prerequisites

- Python 3.8
- Udacity Self-Driving Car Simulator (available [here](https://github.com/udacity/self-driving-car-sim))
- Conda (recommended for environment management)

## Project Structure

```
self-driving-car-sim/
│
├── drive.py
├── model.h5
└── README.md
```

## Setup Instructions

1. Clone this repository:
   ```
   git clone [Your Repository URL]
   cd self-driving-car-sim
   ```

2. Create and activate a new conda environment:
   ```
   conda create --name sdcar python=3.8
   conda activate sdcar
   ```

3. Install the required packages:
   ```
   pip install tensorflow
   pip install opencv-python
   pip install pillow
   pip install python-socketio==4.6.0
   pip install python-engineio==3.13.2
   pip install eventlet
   pip install flask
   ```

4. Ensure that `model.h5` (your trained model) is in the project directory.

## Running the Simulator

1. Start the drive script:
   ```
   python drive.py
   ```

2. Launch the Udacity Self-Driving Car Simulator.

3. Select the track you want to test on.

4. Click the "Autonomous Mode" button.

The car should now start driving autonomously using the trained model.

## Troubleshooting

If you encounter issues with conda, try using a virtual environment instead:

1. Create a new virtual environment:
   ```
   python -m venv sdcar_venv
   ```

2. Activate the virtual environment:
   - On Windows: `sdcar_venv\Scripts\activate`
   - On macOS and Linux: `source sdcar_venv/bin/activate`

3. Install the required packages as listed in step 3 of the Setup Instructions.

## Model Training

The `model.h5` file was trained using [briefly describe your training process and data]. For details on the model architecture and training process, refer to [link to your training code or documentation].

## Additional Notes

- This project uses TensorFlow and Keras for the neural network model.
- The `drive.py` script interfaces with the Udacity simulator using Socket.IO.
- Ensure your computer meets the system requirements for running the Udacity Self-Driving Car Simulator.

## Contributing

We welcome contributions to improve the Self-Driving Car Simulator Project! Here's how you can contribute:

1.Fork the repository on GitHub.
2.Clone your forked repository to your local machine.
3.Create a new branch for your feature or bug fix.
4.Make your changes and commit them with clear, descriptive commit messages.
5.Push your changes to your fork on GitHub.
6.Submit a pull request to the main repository.

Please ensure your code adheres to the existing style of the project to maintain consistency. Also, make sure to update the README.md with details of changes to the interface, including new environment variables, exposed ports, useful file locations, and container parameters.

## Reporting Issues
If you find a bug or have a suggestion for improvement:

Check the GitHub Issues to see if the bug or suggestion has already been reported.
If not, open a new issue. Clearly describe the issue or suggestion, including steps to reproduce when it is a bug.

Thank you for your contributions to make this project better!

## License

This project is licensed under the MIT License - see below for details:
MIT License
Copyright (c) [2024] [MachaPraveen]
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.