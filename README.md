# 10 Meter Walk Test Data
## Overview
This dataset captures detailed lower limb movement data during a 10-meter walk test, which is useful for gait and mobility analysis. The data is collected using two tilebox sensors, strategically positioned to capture a comprehensive set of motion parameters.

Each sensor records the following types of data:

Accelerometer Data: Measures linear acceleration, providing insights into the speed and direction of leg movements.
Gyroscope Data: Captures angular velocity, aiding in the analysis of limb rotation and stability during walking.
Magnetometer Data: Records magnetic field data, useful for determining the orientation and heading of the sensors relative to the Earth's magnetic field.
Temperature Data: Monitors ambient or sensor temperature, which can impact sensor performance or provide environmental context.

The dataset also includes a YAML file containing demographic and lifestyle information for each participant, which provides critical context for data interpretation. The YAML file details include:

Demographic Information: Gender, age, weight, height.
Physical Activity: Frequency, duration, and type of exercise (e.g., walking).
Diet and Nutrition: Dietary habits, portions of fruits or vegetables consumed, daily water intake.
Health Status: Presence of health pathologies (e.g., motor-related issues), smoking status, and current physical state.
Sleep and Energy Levels: Average hours of sleep and perceived energy levels.
Motivation and Participation: Interest in participating in the study.
Mobility Aids: Use of walking aids, if applicable.


## Usage Notes
In order to test the jupyter notebooks available in this repository, we recommend using Python Virtual Environment so to not pollute your python installation. The following commands will help you create a Python Virtual Environment. **Be aware that Python 3 is required to be installed in your machine**

Firstly, install python Venv:
```bash
sudo apt install python3.12-venv
```

After installing it, change directory to the repository:
```bash
cd /path/to/this/git/repo/TMWT-Data
```

Now, let's create a new virtual environment inside this repository folder:
```bash
python3 -m venv .
```
With this command, some new folders should've been created in the directory you are in at the moment.

Let's start the Python Environment
```bash
source bin/activate
```

Let's install pip inside this new enviroment:
```bash
python -m ensurepip --upgrade
```

And right after that, we need to install all the requirements, using pip:
```bash
pip3 install -r requirements.txt
```

You now should be able to run the jupyter notebooks.



In order to exit the python environment, you can run the following command:
```bash
deactivate
```
