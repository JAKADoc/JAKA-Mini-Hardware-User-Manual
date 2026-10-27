The tool input/output interface (TIO) is located on the side of the robot flange. It provides two digital inputs, two digital outputs, and two analog inputs, and two channels can also be used for RS485 signals. See :ref:`Definition of End Effector Side <Definition of End Effector Side>` for the interface definition.

The TIO cable connector features a foolproof design to ensure correct installation. Align the raised part of the TIO connector with the concave groove on the TIO connector of the flange and insert the cable. The TIO position is as shown in the figure below.

.. figure:: ../../images/07_运输及调试/机器人工具I-O.*
   :width: 3cm
   :align: center

   Robot tool I/O

1 TIO

The definition and specifications of the TIO cable are as follows.

.. figure:: ../../images/07_运输及调试/TIO线尺寸图.*
   :width: 18cm
   :align: center

   TIO cable dimensions

| 1 Connect the robot flange
| 2 Connect the end effector

.. _Definition of End Effector Side:

Definition of End Effector Side
-------------------------------

The definition table of the TIO V3.0 interfaces is as follows:

.. list-table:: Specifications of TIO pins
   :widths: 9 19 9 12 51
   :header-rows: 1

   * - **Pin**
     - **Definition**
     - **I/O**
     - **Color**
     - **Description**

   * - 1
     - +24V
     - -
     - Red
     - Positive electrode, 24V/12V (switchable); configurable for enabling or disabling; continuous current capacity 1A; peak output current up to 2A.

   * - 2
     - DI1
     - I
     - Blue
     - Digital input 1: sink or source configurable

   * - 3
     - DI2
     - I
     - Green
     - Digital input 2: sink or source configurable

   * - 4
     - DO1/RS485A_1
     - O
     - Yellow
     - Digital output 1: sink, source, or push-pull configurable by application; current output capability ≤1A

       Multiplexed as RS485-1 communication A+

   * - 5
     - DO2/RS485B_1
     - O
     - Pink
     - Digital output 2: sink, source, or push-pull configurable by application; current output capacity ≤1A

       Multiplexed as RS485-1 communication B-

   * - 6
     - AIN1/RS485A_2
     - I
     - Brown
     - Analog input 1: detection range 0-10V 

       Multiplexed as RS485-2 communication A+

   * - 7
     - AIN2/RS485B_2
     - I
     - White
     - Analog input 2: detection range 0-10V

       Multiplexed as RS485-2 communication B-

   * - 8
     - GND
     - -
     - Gray
     - 24V negative electrode

.. _Wiring of End effector Side:

Wiring of End effector Side
---------------------------

.. _Digital Input:

Digital Input
-------------

The TIO provides two user DI channels compatible with both NPN and PNP signals. Configure the input type in the App; see the |jaka_app| Software User Manual for details.

**Dry contact input**

When the DI input is configured as sink:

The dry contact input (switch-type input) is connected to GND of TIO (gray wire) at one end, and to the digital input (blue or green wire) at the other end.

.. figure:: ../../images/07_运输及调试/NPN型干接点输入接线.*
   :width: 9.67cm
   :align: center

   Sink wiring of digital input

When the DI input is configured as source:

Connect one side of the dry-contact input (switch input) to 24 V on the TIO (red wire) and the other side to the digital input (blue or green wire).

.. figure:: ../../images/07_运输及调试/PNP型干接点输入接线.*
   :width: 9.72cm
   :align: center

   Source wiring of digital input

**Connecting NPN/PNP Devices**

The connection method of sink and source type digital input devices: V+ is connected to 24V of TIO (red wire), 0V is connected to GND of TIO (gray wire), and the signal wire is connected to the digital input of TIO (blue or green wire).

.. figure:: ../../images/07_运输及调试/连接外部NPN设备接线.*
   :width: 9cm
   :align: center

   Wiring of sink device for digital input

| A External sink device
| B TIO V3
| C Main circuit

.. _Digital Outputs:

Digital Outputs
-----------------

When the digital output interface is sink or source output, it adopts open drain output and the maximum continuous current output is 1A. Connection method: the external input interface is connected to the digital output of TIO (yellow or pink wire), V+ side of external device is connected to 24V of TIO (red wire), and 0V side of external device is connected to GND of TIO (gray wire).

.. figure:: ../../images/07_运输及调试/连接外部NPN设备接线_2.*
   :width: 9cm
   :align: center

   Wiring of sink device for digital output

| A External sink device
| B TIO V3
| C Main circuit

.. _RS485:

RS485
-----

Using the RS485 function, the wiring method: external RS485+ is connected to RS485+ of TIO (yellow or brown wire), external RS485- is connected to RS485- of TIO (pink or white wire), the V+ of external device is connected to the 24V of TIO (red wire), and 0V of external device is connected to the GND of TIO (gray wire).

.. figure:: ../../images/07_运输及调试/RS485接线.*
   :width: 9cm
   :align: center

   Wiring of RS485

| A External sink device
| B TIO V3
| C Main circuit

.. _Analog Inputs:

Analog Inputs
---------------

TIO supports 2 analog voltage input interfaces, and the voltage input range is 0-10V. The wiring method: the external analog voltage positive electrode is connected to AIN1/AIN2 of TIO (white and brown wire), and the internal circuit of the negative electrode on the TIO board is grounded. The V+ of external device is connected to the 24V of TIO (red wire), and 0V of external device is connected to the GND of TIO (gray wire).

.. figure:: ../../images/07_运输及调试/模拟输入接线.*
   :width: 9cm
   :align: center

   Wiring of analog input

| A External sink device
| B TIO V3
| C Main circuit