---
title:  "Asteroid Retrieval Mission"
date:   2018-03-09
categories: project
post_id: 2
---
My final project for my Space Mechanics class was to conduct an asteroid retrieval mission. We were told a spacecraft would depart from Earth on a trip to an asteroid to capture a boulder from the asteroid and return it to an orbit around the Moon. It was required to design the trajectory of the spacecraft from Earth departure until the final orbit around the Moon. The assumptions given consisted of the following:
* Spacecraft has a 6 Ton dry mass
* Only impulsive thrusters
* Trajectory should be computed with as small as possible fuel mass
* Target is to return a boulder of mass 10 Tons from the asteroid
* The mission can start anytime between January 2018 and December 2019
* Duration of the mission should not exceed 6 years

#### Introduction
Near Earth objects (NEO) have become increasingly desirable  locations to navigate over recent decades because  of the insight asteroids give to the earlier formation of our solar system and beginning of life on Earth. My team was contracted to manifest the trajectories of one of these missions to retrieve samples from a NEO asteroid. To keep fuel mass as low as possible, a lunar fly-by will be performed before rendezvousing with the asteroid. After rendezvousing with the asteroid for several days, the spacecraft has been instructed to return to Earth and perform capture maneuvers to arrive at an orbit around the Moon. The timeline has been set to start the mission between January 2018 and December 2018 and should not exceed 6 years.

### Research
#### NASA's Asteroid Redirect Mission (ARM)
To begin our project, we first sought out other missions involving NEO's. The first mission we found was NASA's Asteroid Redirect Mission (ARM). This mission is still in its developmental phase, but purposes the first-ever robotic mission to visit a large near-Earth asteroid. Similar to our objectives, ARM intends to collect a multi-ton boulder from the asteroid surface and redirect the payload to a stable orbit around the moon. The goal of this mission is to further the advancement of technologies and spaceflight necessary to perform a manned mission to the Martian system in the 2030's. NASA has stated that in the process of selecting a potential asteroid, they are taking into account their velocities, orbit sizes and spin. These are similar parameters that we took into account when selecting an asteroid for the retrieval mission. This mission also helped demonstrate what kind of planetary defense techniques are needed to deflect dangerous asteroids if they were to ever collide with Earth.


<i>See more about NASA's ARM mission [here!](https://www.nasa.gov/content/what-is-nasa-s-asteroid-redirect-mission)
</i>
#### David B. Reid, University of Colorado Boulder
Another mission proposal we found was written by David B. Reid at the University of Colorado Boulder. In Reid's research project titled "The Use of Gravity Assist Flybys in Plane Change Maneuvers", he explained as proposed mission the asteroid 1036 Ganymed that utilizes a lunar flyby. Because of the asteroids large size, it is a primary candidate for an asteroid-mining mission. As David describes, there are four phases for his mission: parking orbit departure, lunar flyby, hyperbolic Earth departure, and Hohmann target-intercept, respectively. He explains how important is it to work backwards through the trajectories, for example, the delta V's necessary for the asteroid orbit insertion must first be known before performing a lunary fly-by and so on. The mission specifically utilizes a flyby of the south pole of the moon to study the Shackleton Crater, predicted to have a layer of water ice at the bottom of its 4.2 km depth. This demonstrates that flybys not only have trajectory advantages, but valuable research can occur if location of the maneuver is taken into account.

<i>You can check out David's full research project [here!](http://ccar.colorado.edu/asen5050/projects/projects_2012/reid/)
</i>
### Asteroid Selection
To start to get an idea of what kind of asteroid we should look to traveling to, my team utilized the [NASA Ames Research Center Trajectory Browser](https://trajbrowser.arc.nasa.gov "NASA Ames Research Center Trajectory Browser"). As seen in the picture below, the tool lets the user search the JPL small-body database using credentials such as when the launch should occur, for how long and how much delta V used to carry out the mission.

<figure class="imagecenter">
<img src="{{site.url}}/assets/img/asteroid_selection.png" alt="asteroid selection">
<img class="padded" src="{{site.url}}/assets/img/orbital_diagram.png" alt="orbital diagram">

<figcaption><i>NASA Ames Research Center Trajectory Constraints</i> </figcaption>
</figure>

When selecting asteroids, we had to keep in mind that some asteroids had perigees that came too close to lining up with the orbital trajectory of Earth. This causes the use of a lunar flyby to become unnecessary since the delta V that would be produced would be too high for our mission needs. With this information in mind, we search the JPL small body database for near-Earth asteroids with small eccentricities, relatively high perigees and within the same plane as Earth plus of minus one degree. We ultimately chose asteroid 2012 EJ5, whose orbit can be seen in the above picture on the right. It has a low eccentricity at 0.3162, an inclination of 0.1871 degrees, and perigee radius of 2.27 x 10<sup>8</sup> km. The synodic period was also found to be approximately 829 days, proving that many rendezvous opportunities would be available within the mission timeline.

### Maneuvers
As previously discussed, my team utilized the approach that David B. Reid used in his research project with a few tweaks. The following sections describe the different stages of the mission and maneuvers purposed to be performed during them. The numbers that are presented were calculated using a MatLab code which can be found at the end of this post.   

### Parking Orbit Departure
Starting at position (1), the spacecraft would be required to make an impulsive maneuver in order to perform a Hohmann transfer to a larger orbit. Using our code, the total delta V for the impulse was found to be 3.1315 km/s. After several days, the spacecraft will arrive at the Moon and will need to make an impulse of around 0.831 km/s in order to enter the sphere of influence.

### Lunar Fly-by
Once in the Moon's sphere of influence we can begin to conduct our flyby maneuvers. This is the part of the mission we struggled the most on due to the complicated vector math involved.

### Hohmann Transfers
After the velocity boost of the lunary flyby, we can begin to perform a simple Hohmann transfer to the asteroid. To calculate the total delta V necessary for this maneuver, we first need to
<img src="{{site.url}}/assets/img/hohmann_transfer.jpg" alt="Hohmann Transfer">

### Earth Lunar Altitude Insertion and Phasing

#### Lunar Insetion

#### Closing Notes
Although this project was not easy and we weren't able to find everything out as a team, it challenged our research skills and made us persevere.

#### References
