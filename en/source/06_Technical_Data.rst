.. _Technical-Data:

Technical Data
**************

.. _Technical Specifications:

Technical Specifications
+++++++++++++++++++++++++++

.. _Robot-Technical-Specifications:

Robot Technical Specifications
===============================

.. csv-table:: Robot technical specifications
   :file: ./tables/Robot technical specifications.csv
   :encoding: utf-8-sig
   :widths: 34 33 33
   :header-rows: 1

.. container:: table-notes

   :sup:`1` When the ambient temperature is below 10°C, warm up the robot before use; otherwise, the robot may stop or operate at a reduced speed.

.. _Control cabinet technical specifications:

Control cabinet technical specifications
=========================================

.. csv-table:: Control cabinet technical specifications
   :file: ./tables/Control cabinet technical specifications.csv
   :encoding: utf-8-sig
   :widths: 10 10 40 40
   :header-rows: 1

.. _Dimensional-Drawings:

Dimensional Drawings
++++++++++++++++++++

.. _Robot Outline Dimensions:

Robot Outline Dimensions
==========================

The sizes of the |product_name| robots are shown below. During the installation, the motion range of the robot must be considered to avoid injury to or collision with surrounding personnel and equipment.

.. figure:: ../../images/06_技术规格/外形尺寸图.*
   :width: 6cm
   :align: center

   Outline dimensions

.. _Robot-Working-Space:

Robot Working Space
====================

When the robot is mounted, a cylindrical space must be considered. Due to the robot being in close proximity of a singularity, it is recommended to keep the robot end outside of this workspace. If the previously mentioned recommendations are not followed, the robot might perform at lower efficiency and create difficulties in the risk assessment. The working space of the |product_name| robots are shown below.

.. figure:: ../../images/06_技术规格/工作空间.*
   :width: 15cm
   :align: center

   Working space

.. _Control Cabinet Dimension:

Control Cabinet Dimension
==========================

.. figure:: ../../images/06_技术规格/MiniCabLite外形尺寸图.*
   :width: 17cm
   :align: center

   Outline dimensions of control cabinet

.. _Electrical Specifications:

Electrical Specifications
+++++++++++++++++++++++++++

.. include:: Electrical Specifications.rst

.. _Indicators:

Indicators
+++++++++++++

.. _Ring-Shaped-Light:

Ring-Shaped Light
====================

Ring‑shaped indicator light on the base indicates the robot status. 
The position of the ring-shaped lights is shown in figure below.

.. figure:: ../../images/06_技术规格/环形指示灯.*
   :width: 3.44cm
   :align: center

   Ring-shaped light

.. list-table:: Meaning of ring-shaped light color
   :widths: 46 54
   :header-rows: 1

   * - **Color**
     - **Robot State**

   * - Blue
     - Powered on but disabled

   * - Green
     - Enabled

   * - Red
     - Failure/Protective stop

   * - Yellow
     - Freedrive mode

   * - Yellow flash
     - Pause

   * - Yellow flash
     - Single-step program debugging

.. _Control Cabinet Light:

Control Cabinet Light
======================

.. _MiniCab Lite Light:

MiniCab Lite Light
--------------------

The |Lite| has an indicator light on the front panel. The color definitions are as follows.

.. figure:: ../../images/06_技术规格/指示灯位置.*
   :align: center
   :width: 12cm

   Power indicator

.. list-table:: Meaning of indicator color
   :widths: 40 60
   :header-rows: 1

   * - **Name**
     - **Function**

   * - Power indicator
     - Green: control cabinet is powered up

.. _MiniCab Pro Light:

MiniCab Pro Light
--------------------

The |Pro| has two indicator lights — a power indicator and a status indicator — both located on the front panel.

.. _Power Indicator:

Power Indicator
~~~~~~~~~~~~~~~~~

.. figure:: ../../images/06_技术规格/电源指示灯位置.*
    :align: center
    :width: 12cm

    Power indicator

The color definitions of power indicator are as follows.

.. list-table:: Meaning of power indicator color
   :widths: 40 60
   :header-rows: 1

   * - **Color**
     - **Function**

   * - Green
     - Control cabinet is powered up

.. _Status Indicator:

Status Indicator
~~~~~~~~~~~~~~~~~~

