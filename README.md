# GenFr


## Table of Contents

- [Introduction](#introduction)
- [Pre-requirement](#pre-requirement)
- [Dataset](#Dataset)
- [Replay](#Replay)

  
## Introduction  
This temporary repository provides some details and additions.  
Our tests are based on generated DSL files. For general considerations and complete anonymity, we will open source the DSL file database after Accept Notification to help the communities in related fields.

Currently, we provide some inplementation details and Supplementary Materials of our work.



## Pre-requirement

### Carla Simulator 0.9.14/0.9.15 Compiled version (Recommended)
### UE4 Engine (Related to Carla version)
### Other Carla-related pre-requirement




## Dataset
In order to facilitate research and discussion in related fields, the reports we use are all real open source reports recorded and released by officials.  
CADMV Disengagement Report: https://www.dmv.ca.gov/portal/vehicle-industry-services/autonomous-vehicles/disengagement-reports/
  
CADMV Crash Report: https://www.dmv.ca.gov/portal/vehicle-industry-services/autonomous-vehicles/autonomous-vehicle-collision-reports/
  
NHTSA Crash Report: https://crashviewer.nhtsa.dot.gov/LegacyNMVCCS/Search
  

## Replay
### Setup

   
Replay the log file in the demo   
Please find the Intro.txt of demo for more details of the demo replay     
Start Carla:            
```
./CarlaUE4.sh
```
Load Map using Carla util:
```
python3 config.py --map XX
```
    
Replay log:      
```
client.replay_file("/path/xx/fileName")
```
Advanced options for replay:    
```
client.replay_file("/path/xx/fileName", start, duration, camera)
```

Start: The time you want to start the simulation    
Duration: The number of seconds you want to play    
Camera: The camera will focus and follow the actor     

Notice: If you have run Carla files before, please make sure you have refreshed the environment. The replay lag is caused by Carla recording/replaying.   


