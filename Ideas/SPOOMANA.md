Mission requirement:
A coastal town is flooded. Residents are stranded on rooftops without food, water, or medicine. After 48 hours, the weather improves, and drones are now deployable for rescue support.
Objective:
Part 1: Search and Locate
Scan a 30-hectare area.
Detect survivors visually (actual humans standing in the field).
Geotag their locations.
Communicate with them via a speaker on the drone.


Part 2: Aid Delivery
Deliver survival kits (200g, 5x10x20 cm).
Drop kits accurately within the proximity of survivors.
Aim for Zone A (highest accuracy score).
Drone Requirements: Use 2 drones
1 Scout Drone– detection & geotagging.
1 Delivery Drone – package delivery.
OR build a combined “Scout+Delivery” Drone.


Note: Must operate autonomously, but manual control is allowed with penalties.
Use a Command & Control Station (single interface preferred).
Real-time video, status updates, and control via GCS.
Scoring: 600 points max
Survivor detection (Autonomous: 35 pts per target)
Delivery accuracy:


Zone A: 40 pts


Zone B: 30 pts


Zone C: 20 pts


Note : Manual operation reduces all scores to 60% of autonomous values.






Idea : is to make a Scout Drone (Eye) and a Delivery Drone (Supply).
Scout Drone(EYE) : Autonomously search a mock 30-hectare area to detect and locate survivors.
Components:
  Airframe: Quadrotor (450mm frame, carbon fiber or PLA frame).
 Camera: 1080p RGB module (e.g., Raspberry Pi Camera or ESP32-CAM)
 Onboard Computer: Raspberry Pi 4 or Jetson Nano.

Delivery Drone (SUPPLY): Delivery Drone: Deliver lightweight survival kits to the geotagged locations.
Components:
Airframe: Similar quadrotor with stronger thrust-to-weight ratio.
Payload Dropper: Servo-controlled trapdoor or gripper.
Flight Controller: Pixhawk or Navio2
Payload:
Foam/plastic survival kit box: ~200g (simulate water bottle, snacks, etc.).
Dropped from 15–20 ft.
Mission Execution Workflow
Scout Drone takes off, autonomously follows the uploaded KML route.(SPECIFIED PATH)
It detects “survivors”, geotags them, and plays alert messages.
Coordinates are logged on the control station.
Delivery Drone is assigned those coordinates as waypoints.
Drone flies to each coordinate and drops survival kits accurately.
All mission logs, detections, and drops are recorded for scoring and analysis.




