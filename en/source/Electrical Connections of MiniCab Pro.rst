.. _pro-network-connection:

Network Connection
====================

.. figure:: ../../images/07_运输及调试/电气连接/Pro网口位置.*
    :align: center
    :width: 12cm
    
    Ethernet Port Locations

|Pro| has three Ethernet ports on the rear panel.

   - LAN1: Gigabit Ethernet port with a fixed, non-editable default IP address of 10.5.5.100.
   - LAN2: Gigabit Ethernet port with a dynamic IP address; acts as a DHCP server.
   - LAN3: Gigabit Ethernet port with a fixed, non-editable default IP address of 192.168.108.1.

.. attention::
  
  LAN2 must not be configured with an IP address in the 10.5.5.x subnet. If it is, the message “This subnet is disabled” is displayed.

In addition to the three Ethernet ports, |Pro| has a Wi-Fi module for wireless connectivity.

  - Default name: Control cabinet serial number
  - Default password: JKadmin123

.. _pro-usb-connection:

USB Connection
====================

|Pro| has two USB 3.0 ports on the rear panel. They are for internal debugging only.

.. figure:: ../../images/07_运输及调试/电气连接/ProUSB接口位置.*
    :align: center
    :width: 12cm
    
    USB Port Locations

.. _pro-hdmi-connection:

HDMI Connection
================

|Pro| has one HDMI port on the rear panel for connecting an external display.

.. figure:: ../../images/07_运输及调试/电气连接/HDMI接口位置.*
    :align: center
    :width: 12cm
    
    HDMI Port Location

.. _pro-braking-resistor-connection:

Braking Resistor Connection
============================

|Pro| has two braking-resistor connector sets on the rear panel for connecting braking resistors.

.. figure:: ../../images/07_运输及调试/电气连接/制动电阻接口位置.*
    :align: center
    :width: 12cm
    
    Braking Resistor Connector Location

For braking-resistor connector wiring, use a harness that meets the specifications below.

.. list-table:: Braking resistor connector harness specifications
   :widths: auto
   :header-rows: 1

   * - **Connector model**
     - **Recommended crimp terminal**
     - **Wire cross-section**
     - **Strip length**
   * - DEGSON: DGPS2.5FR-5.0-04P
     - China: E7508
       
       Overseas: PHOENIX AI1-8RD-Ferrule
     - 0.75–2.5 mm² (18–14 AWG)
     - 10 mm (0.4 in)

The wiring is shown below.

.. figure:: ../../images/07_运输及调试/电气连接/制动电阻接线.*
    :align: center
    :width: 6cm
    
    Braking Resistor Wiring

.. _pro-control-stick-connection:

Control Stick Connection
=========================

The STICK connector is for connecting a JAKA control stick. Insert the control stick cable into this connector. The connector is intended only for a JAKA control stick for the control cabinet and must not be modified.

.. figure:: ../../images/07_运输及调试/电气连接/Pro手柄接口.*
    :align: center
    :width: 12cm
    
    Control Stick Connector Location

.. _pro-emergency-stop-device-connection:

Emergency Stop Device Connection
=================================

|Pro| provides one emergency-stop connector. It uses a dual-channel redundant design: the function can be triggered when the signal on either channel is valid. When using external safety equipment, select equipment that supports a dual-channel design. Depending on safety requirements, a safety door, safety light curtain, sensor, or similar device can be connected.

.. figure:: ../../images/07_运输及调试/电气连接/急停接口.*
    :align: center
    :width: 5cm
    
    Emergency Stop Connector

The connector pin assignments are as follows:

#. Internal logic 24 V output
#. Emergency stop input 1; shorted to Pin 1 by default
#. Internal logic 24 V output
#. Emergency stop input 2; shorted to Pin 3 by default

For emergency-stop connector wiring, use a harness that meets the specifications below.

.. list-table:: Emergency Stop Connector Harness Specifications
   :widths: auto
   :header-rows: 1

   * - **Connector model**
     - **Recommended crimp terminal**
     - **Wire cross-section**
     - **Strip length**
   * - DEGSON: 15EDGKNHBM-3.5-04P-14-01A(H)
     - China: E0512
       
       Overseas: PHOENIX AI1-12RD-Ferrule
     - 0.75 mm² (17 AWG)
     - 7~8 mm (0.28~0.31 in)

Factory Default Wiring
------------------------

When no external emergency-stop device is connected, short Pin 1 to Pin 2 and Pin 3 to Pin 4. The factory default connects the inputs to the internal 24 V supply. The wiring diagram is shown below.

.. figure:: ../../images/07_运输及调试/电气连接/急停接口-默认出厂接线.*
    :align: center
    :width: 4cm
    
    Factory Default Wiring

