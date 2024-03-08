# Validating a Low-Cost Single-Channel fNIRS Device Across Cognitive Tasks

This repository contains the code used in our paper "Validating a Low-Cost Single-Channel fNIRS Device Across Cognitive Tasks". This code is being made open-source in response to a request from the reviewers.

## Paper Information

- Title: Validating a Low-Cost Single-Channel fNIRS Device Across Cognitive Tasks


## Code Description

This repository includes the following code files:

vv.exe: These files are related to receiving and plotting data from LSL (Lab Streaming Layer) streams in real-time. The vv.py script demonstrates use cases for receiving data from all found outlets and plotting them.

tran.exe: This script reads a file named wordlist.csv, shuffles its content randomly, and then writes the shuffled characters into a new CSV file distractorlist.csv in groups of 7 characters. This might be for generating some random distractor items.

portlsl.spec and portlsl.py: These files involve selecting a COM port using a GUI, setting up a serial connection, and handling different types of LSL inlets (data and marker inlets). The script pulls data from the inlets and sends it over the selected COM port.

lslslv.exe: This script creates a GUI application for HEG (Hemoencephalography) recording. It allows connecting to a serial port, starting and stopping LSL streaming, and sending data to another COM port (COM10). It also interacts with Psychopy for experiment control.

lslsl.spec and lslsl.py: These files implement a serial monitor application using a GUI. It allows selecting data and marker ports, specifying an output CSV file, and starting/stopping the recording. The script reads data from the selected ports and writes it to the CSV file along with timestamps.

