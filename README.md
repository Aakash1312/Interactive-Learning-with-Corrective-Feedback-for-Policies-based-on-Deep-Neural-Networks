# Interactive Learning with Corrective Feedback for Policies based on Deep Neural Networks
Code of the paper "Interactive Learning with Corrective Feedback for Policies based on Deep Neural Networks" to be presented at ISER 2018.

This code is based on the following publication:
1. [Interactive Learning with Corrective Feedback for Policies based on Deep Neural Networks (Preprint)](https://arxiv.org/abs/1810.00466) 

**Authors:** Rodrigo Pérez-Dattari, Carlos Celemin, Javier Ruiz-del-Solar, Jens Kober.

Link to paper video:

[![Paper Video](https://www.youtube.com/watch?v=vcEtuRrRIe4)

## Installation

To use the code, it is necessary to first install the gym toolkit (release v0.9.6): https://github.com/openai/gym

Then, the files in the `gym` folder of this repository should be replaced/added in the installed gym folder on your PC. There are modifications of two gym environments:

1. **Continuous-CartPole:** a continuous-action version of the Gym CartPole environment.
2. **CarRacing:** the same CarRacing environment of Gym with some bug fixes and modifications in the main loop for database generation.

### Requirements
* setuptools==38.5.1
* numpy==1.13.3
* opencv_python==3.4.0.12
* matplotlib==2.2.2
* tensorflow==1.4.0
* pyglet==1.3.2
* gym==0.9.6

## Usage

To run the code just type in the terminal inside the folder `D-COACH`:

```python 
python main.py --config-file <environment>
```
To be able to give feedback to the agent, the environment rendering window must be selected/clicked.

## Comments

The D-COACH algorithm is designed to work with problems of continuous actions spaces. Given that the Cartpole environment of gym was designed to work with discret action spaces, a modified continuous version of this environment is used.

This code has been tested in `Ubuntu 16.04` and `python >= 3.5`.