External Emergency Stop Switches
----------------------------------

For safe operation, remove the jumpers and use one or more external emergency-stop switches. The wiring diagrams are shown below.

.. figure:: ../../images/07_运输及调试/电气连接/急停接口-外接急停开关（单路）.*
    :align: center
    :width: 6cm
    
    External Emergency Stop Switch (Single)

.. figure:: ../../images/07_运输及调试/电气连接/急停接口-外接急停开关（多路）.*
    :align: center
    :width: 6cm
    
    External Emergency Stop Switches (Multiple)

.. _pro-io-connector:

I/O Connector
==============

.. figure:: ../../images/07_运输及调试/电气连接/IO接口.*
    :align: center
    :width: 12cm
    
    I/O Connector

.. _pro-io-connector-pinout:

I/O Connector Pinout
---------------------

|Pro| has eight digital inputs and eight digital outputs. The pin assignments are listed below.

.. list-table:: DO connector pinout
   :widths: 20 20 60
   :header-rows: 1

   * - **Pin**
     - **Name** 
     - **Description**

   * - 1
     - UDIO 24V
     - Integrated 24 V interface power output with built-in 2.7 A overcurrent protection
   * - 2
     - UDIO COM
     - Positive common terminal for user-interface power; externally shorted to Pin 1 by default
   * - 3, 4
     - GND
     - User-interface power logic ground
   * - 5
     - DO1
     - Digital output 1, NPN type; can be reused as safety digital output 1
   * - 6
     - DO2
     - Digital output 2, NPN type; can be reused as safety digital output 1
   * - 7
     - DO3
     - Digital output 3, NPN type; can be reused as safety digital output 2
   * - 8
     - DO4
     - Digital output 4, NPN type; can be reused as safety digital output 2
   * - 9
     - DO5
     - Digital output 5, NPN type; can be reused as safety digital output 3
   * - 10
     - DO6
     - Digital output 6, NPN type; can be reused as safety digital output 3
   * - 11
     - DO7
     - Digital output 7, NPN type; can be reused as safety digital output 4
   * - 12
     - DO8
     - Digital output 8, NPN type; can be reused as safety digital output 4

.. list-table:: DI connector pinout
   :widths: 20 20 60
   :header-rows: 1

   * - **Pin**
     - **Name** 
     - **Description**

   * - 1
     - UDIO 24V
     - Integrated 24 V interface power output with built-in 2.7 A overcurrent protection
   * - 2
     - UDIO COM
     - Positive common terminal for user-interface power; externally shorted to Pin 1 by default
   * - 3, 4
     - GND
     - User-interface power logic ground
   * - 5
     - DI1
     - Digital input 1, NPN type; can be reused as safety digital input 1
   * - 6
     - DI2
     - Digital input 2, NPN type; can be reused as safety digital input 1
   * - 7
     - DI3
     - Digital input 3, NPN type; can be reused as safety digital input 2
   * - 8
     - DI4
     - Digital input 4, NPN type; can be reused as safety digital input 2
   * - 9
     - DI5
     - Digital input 5, NPN type; can be reused as safety digital input 3
   * - 10
     - DI6
     - Digital input 6, NPN type; can be reused as safety digital input 3
   * - 11
     - DI7
     - Digital input 7, NPN type; can be reused as safety digital input 4
   * - 12
     - DI8
     - Digital input 8, NPN type; can be reused as safety digital input 4

For I/O connector wiring, use a harness that meets the specifications below.

.. list-table:: I/O Connector Harness Specifications
   :widths: auto
   :header-rows: 1

   * - **Connector model**
     - **Recommended crimp terminal**
     - **Wire cross-section**
     - **Strip length**
   * - DEGSON, 15EDGKNHC-3.5-12P
     - China: E0512
       
       Overseas: PHOENIX AI1-12RD-Ferrule
     - 0.2–1.5 mm² (24–16 AWG) 
     - 8 mm (0.31 in)

Factory Default Wiring
------------------------

The digital I/O is connected to the internal power supply by default. The wiring is shown below.

.. figure:: ../../images/07_运输及调试/电气连接/IO-出厂接线.*
    :align: center
    :width: 8cm
    
    Factory Default Wiring

External Power Supply
-----------------------

For higher output power, use an external power supply. Each channel supports up to 0.5 A. When using an external 24 V supply, remove the jumper between Pin 1 and Pin 2. The wiring is shown below:

.. figure:: ../../images/07_运输及调试/电气连接/IO-外接电源.*
    :align: center
    :width: 9cm
    
    External Power Supply

Digital Input Wiring
---------------------

Connect one wire to GND (Pin 3/4) and the other to the specified DI channel. DI1 is used as an example below.

