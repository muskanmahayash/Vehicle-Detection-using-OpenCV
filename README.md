The vehicle counting system used here is made up of three main components:
•	Detector
•	Tracker and 
•	Counter
The detector identifies vehicles in a given frame of video and returns a list of bounding boxes around the vehicles to the tracker. The tracker uses the bounding boxes to track the vehicles in subsequent frames. The detector is also used to update the trackers periodically to ensure that they are still tracking the vehicles correctly. The counter counts vehicles when they leave the frame or makes use of a counting line drawn across a road.
Algorithm Introduction
•	In our system we are using Background SubtractorMOG algorithm. Background subtraction (BS) is a common and widely used technique for generating a foreground mask (namely, a binary image containing the pixels belonging to moving objects in the scene) by using static cameras.
•	As the name suggests, BS calculates the foreground mask performing a subtraction between the current frame and a background model (Fig.4), containing the static part of the scene or, more in general, everything that can be considered as background given the characteristics of the observed scene.

