# Preliminary idea
## Mission Overview
Disaster Scenario:
A coastal town has been severely flooded. Residents are trapped on rooftops without access to food, clean water, or medical supplies. After 48 hours of continuous rain, the weather has cleared, enabling aerial rescue efforts.
## Objective:
1. Develop two quadcopter drones to assist in rescue operations by:
 1. Scanning a 30-hectare area.
 2. Streaming real-time video.
 3. Geotagging survivors' locations.
 4. Communicating with stranded individuals via onboard speakers.

## Drone 1: Surveillance Unit
A quadcopter is the optimal platform for surveillance in disaster-stricken environments due to its high manoeuvrability, lightweight structure, and efficient energy consumption. In flooded urban areas with obstacles like power
 lines, trees, and damaged buildings, quick directional changes and precision hovering are crucial capabilities where quadcopters excel. But the most important one of them all is the faster deployment.

2. System Architecture
### Airframe
Type: Quadrotor
1. Material: Carbon fiber or aluminium alloy for durability and lightweight
2.Camera: Gimbal-stabilized FHD+ camera (1440p) for real-time video
3. GPS Module: u-blox NEO-M8N or similar for precise location tracking
4. Speaker: Waterproof Speaker with 85–100 dB output at 1m.
5. Microcontroller: Pixhawk or CubePilot flight controller
6. Communication Link: 4G/LTE module or 5.8 GHz analog video transmitter with a ground receiver

## Drone 2: payload dropping
Type: Hexacopter
A hexacopter is well-suited for payload delivery missions in disaster relief scenarios due to its higher lifting capacity, greater stability, and built-in redundancy. 
When delivering essential supplies like food, water, or medicine to stranded individuals, the drone must carry significant weight and maintain stable flight, even in turbulent conditions.

## Mechanism

The payload delivery hexacopter is equipped with foldable arms and movable landing feet to enhance its functionality in disaster-stricken environments. 
The foldable arm design allows the drone to be compactly stored and easily transported, which is essential for quick deployment in emergencies where space and time are limited.
Once on site, the arms can be swiftly unfolded and locked into position, enabling the drone to be operational within minutes. 
The movable landing feet provide critical clearance beneath the drone for the payload drop mechanism, ensuring safe and unobstructed release of supplies such as food, water, or medicine. 
These feet also offer greater adaptability for landing on uneven or sloped surfaces, which are common in flooded or damaged areas. 
Together, these features make the hexacopter highly versatile, portable, and reliable for executing precise and safe payload delivery missions.
All the electronics will be similar to the quad but with certain adaptations for the benifit og the hexacopter.

## Why Quadcopter + Hexacopter?

| Feature           | Surveillance Quadcopter     | Payload Hexacopter              |
|------------------|-----------------------------|---------------------------------|
| Agility          | High (lightweight)          | Moderate (heavy payload)        |
| Endurance        | ~35 min                     | ~25 min                         |
| Stability (wind) | Good                        | Excellent (6 motors)            |
| Redundancy       | Limited                     | Better motor failure tolerance  |