.. figure:: ../../images/07_运输及调试/电气连接/DI-干接点输入.*
    :align: center
    :width: 9cm
    
    Digital Input Wiring

Digital Output Wiring
-----------------------

Connect one wire to UDIO 24 V (Pin 1) and the other to the specified DO channel. DO1 is used as an example below.

.. figure:: ../../images/07_运输及调试/电气连接/DO-数字输出.*
    :align: center
    :width: 9cm
    
    Digital Output Wiring

.. _pro-safety-io-connector:

Safety I/O Connector
=====================

The |Pro| has four digital inputs and four digital outputs, refer to :ref:`pro-io-connector-pinout` for the connector pinout.

The safety I/O uses a dual-channel redundant design, so a fault in one channel does not disable the safety function. Connect both channels in each safety I/O pair; for example, when connecting I/O 1, also connect I/O 2. The pairings are listed below:

.. list-table:: Safety I/O pairings
   :widths: 50 50
   :header-rows: 1

   * - **DI**
     - **DO**

   * - DI1 & DI2 = SDI1
     - DO1 & DO2 = SDO1

   * - DI3 & DI4 = SDI2
     - DO3 & DO4 = SDO2

   * - DI5 & DI6 = SDI3
     - DO5 & DO6 = SDO3

   * - DI7 & DI8 = SDI4 \ :sup:`1`
     - DO7 & DO8 = SDO4

.. container:: table-notes

   | :sup:`1` SDI4 can only be configured for the protective stop function; other safety functions are not supported.

Safety Digital Input Wiring
----------------------------

Connect one wire to GND (Pin 3/4) and the other to the specified DI channel. SDI1 is used as an example below.

.. figure:: ../../images/07_运输及调试/电气连接/SDI-数字输入.*
    :align: center
    :width: 9cm
    
    Safety Digital Input Wiring

Safety Digital Output Wiring
-----------------------------

Connect one wire to UDIO 24 V (Pin 1) and the other to the specified DO channel. SDO1 is used as an example below.

.. figure:: ../../images/07_运输及调试/电气连接/SDO-数字输出.*
    :align: center
    :width: 9cm
    
    Safety Digital Output Wiring

Connecting Protective Stop Devices
-----------------------------------

|Pro| DI connector Pins 11 and 12 can be reused for the protective stop function. This connector uses a dual-channel redundant design: the function can be triggered when the signal on either channel is valid. When using external safety equipment, select equipment that supports a dual-channel design. Depending on safety requirements, a safety door, safety light curtain, sensor, or similar device can be connected.

.. figure:: ../../images/07_运输及调试/电气连接/外接保护性停止开关（单路）.*
    :align: center
    :width: 10cm
    
    External Protective Stop Switch (Single)

.. figure:: ../../images/07_运输及调试/电气连接/外接保护性停止开关（多路）.*
    :align: center
    :width: 10cm
    
    External Protective Stop Switches (Multiple)

.. _pro-com-connector:

COM Connector
==============

.. _pro-com-connector-pinout:

COM Connector Pinout
---------------------

|Pro| has one 14-pin COM connector for remote power control and RS485 communication. The pin assignments are as follows.

.. list-table:: COM Connector Pinout
   :widths: 20 20 60
   :header-rows: 1

   * - **Pin**
     - **Name** 
     - **Description**

   * - 1, 3, 5
     - UDIO 24V
     - Integrated 24 V interface power output with built-in 2.7 A overcurrent protection
   * - 2
     - UDIO COM
     - Positive common terminal for user-interface power; externally shorted to Pin 1 by default
   * - 4, 6
     - GND
     - User-interface power logic ground
   * - 7
     - Remote Off
     - Remote power-off control input; active at 24 V
   * - 8
     - Remote On
     - Remote power-on control input; active at 24 V
   * - 9
     - CANH
     - CANH for internal debugging
   * - 10
     - CANL
     - CANL for internal debugging
   * - 11
     - Master RS485A
     - Master RS485 communication, 485A
   * - 12
     - Master RS485B
     - Master RS485 communication, 485B 
   * - 13
     - Slave RS485A
     - Slave RS485 communication, 485A
   * - 14
     - Slave RS485B
     - Slave RS485 communication, 485B

For COM connector wiring, use a harness that meets the specifications below.

.. list-table:: COM Connector Harness Specifications
   :widths: 25 25 25 25
   :header-rows: 1

   * - **Connector model**
     - **Recommended crimp terminal**
     - **Wire cross-section**
     - **Strip length**
   * - DEGSON, 15EDGKNHC-3.5-14P
     - China: E0512
      
       Overseas: PHOENIX AI1-12RD-Ferrule
     - 0.2–1.5 mm² (24–16 AWG)
     - 8mm (0.31 in)

