# FLIGHT CONTROLLER

## STEP 001 : OBJECTIVE, REQUIREMENTS AND SPECIFICATIONS

### OBJECTIVE :

Build a flight controller from scratch that can be used for drones in racing competitions and autonomous missions.

REQUIREMENTS  :

PERFORMANCE REQUIREMENTS ( PERFORMANCE METRICS ) :

Since this is a project where we are mainly focusing on learning things while we build them, we will not care very much about high performance. So, having the data requirement for this is not required for now.

SPECIFICATIONS ( will be added on the basis of components available ) :

- [ ]  

Flight controllesr should be 

HARDWARE REQUIREMENTS : 

1. BRAIN : microcontrollers. there are two types of microntrollers :
    1. MCU: microcontroller unit.  contains a processor core, memory, and programmable input/output peripherals on a single chip.
        1. ARDUINO : not better than STM32.
        2. STM32 : better because of high processing speed.
    2. MPU : microprocessor unit.  designed for general-purpose computing tasks and often have high processing power. general purpose controller.
        1. rasberry pi.
    
    SO, WE ARE GOING TO LOOK FOR MCUs as MPU is not generally recommended for real time applications where quick response is required as it is multifunctional. But since, we are building a complete flight controller on it, we will use MPU, rasberry Pi 4.
    
2. SENSORS : 
    1. gyroscopes : To know the drone’s rotation around different axes.
    2.  accelerometer : Measrures acceleration.
    3. Magnetometer : another kind of GPS.
        
        THE ABOVE SENSORS ARE BOUGHT TOGETHER AS IMU( inertial measurement unit )
        
    4. barometer : measures atmospheric pressure to mentain stable flight.
    5. **GPS (Global Positioning System):** Provides location data, enabling drones to follow waypoints and return to a designated location. 
    6. **Ultrasonic Sensors:** Used for short-range obstacle detection and ranging.
    7. **Radar:** Another sensor for obstacle detection, particularly useful in challenging conditions.
    8. **Camera Systems:** Used for various purposes, including visual navigation, object detection, and image capture. Some drones utilize thermal cameras for applications like search and rescue or infrastructure inspection.
3. CONNECTIVITY :
    1. RECIEVER PORT :
    2. TELEMETRY PORT :
    3. ESC OUTPUTS : 
    4. CAMERA CONNECTIVITY :
4. FIRMWARE : Software, that helps us to program our drone.
5. POWER SUPPLY :
    - 3.3 V is the standard industry volatge on which most of the circuits work. So, we are going to give 3.3V power supply.

## STEP 002 : DECIDING COMMPONENTS AND PLANNING THE CIRCUIT

### PLANNING THE CIRCUIT :
  STEP 001 : 
SETTING UP A GYROSCOPE : 

components : microelectromechanical systems (MEMS), processor, sensor module : MPU6050 , breadboard, wires, voltage source.

PIN DIAGRAM : 

[![pin_diagram_mpu6050.png](attachment:de70c617-09f5-4078-aac0-db606f2674d9:20241114235404375.png)](https://www.ariat-tech.com/upfile/images/a2/20241114235404375.png)

Here, MPU6050 uses data collected from 6 AXIS : 3-axes:gyroscope and 3-axes accelerometer.

Data is transferred through I2C protocol. 

Vcc : input voltage for the sensor to work.

Ground : to complete the circuit.

Serial Clock → SCL : clock for the circuital part of communication.

Serial Data → SDA : This is the place fromm where data is being transferred.

Auxiallary Serial Data → Place where you can put the data from other axes like magnetometer and integrate all the 9 axes data at MPU6050 itself.

Auxiallary Clock → Clock for Aux I2C protocol circuit.

I2C address Select ( ADO ) → This port helps to MPU6050 have a different I2C address if a circuit is having more than one MPU6050.

Interrupt Pin ( INT ) → This pin helps to reduce load from processor as it notifies to processor whenever new data has been produced and eliminating the polling process.

 ( to be continued… )
( to be continued… )
