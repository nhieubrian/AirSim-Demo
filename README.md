*Note: This readme and demo was created alongside 2 AIP students*

# AirSim Reinforcement Learning

## File Location: -- This was done because GitLab was not allowing the large file sizes.

Part 1: https://gitlab.nautilus.optiputer.net/aip_197_accchi/purple_nl/AirSim

*Note: This drive is only accessible for UCSD members*

Part 2: https://drive.google.com/drive/folders/1ww7ipw26vJ_Ap1Ph-0f7iSBuSxXaEm4w?usp=sharing

## Installation

### Installing Unreal Engine

Download the Epic Games Launcher
https://www.epicgames.com/store/en-US/download 

Once downloaded, install Unreal Engine 4.25 in the Library Section

### Building AirSim

Install Visual Studio 2019
Make sure to select Desktop Development with C++ and Windows 10 SDK 10.0.18362

Clone the Repository on GitLab on your local computer

Follow Documentation to set up on Windows
https://microsoft.github.io/AirSim/build_windows/ 

Follow Documentation to set up Blocks Environment
https://microsoft.github.io/AirSim/unreal_blocks/ 

## How to Use

### Car Demo

Follow Documentations to set up VS solution file to run demo: https://microsoft.github.io/AirSim/unreal_custenv/ 

Open LandscapeMountains.sln file and set configurations to DebugGameEditor and Win64

Press F5 to run

In Window/World Settings, set GameMode Overrride to AirSimGameMode

In Edit/Editor Preferences, search for ‘CPU’ and make sure that ‘Use Less CPU when in Background’ is unchecked

Save and Press Play

Once car simulation has loaded, you can first attempt to drive the arrow keys and see that it can drive

Also a camera appears with the car simulation

#### Image of Car Simulation with Camera

![alt text](/images/CarDemoCamera.png)


## Examples

### Reinforcement Learning

Install Anaconda and with Anaconda install stable-baselines3 with command
```
pip install stable-baselines3[extra]
```
Once installed, use Anaconda command line to go into the AirSim/PythonClient/reinforcement_learning directory and run command
```
python dqn_car.py
```

There may be missing modules that cause errors when running this command and we can download these modules using pip install

Once all modules are downloaded, run the command 
```
python dqn_car.py
```

If the command works, you will begin to see the car drive on its own and reset if there are obstructions

#### Image of Reinforcement Learning with Car Simulation

![alt text](/images/CarDemoRL.png)

#### Image of Command Prompt Returns

![alt text](/images/CarDemoRLCommand.png)



## Resources

AirSim Documentation

https://github.com/Microsoft/AirSim/#how-to-use-it 

https://microsoft.github.io/AirSim/ 

AirSim Setup on Windows

https://microsoft.github.io/AirSim/build_windows/ 

AirSim Setup for Blocks Environment

https://microsoft.github.io/AirSim/unreal_blocks/ 

AirSim Custom Unreal Environment

https://microsoft.github.io/AirSim/unreal_custenv/ 

AirSim Reinforcement Learning

https://microsoft.github.io/AirSim/reinforcement_learning/ 