.. _pro-remote-power-control-wiring:

Remote Power Control Wiring
---------------------------

The remote power-control inputs are COM Pins 8 and 7, used to control power-on and power-off of |Lite|. They can be connected to a PLC system for remote control of the cabinet. 

.. _pro-remote-power-on:

Remote Power-On
~~~~~~~~~~~~~~~~

Remote power-on requires an external 24 VDC supply. Connect the positive terminal to Pin 8 (Remote On) and the negative terminal to Pin 4/6 (GND). The wiring is shown below.

.. figure:: ../../images/07_运输及调试/电气连接/远程开机.*
    :align: center
    :width: 9cm
    
    Remote Power-On

.. _pro-remote-power-off:

Remote Power-Off
~~~~~~~~~~~~~~~~~

Remote power-off can use either an external 24 VDC supply or the internal UDIO 24 V supply (Pin 1/3/5).

- Internal power supply: If the connected device is a passive dry contact, use the 24 V supply provided by the control cabinet. Connect one wire to internal UDIO 24 V (Pin 1/3/5) and the other to Pin 7 (Remote Off).
- External power supply: Connect the positive terminal to Pin 7 (Remote Off) and the negative terminal to Pin 4/6 (GND).

The wiring diagram is shown below.

.. figure:: ../../images/07_运输及调试/电气连接/远程关机.*
    :align: center
    :width: 18cm
    
    Remote Power-Off

.. attention::
  
  The remote power-on and remote power-off inputs must not be shorted at the same time.

.. _pro-rs485-wiring:

RS485 Wiring
-------------

The RS485 interface enables communication between devices and is provided on COM Pins 11 to 14. Pins 11 and 12 are the master interface; Pins 13 and 14 are the slave interface.

.. note::

  A 120 Ω terminating resistor (YAGEO MF0207FTE52-120R) is recommended.

Control Cabinet as Master
~~~~~~~~~~~~~~~~~~~~~~~~~~

The wiring diagram below shows the control cabinet operating as the master.

.. figure:: ../../images/07_运输及调试/电气连接/RS485-控制柜作主站.*
    :align: center
    :width: 12cm
    
    Control Cabinet as Master

1, 2: External devices

Control Cabinet as Slave
~~~~~~~~~~~~~~~~~~~~~~~~~~

The wiring diagram below shows the control cabinet operating as the slave.

.. figure:: ../../images/07_运输及调试/电气连接/RS485-控制柜作从站.*
    :align: center
    :width: 11cm
    
    Control Cabinet as Slave

1: External device

.. _pro-qep-connector:

QEP Connector
==============

.. _pro-qep-connector-pinout:

QEP Connector Pinout
---------------------

|Pro| has one 16-pin QEP connector for connecting an external encoder in applications such as conveyor tracking. The pin assignments are as follows.

.. list-table:: QEP Connector Pinout
   :widths: 20 20 60
   :header-rows: 1

   * - **Pin**
     - **Name** 
     - **Description**

   * - 1, 15
     - QEP_5V
     - Internal encoder power supply, +5 V; maximum output current: 100 mA
   * - 2, 16
     - QEP_GND
     - Negative terminal of the internal encoder power supply
   * - 3, 5
     - A_P
     - Differential signal 1 positive input/encoder A+
   * - 4, 6
     - A_N
     - Differential signal 1 negative input/encoder A–
   * - 7, 9
     - B_P
     - Differential signal 2 positive input/encoder B+
   * - 8, 10
     - B_N
     - Differential signal 2 negative input/encoder B–
   * - 11, 13
     - Z_P
     - Differential signal 3 positive input/encoder Z+
   * - 12, 14
     - Z_N
     - Differential signal 3 negative input/encoder Z–

For QEP connector wiring, use a harness that meets the specifications below.

.. list-table:: QEP connector harness specifications
   :widths: 25 25 25 25
   :header-rows: 1

   * - **Connector model**
     - **Recommended crimp terminal**
     - **Wire cross-section**
     - **Strip length**
   * - DEGSON, 15EDGKNHC-3.5-16P
     - China: E0512
      
       Overseas: PHOENIX AI1-12RD-Ferrule
     - 0.2–1.5 mm² (24–16 AWG)
     - 8mm (0.31in)

Differential Input
-------------------

Wiring for a differential-input encoder:

.. figure:: ../../images/07_运输及调试/电气连接/差分输入.*
    :align: center
    :width: 13cm
    
    Differential Input

1. Encoder

Single-Ended Input
-------------------

Wiring for a single-ended-input encoder:

.. figure:: ../../images/07_运输及调试/电气连接/单端输入.*
    :align: center
    :width: 13cm
    
    Single-Ended Input

1. Encoder
