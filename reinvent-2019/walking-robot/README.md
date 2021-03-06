# Walking Robot #

Learning to walk takes time and a practise for humans to do naturally. It means the ability to stand upright and balanced, then the actions of locomotion and failing and then trying again until we get it right.

Building a robot to do the same is even harder. We have to design the limbs and motors, build a perception system so is understand balance and more importantly we need to use re-enforcement learning, so that it keeps on trying even when it falls.

AWS now has the tools to create such a robot. We use AWS RoboMaker to design, simulate and then help build a physical limbs and motors, we then use Sagemaker to help learn balance and then IoT to control and use feedback of real-world measurements to compare with the simulated data. 

Amazon Sumerian provides a way to create interactive graphical user interfaces to simulate, observe and control the robot. Since it is connected via AWS IoT Shadow to the robot, it does not matter if you are right next to it or miles away.

## Architecture ##

![Architecture Diagram](./docs/Robot-Legs-Diagram.png)

## AWS Services Used ##
- [AWS IoT Core](https://aws.amazon.com/iot-core/)
- [Amazon Sumerian](https://aws.amazon.com/sumerian/)
- [AWS RoboMaker](https://aws.amazon.com/robomaker/)
- [Amazon Cognito](https://aws.amazon.com/cognito/)

## 3d model we created for this demo ##

![Architecture Diagram](./docs/3d-robot.png)

## FAQ ##
__Q: Where can I get the Robot Legs?__

You can buy a MK1 robot set [here](https://www.aliexpress.com/i/32933030622.html).

You can get all the information of building the MK2 [here](https://releasetheinnergeek.com/2018/11/28/walbi-the-walking-biped/).

__Q: What edge/IoT device was used for this project?__

For the MK1 Robot we used a Raspberry PI and a Arduino UNO board with a PWM shield.

For the MK2 Robot we used a Raspberry PI and a Arduino Nano board and a debug board.

## Authors ##
- Munir Hasan munhasan@amazon.co.uk
- Heiko Ihde ihdeheik@amazon.de

# License #

This content is licensed under the Apache 2.0 License.