.. figure:: ../../images/06_技术规格/状态指示灯位置.*
    :align: center
    :width: 12cm

    Status indicator

.. list-table:: Meaning of ring-shaped light color
   :widths: 46 54
   :header-rows: 1

   * - **Color**
     - **Robot State**

   * - Blue
     - Powered on but disabled

   * - Green
     - Enabled

   * - Red
     - Failure/Protective stop

   * - Yellow
     - Freedrive mode

   * - Yellow flash
     - Pause

   * - Yellow flash
     - Single-step program debugging

.. _Buttons:

Buttons
+++++++++

.. _Free-and-Point-Buttons:

Free and Point Buttons
=========================

The robot is equipped with a tool I/O interface (TIO) and two buttons on the side of the flange. 
The two buttons are a freedrive button (FREE) and a point recording button (POINT), 
as shown in figure below.

.. figure:: ../../images/06_技术规格/末端法兰按钮.*
  :width: 7cm
  :align: center

  Free and point button

| **1** Point button
| **2** Free button

When the Free button is pressed, the robot enters the freedrive mode. 
The robot can be dragged to the desired position manually.

The Point button is used with the |jaka_app|. When this button is pressed, 
the corresponding position will show up in the programming interface of the App as a command (see |jaka_app| Software User Manual for details).

.. warning::
  
  User must first assess the risks before using the free drive and point buttons. 
  Ensure that the robot’s mounting orientation, end payload, TCP, and other parameters are correctly set, 
  otherwise it may cause injury to personnel or damage to the equipment.

.. _Control Cabinet Buttons:

Control Cabinet Buttons
=========================

.. _MiniCab Lite Button:

MiniCab Lite Button
---------------------

The power button of |Lite| is located on the front panel and is used to power the device up and down as follows:

.. figure:: ../../images/06_技术规格/Lite电源按钮位置.*
    :align: center
    :width: 12cm

    Power button

- Power up: Press the POWER button for 1 seconds, and then the control cabinet will be powered up.
- Power down: Press the POWER button for more than 3 seconds, and then the control cabinet will be powered down.

.. _MiniCab Pro Button:

MiniCab Pro Button
---------------------

.. _Power Button:

Power Button
~~~~~~~~~~~~~~~

The power button of |Pro| is located on the front panel and is used to power the device up and down as follows:

.. figure:: ../../images/06_技术规格/Pro电源按钮位置.*
    :align: center
    :width: 12cm

    Power button

- Power up: Press the POWER button for 1 seconds, and then the control cabinet will be powered up.
- Power down: Press the POWER button for more than 3 seconds, and then the control cabinet will be powered down.

.. _Network Reset Button:

Network Reset Button
~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: ../../images/06_技术规格/网络复位按钮位置.*
   :align: center
   :width: 12cm

   Network reset button

**RST Wi-Fi:** Control cabinet's Wi-Fi reset button. Press and hold for 8 seconds, 
the Wi-Fi configuration is restored to factory default settings. 
This includes all parameters configured within the |jaka_app| “Wi-Fi Settings > AP Device Networking” interface.

The reset button is housed in a 2 mm diameter bore and can be depressed using a 1.5 mm slotted ESD-safe screwdriver.

.. _Robot Calibration Orientation:

Robot Calibration Orientation
+++++++++++++++++++++++++++++++

The robot calibration orientation is the orientation adopted during robot calibration. Calibration marks are 
stuck onto joints and tubes, being used for recalibration after joint replacement. When all adjacent marks are 
aligned, the robot is in the calibration orientation. 

The joint angles for the calibration are listed below.

.. list-table:: A5L calibration joint angle
   :widths: 17 17 17 17 17 15
   :header-rows: 1

   * - **Joint 1**
     - **Joint 2**
     - **Joint 3**
     - **Joint 4**
     - **Joint 5**
     - **Joint 6**

   * - 0°
     - 0°
     - 0°
     - 0°
     - 0°
     - 0°

.. figure:: ../../images/06_技术规格/机器人标定姿态.*
   :width: 2cm
   :align: center

   Robot calibration orientation

.. _Robot-Rotation-Direction:

Robot Rotation Direction
++++++++++++++++++++++++++

Refer to :ref:`Robot-Technical-Specifications` for robot rotation range. 
The rotation direction is as follows:

