# Neural Circuit Deployment

This is an audio effect plugin designed for the [Neural Audio Plug-in Competition](https://www.theaudioprogrammer.com/neural-audio).

It models a 1951 Fender Deluxe 5A3 guitar amplifier. Neural networks are employed as the circuit modelling approach. Therefore, an iterative solver for differential equations is not required, and performance is consistent and safe for real-time deployment.

Although controls are not included in the model, it does react to input volume changes and can be controlled via the guitarist's playing style.

3 kinds of models are available: a Temporal Convolutional Network (TCN), a WaveNet, and a Long Short-Term Memory (LSTM) Network.

# Wider impact

The same process used in this project can be employed to model any existing or new circuit and deploy it as a real-time audio effect. A good white-box simulation (e.g. SPICE) must exist in order to provide the training data in case of absence of the original device.

# Loading

You can load and run the neural network models in their respective audio plugin projects.

## TCN

To load the Temporal Convolutional Network (TCN) model, you need the [Neutone plugin](https://neutone.space). It's available in VST3 and AU formats. For more information, visit the Neutone website.

## WaveNet

To load the WaveNet model, you need the [Neural Amp Modeller (NAM) plugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin). It's available in VST3 and AU formats.

## LSTM

To load the LSTM model, you need the [Proteus plugin](https://github.com/GuitarML/Proteus). It's available for Windows, Mac and Linux. Make sure to run Proteus at a sample rate of 44.1kHz. 3 Proteus models are provided: Clean, Gain and Pedal. The best performing model is Gain.

# Acknowledgments

* The Audio Programmer community for inspiration and help
* The developers of the NN plugins used in this project and the corresponding training scripts
* The developers of the underlying platforms and frameworks, notably Jatin Chowdhury and Oli Larkin 
* A friend who helped record the live demo and the person who provided the guitar
