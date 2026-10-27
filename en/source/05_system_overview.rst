.. _System Overview:

System Overview
***************

.. _Compatibility:

Compatibility
++++++++++++++++

The |product_name| series includes two products: Mini2 and Mini2C.

- The control cabinet for Mini2 is the MiniCab Pro.
- The control cabinet for Mini2C is the MiniCab Lite.

.. _System Architecture:

System Architecture
+++++++++++++++++++++

.. figure:: ../../images/05_系统概述/Pro机器人系统连接.*
    :align: center
    :width: 15cm
    
    Robot system components of Mini2

.. figure:: ../../images/05_系统概述/机器人系统连接.*
   :width: 15cm
   :align: center

   Robot system components of Mini2C

As is shown in the figure above, the JAKA robot system contains following components: 

1. Robot: A six axes robotic arm which moves as programmed by the user. It consists of buttons for dragging and point teaching and a I/O interface for connecting tools (the TIO interface) on joint 6.
2. Control cabinet: The control cabinet includes the core computing components and various electrical interfaces.
3. Robot connection cable: Cable connection robot to control cabinet.
4. Control cabinet power: The control cabinet accepts a DC input and supports a wide voltage range of 30–60 VDC. A 48 V supply is recommended.
5. Operation terminal: The users desired teaching device.
6. Router and network cable: The control cabinet is equipped with Ethernet ports. These ports can be connected either directly to the operation terminal or to a router, in which case the operation terminal can also connect to the router’s Wi‑Fi network.
   It is recommended to configure a specialized router for the robot to prevent conflicts with other devices.
7. Control stick: Only Mini2 has a control stick by default. Power on/off and enable/disable the robot, etc.

.. attention:: 

   When the control cabinet is integrated into the hybrid robot, it must be connected to isolated power supply to avoid burning. 