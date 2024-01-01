# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: Take the Ep core robot insert the battery and check the battery percentage


Step2: Turn on the robot and connect the robot to the computer through WIFI


Step3: Open visual studio and import robomaster package and do all the code


Step4: Take the measurment of the track on each and every turn and gives the valuse through code in (m)


Step5: run the program to see the robot movement


## Program
```python
import time
from robomaster import camera
if _name=='__main_':
    ep_robot=robot.Robot()
    ep_robot.initialize(conn_type='ap')

    ep_chassis= ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera= ep_robot.camera

    print('video streaming started ...')
    ep_camera.start_video_stream(display=True,resolution= camera.STREAM_360P)


    ep_chassis.move(x=2.4,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0.5,y=0,z=80,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=1,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=90).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.3,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")
    
    ep_chassis.move(x=0,y=0,z=-28,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=1.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=255,effect="on")
    
    ep_chassis.move(x=0,y=0,z=36).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=204,effect="on")

    ep_chassis.move(x=0,y=0,z=98).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=225,b=255,effect="on")

    ep_chassis.move(x=2.04,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=204,effect="on")

    ep_chassis.move(x=0,y=0,z=85).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=128,b=128,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![292491196-ec03b6c7-db70-4459-9915-0bfa5314ee36](https://github.com/nataraj26/mobilerobot-openloopcontrol/assets/147514615/b60e5e72-0000-49f3-9234-6ffba7e4ac11)




<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here
https://youtube.com/shorts/fH1QrrpZba4?feature=share



<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