.. figure:: ../../images/06_技术规格/机器人旋转方向.*
   :width: 7cm
   :align: center

   A5L rotation direction

.. _Robot-Singularity:

Robot Singularity
++++++++++++++++++

Singularities are positions described in Cartesian space that have no impact on MoveJ. When the robot is at a singularity, replace the Cartesian movement by MoveJ if the motion can be achieved by MoveJ. If there is singularity in the middle of the robot’s motion path, the robot’s trajectory can be changed to bypass the singularity. You can also change the robot's mounting position or the size of the end effector to change the value of Cartesian points in the robot's joint space. A singularity is a robot arm configuration where one or more degrees of freedom are lost causing the robot to be stuck in a position and unable to move. This usually occur when joint axes align in one way or another.

When a robot is at a singularity, the following effects may occur:

- Robots cannot move in one or more directions.
- The robot cannot find a suitable set of joint angles for the TCP to move to the desired position.
- The robot joint should move at high speed to achieve the desired TCP speed.
- Intense movements near singularities will result in accidents and shorten the lifespan of robot joints.

The robot has three types of singularities: shoulder singularities, elbow singularities and wrist singularities. Descriptions and avoidance methods of the singularity are as follows.

**Shoulder singularity:** When the axes intersection of the joint 5 and joint 6 lies on the plane of axes of joint 1 and joint 2, the robot is at shoulder singularity.

.. figure:: ../../images/06_技术规格/肩部奇异姿态.*
   :width: 7cm
   :align: center

   Shoulder singularity

Ways to avoid shoulder singularity:

- Ensure that the robot TCP is not directly above the robot base. TCP cannot reach the positions directly above the robot. A shoulder singularity will occur if the TCP approaches a position directly in line with the base Z axis.
- Do not use MoveL when the angle of joint 1 is 180 between two points in space. When the difference is about 180°, the robot reaches shoulder singularity. You can use MoveJ to avoid singularity or set an intermediate transition point outside the shoulder singularity range.

**Elbow singularity:** When joints 2, 3 and 4 are coplanar or when joint 3 is 0°, the robot is at elbow singularity.

.. figure:: ../../images/06_技术规格/肘部奇异姿态.*
   :width: 7.23cm
   :align: center

   Elbow singularity

Ways to avoid elbow singularity:

- When the robot is at an elbow singularity, it indicates that the target position is close to the limits of the working range of the robot. At this point, it is necessary to adjust the robot mounting position or extend the length of the end effector.

**Wrist singularity:** When joint 4 and joint 6 are collinear or when joint 5 is 0°, the robot is in wrist singularity.

.. figure:: ../../images/06_技术规格/腕部奇异姿态.*
   :width: 7cm
   :align: center

   Wrist singularity

Ways to avoid wrist singularity:

- The wrist singularity typically occurs in movements with orientation changes. Therefore, in cases of considerable orientation change, it is advisable to prioritize MoveJ and not use Cartesian motions such as MoveL or MoveC.

.. _Control-Stick-Buttons:

Control Stick Buttons
+++++++++++++++++++++

.. include:: Control Stick Buttons.rst

.. _Performance-Data:

Performance Data
++++++++++++++++

.. _Load-Capacity-of-the-Robot:

Load Capacity of the Robot
==========================

The maximum payload of the robot is related to the offset of the gravity center, and degree of the offset is related to the distance between the center of robot end flange and the payload centroid. Figures below show the relation between the payload and the offset of the gravity center:

- X: Center of gravity offset
- Y: Payload

.. figure:: ../../images/06_技术规格/Mini2负载偏心图.*
   :width: 15cm
   :align: center

   Load capacity

.. note::

   Offset distance is the center of gravity distance from the center of the flange.

.. _Stopping-Time-and-Distance:

Stopping Time and Distance
==========================

The time from the application of a stop signal to the standstill of the robot is measured. 
This measurement is carried out for various reaches and velocities (measurement according to ISO 10218-1).

Safety stopping time is the time it takes to stop the robot from the moment when the emergency stop button is pressed or a safety protection function is triggered. 
The stopping distance is the distance the end of the robot moves during the safety stopping time. Among them, pressing the emergency stop button falls into Cat.1, 
while triggering the safety protection function falls into Cat.2. During this period, the robot is still moving and may harm the personnel or other equipment. 
Therefore, users and integrators should consider this time and distance in risk assessment.

