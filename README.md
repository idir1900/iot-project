# iot-project
light-house monitoring



What is the problem and why do you need IoT?
for several centuries ships and boat were used to find the port by the help of lighthouses,and thoes lighthouses were runing all nights all days whether there is a boat comming to the port or not wasting by that energy and loose efficiency that's why i introduce you this iot system in purpose of monitoring the energy consumed by lighthouses depending on proximity of ships and the visibilty of the weather.

You need to identify an application scenario that you would like to address. What are you going to learn by monitoring the environment - which type of sensors will help you? How will you act into the environment and by what actuators?
depending on if there is a ship or ships near by the light house we can adjust le angle of rotation of the light house and also the brightness of it so if we take as example a boat that is coming toward the port the light of the lighthouse will decrease according to the disantce between the ship and the port so no more waste of energy and also the led will be directed to this ship so no more energy waste in rotating the led.
we will use a GPS to detect the position of the ship and a Photosensor for the visibility,we will act on the lighthouse with a led controlled by PWM and a servo motor to fix the light to the specific ship 

the gps will send data every 30 seconds and the visibility will be sent every 1 minute when the ship is near enough 

the average range of a light house is 16 km so when the gps indicate a distance <= 16 the brightness will be at the maximum and decrease depending on the distance separating the ship to the lighthouse 
if there two or more ship the brightness will be set to fit the farest one and if the boat in the range of the 16 km are not moving for 3 cycle the led of the lighthouse will be off till the ship rebigin to move.
the brightness depend also on the clarty of the sky if there some fog the bright will increase to reach the ship. 
the servo motor is controlled depending on the angle between the ship and the lighthouse and if there two or more ships the servo motor will do 180° back and forward 


What data are collected and by which sensors?
the data collected is the position in latitude and longitude  and the visibility of the sky 
Given the sensors selected, identify the type of data collected by the specific sensor component by examining the manufacturer's datasheet. You need to report the accuracy of the component, the unit of measurement and the desired periodicity of the measurements.
Report the velocity, variability and variety of the data collected by your application.
Describe the data analysis that is required to transform the data collected from sensors. What kind of collective intelligence do you expect will emerge?
What are the connected components, the protocols to connect them and the overall IoT architecture?
Provide a network diagram that includes all the devices and identifies the network and communication protocols used to interconnect them.
Identify the software components that make up your system both at IoT device level and at cloud level.
Provide a high-level architecture diagram that depicts the interdependencies of your software components.
