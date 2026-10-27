This chapter describes the electrical specifications and parameters of the control cabinet interfaces and harnesses.

.. warning::

  Operate the robot and control cabinet within the recommended electrical parameters. Exceeding the 
  specified limits may cause permanent damage to the control cabinet hardware.

.. _Electrical-Specifications-of-Power:

Electrical Specifications of Power
==================================

Electrical specifications of control cabinet are as follow.

.. list-table:: Electrical specifications of control cabinet
   :widths: 20 20 20 20 20
   :header-rows: 1

   * - 
     - **Min.**
     - **Typ.**
     - **Max.**
     - **Unit**

   * - Power Input
     - 20
     - 48
     - 60
     - V DC

.. _Electrical-Specifications-of-I-O-Interfaces:

Electrical Specifications of I/O Interfaces
===========================================

The I/O is designed in accordance with IEC 61131-2. It supports 16 channels of digital input and 16 channels of digital output. The electrical specifications for the I/O are shown in the table below:

.. csv-table:: Electrical specifications of I/O interfaces
   :file: ./tables/Electrical specifications of IO interfaces.csv
   :encoding: utf-8-sig
   :widths: 15 27 15 14 14 15
   :header-rows: 1

.. _Typical-Power-Consumption:

Typical Power Consumption
=========================

Typical power consumption of control cabinet:

.. list-table:: Typical power consumption of control cabinet
   :widths: 40 30 30
   :header-rows: 1

   * - **Parameters**
     - **Typ.**
     - **Unit**

   * - Standby Power Consumption
     - 9
     - W

   * - Startup Power Consumption
     - 15
     - W

   * - Robot Power On Consumption
     - 24
     - W

.. _ESD-Sensitive:

ESD Sensitive
================

ESD (electrostatic discharge) is the transfer of electrical static charge between two bodies at different potentials, either through direct contact or through an induced electrical field. When handling parts or their containers, personnel not grounded may potentially transfer high static charges. This discharge may destroy sensitive electronics.

Use one of the following alternatives:

- Use a wrist strap. Wrist straps must be tested frequently to ensure that they are not damaged and are operating correctly.
- Use an ESD protective floor mat. The mat must be grounded through a current-limiting resistor.
- Use a dissipative table mat. The mat should provide a controlled discharge of static voltages and must be grounded.

.. _Line-Fusing:

Line Fusing
=============

There is no integrated fuse inside the control cabinet. Add an external fuse (time-delay) or circuit breaker (class K) according to full load current 
in :ref:`Electrical-Specifications-of-Power`. The following table shows the recommended rating for an external fuse or circuit breaker.

.. list-table:: Fuse specifications
   :widths: 34 33 33
   :header-rows: 1

   * - **Robot**
     - **Current**
     - **Description**

   * - Mini2，Mini2C
     - 125 VDC, 1 phase
     - 10 A

.. _Residual-Current:

Residual Current
=================

An external earth fault protection (residual current device, RCD) is required based on the following residual current data in control cabinet:

.. list-table:: Residual current
   :widths: 50 50
   :header-rows: 1

   * - **Robot**
     - **Residual Current in Control Cabinet**

   * - Mini2，Mini2C
     - ＜30 mA