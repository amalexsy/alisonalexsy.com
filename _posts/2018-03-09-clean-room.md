---
title:  "Cleanroom Sensor System"
date:   2018-03-09
categories: project
post_id: 1
---
The goal of my senior design was to design an automated sensor system that will be placed in the enterprise's clean room to provide continual monitoring on environmental parameters, including humidity, temperature and pressure. The anticipated outcome was a report describing whether the clean room meets ISO 8 requirements and methods to mitigate any current or future problems.

#### What is the MTU Aerospace Enterprise?
The MTU Aerospace Enterprise is composed of a diverse multidisciplinary group of over 50 students. Students work together on innovative and relevant Aerospace related projects, and all members contribute towards achieving specific project goals. Through the Aerospace Enterprise students are able to enhance their engineering and Aerospace knowledge, as well as develop personal and leadership skills that will provide valuable work experience before graduation. Additionally, students work closely with industry sponsors whose contributions play a vital role to the Enterprise's success.

The first team I joined on the enterprise was the Structures team, responsible for the development of the satellite's structure.  During my time on structures, I helped design the components of the satellites by using Solidworks and Siemens NX. Additionally, I performed FEA analyses to ensure designs could withstand extreme environments. I learned to design with manufacturability and cost efficiency in mind.

Later on I joined the Ground Support Equipment team, responsible for the development of systems that are used to support the spacecrafts while on the ground. I was the team lead of the Electrical Ground Support Equipment (EGSE) whose purpose is to test and interact with the spacecraft before launch. The EGSE is a remote unit that plugs into the satellite to charge its battery, edit the software loaded on its main computer, and monitor the status of its electronic. The GSE team also maintains the Class 100,000 Clean Room on Michigan Tech's campus that is used to work with flight hardware.

#### Goal of my Senior Design
The goal of my senior design was to design an automated sensor system that will be placed in the enterprise's clean room to provide continual monitoring on environmental parameters, including humidity, temperature and pressure. The anticipated outcome was a report describing whether the clean room meets ISO 8 requirements and methods to mitigate any current or future problems.

#### What is a Clean Room? Why is it important?
The Aerospace Enterprise has a Class ISO 8 clean room, meaning that according to the International Organization for Standardization (ISO) 14644-1, the air can contain <i>at most</i> 3,520,000 particles per cubic meter.

{% include table.html %}

The lower the class, the stricter the particle count becomes. Without any sort of sensor system, our organization had no way of actually proving that we were meeting these standards, which is where my senior design came in.




#### IoT Integration
<img align="right" src="{{site.url}}/assets/img/iotready_logo_hardware.png" width="40%">

Because I had basic circuit and software experience I sought after a platform where I could combine my sensors in very user friendly way. My research lead me to find a website called MyDevices and their product called Cayenne.[1](https://mydevices.com/) Cayenne allows users to build complete and ready-to-use IoT solutions with little to no coding during the process. It allows the user to use their own hardware and submit any device into the their library using MQTT API. The main two ways to connect the devices together was either with an Arduino or a Raspberry Pi. I decided to take the Raspberry Pi route because it seemed to not have as high of a learning curve.







#### Sensor Selection
  1. Pressure
<img align="right" src="{{site.url}}/assets/img/pressure_sensor.jpg">


  2. Airflow velocity
  3. Humidity and Temperature



#### References
[1]: https://mydevices.com/