The test conditions are as follows:

- Speed: 100%, 66%, 33%
- Reach: 100%, 66%, 33%

.. list-table::
   :class: no-auto-merge
   :widths: 9 30 29 32
   :header-rows: 1

   * -
     - **100% Reach**
     - **66% Reach**
     - **33% Reach**

   * - **Joint 1**
     - .. figure:: ../../images/06_技术规格/J1-100.*
          :width: 4cm
          :align: center

     - .. figure:: ../../images/06_技术规格/J1-66.*
          :width: 3.6cm
          :align: center

     - .. figure:: ../../images/06_技术规格/J1-33.*
          :width: 3.1cm
          :align: center

.. list-table::
   :class: no-auto-merge
   :widths: 9 30 29 32
   :header-rows: 1

   * -
     - **100% Reach**
     - **66% Reach**
     - **33% Reach**

   * - **Joint 2**
     - .. figure:: ../../images/06_技术规格/J2-100.*
          :width: 4.29cm
          :align: center

     - .. figure:: ../../images/06_技术规格/J2-66.*
          :width: 3.6cm
          :align: center

     - .. figure:: ../../images/06_技术规格/J2-33.*
          :width: 3.1cm
          :align: center

.. list-table::
   :class: no-auto-merge
   :widths: 20 40 40
   :header-rows: 1

   * -
     - **100% Reach**
     - **66% Reach**

   * - **Joint 3**
     - .. figure:: ../../images/06_技术规格/J3-100.*
          :width: 3.5cm
          :align: center
     - .. figure:: ../../images/06_技术规格/J3-66.*
          :width: 3.1cm
          :align: center

- Load: See the table below.

.. list-table:: Load of stopping time and distance test
   :widths: 48 52
   :header-rows: 1

   * - **Model**
     - **Payload**

   * - Mini2，Mini2C
     - 2 kg (4.4 lb) 

See :ref:`Appendix 1: Stopping Time and Distance` for the respective stopping distance and time of Cat.1 and Cat.2.

.. warning::

   **Breakdown of the internal joint holding brake:**

   - Take into account a possible breakdown of the internal joint holding brake during your risk assessment.
   - Take into account that the internal joint holding brake of the JAKA robot only withstands a limited number of brake operations.

   Failure to follow these instructions can result in death, serious injury, or equipment damage.

If there is a power interruption of the control system, the brakes are applied and the robot mechanics may leave the planned trajectory.

.. warning::

   **Leaving the planned trajectory of the robot mechanics:**

   - Use the buffering of the 24 V supply (UPS) in order to enable a controlled stop of the mechanics, in accordance with stop category 1, by making use of the stored residual mechanical and electrical energy.
   - Use a synchronous stop on the path to avoid collisions with obstacles.
   - Observe the extension of the run-on path while performing your risk assessment.

   Failure to follow these instructions can result in death, serious injury, or equipment damage.

.. _Forces-and-Torques-on-Robot-Base:

Forces and Torques on Robot Base
================================

The illustration shows the directions of the robot stress forces.

.. figure:: ../../images/06_技术规格/机器人底座力和转矩方向.*
   :width: 5.27cm
   :align: center

   Directions of forces and torques on robot base

| Fx: Force in X direction
| Mx: Bending torque in X direction
| Fy: Force in Y direction
| My: Bending torque in Y direction
| Fz: Force in Z direction
| Mz: Bending torque in Z direction

The table below shows the maximum forces and torques in various directions working on the robot base.

.. csv-table:: Forces and torques on robot base
   :file: ./tables/Forces and torques on robot base.csv
   :encoding: utf-8-sig
   :widths: 40 60
   :header-rows: 1

.. attention::

   These forces and torques are maximum values that are rarely encountered during operation. The values also never reach their maximum at the same time!

.. _Torques-on-Robot-Flange:

Torques on Robot Flange
=======================

The table below shows the maximum torques working on the robot flange.

.. csv-table:: Torques on robot flange
   :file: ./tables/Torques on robot flange.csv
   :encoding: utf-8-sig
   :widths: 40 60
   :header-rows: 1