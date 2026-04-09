
[__SOURCE](README.md)
# Maintenance Manual – Troubleshooting


[__SOURCE](0-about-this-manual/README.md)
# About the Manual

This section describes the troubleshooting methods for each error code that may occur in the HD Hyundai Robotics' Hi6-N and Hi6-T controllers.

The controller is designed with a primary focus on high precision and high-speed performance. In the event of a malfunction, the system is structured to allow easy identification of the cause and rapid recovery. Please ensure that you fully understand this manual and use it effectively for smooth and efficient troubleshooting.


This manual does not cover detailed application functions, such as direct teaching using a collaborative robot, methods of setting safety functions, spot welding, arc welding, positioner sync function, and sensor sync function. For details on relevant information, refer to the collaborative robot maintenance manual and individual application function manuals.

You must fully understand the contents of the manual before using the product. Moreover, keep the manual nearby so that you can refer to it whenever you need it.

This manual may be provided as reference material for customers who have purchased HD Hyundai Robotics products or may be used as internal training material.

This manual has been created based on standard specifications, so some contents may differ depending on the model of the product you have purchased. In addition, the contents and specifications of this manual are subject to change without prior notice to improve the performance of the product, and HD Hyundai Robotics is not responsible for situations that could be caused by inaccuracies or typos in the manual. For detailed information on the revision of the manual, you need to visit our internet website [https://www.hd-hyundairobotics.com/en/main](https://www.hd-hyundairobotics.com/en/main).

[__SOURCE](0-about-this-manual/precautions.md)
# Precautions

{% include url="https://hrcontentsrelay-bmgae5hdbzapc4bc.koreacentral-01.azurewebsites.net/api/proxy?path=doc-common-pages/en/precautions.md" %}

[__SOURCE](0-about-this-manual/notation.md)
## Notation Convention

In this manual, the following notation conventions and safety instructions are used to help you understand the contents.

### Description of Figures

Figures are used to help you understand how to operate the product and illustrate what you can see on the screen. For the description of figures, numbers will be marked for the relevant parts, and the corresponding contents will be described as follows.

![](../_assets/tp630/pane-prog-cmd-param.png)

### GUI \(Graphical User Interface\)

In the GUI, menu names and button names are enclosed in square brackets and displayed with a light background color.
When multiple menus must be selected in sequence, their names are separated by a hyphen (-).

* Single menu: On the initial screen in Manual or Automatic mode, touch the `[F1: Service]`W button.
* Multiple menus: On the initial screen in Manual mode, touch `[F2: System] - 5: Initialization - 6: Mechanism setting`.


### Notation Method for Operation Keys

Keys that are to be pressed on the operation part of the teach pendant to operate functions will be enclosed in square brackets and displayed with a light background color.

* If you press the `[Start]` key, the automatic operation of the program created in the robot will start.



### Cross Reference 

It provides shortcuts to relevant information within the manual. A cross-reference will be shown in double quotation marks (" ") as follows.

* For details on how to change the date and time information, refer to "[4.5 Setting of Date and Time.](../4-service/5-date-time-setting.md)".

### Note

In this section are some helpful tips or additional information that could be useful when you use the product as follows.

{% hint style="info" %}
When the ![](../_assets/eng-mode.png)icon blinks in the status bar, it means that you are in engineer mode.
{% endhint %}

[__SOURCE](0-about-this-manual/safety-notice.md)
# Safety Cautions

Before using the product, you must read the following safety cautions for proper use, user safety, and prevention of property damage.

### Danger

{% hint style="danger" %}
Imminent danger: Incompliance may cause the death of or serious injuries to the operator.
{% endhint %}

* Read the contents of the product installation in the manual and follow the instructions when installing the robot product and other devices.
* If a fatal error occurs in the software, stop using it immediately, and contact our customer support team.
* If there is a problem with the product, such as failure or damage, stop using it immediately and contact the customer support team for inquiry.



### Warning

{% hint style="warning" %}
Potential danger: Incompliance may cause injuries to the operator or damage to property, such as significant damage to the product.
{% endhint %}



* The safety equipment to be used after being connected to the controller must be connected to the safety contact terminal or to the configurable digital I/O set, which is to be set as the safety I/O, in double signals. When the equipment is connected to common contact terminals or in a single signal, the regulated safety level cannot be satisfied.
* Do not put your fingers or other body parts behind the controller's inner bracket. There is a risk of electric shock or injury.
* 
  If you are a robot application system manufacturer or a robot user, you should fully understand the contents of the manual and complete the product operation training.

* For the safety of workers and users, you must prepare appropriate safety facilities, such as safety fences, before installing the product.
* Check the specification information and perform fastening by using appropriate fixing screws. Loosened screws may lead to separation of the robot, causing it to fall or suffer damage.
* Be careful not to let conductive foreign substances, such as liquid, dust, or metal powder, enter the connection sections \(power and cables\). Moreover, do not poke the connection parts with a pointed object or apply excessive force to them when connecting them. Corrosion or temporary short-circuiting of the connection terminals may cause the product to explode or suffer a fire.
* Check the wiring information and connect the devices using the appropriate terminals corresponding to the type of individual devices. In particular, if a safety device is connected to a general terminal, the safety function cannot be guaranteed, so you must connect it to the terminal designed for safety devices.
* Never use a damaged cable and do not disconnect the power while the product is in use. It may cause electric shock, fire, failure, or injury.
* 
  If the product is used for a long time, it may generate heat and cause injury, such as burns. If you need to touch the product, turn off the power and leave it for at least one hour to let it cool sufficiently before carrying out works.

* 
  Use the teach pendant while paying attention to the movement of the robot.

* If the teach pendant warns of a fatal error, stop the robot with the emergency stop switch immediately, identify the cause, and resolve the error. If the error cannot be resolved, please contact our customer support team for an inquiry.
* Never install, modify, disassemble, or repair the product without our permission. It may cause a failure or an accident. In addition, we are not responsible for any damage to or breaking of the product if you do not follow the instructions.



### Caution

{% hint style="warning" %}
Low-level danger factor: Incompliance may result in minor injury to the operator or damage to property, such as damage to the product.
{% endhint %}



* Do not install, modify, disassemble, or repair the product arbitrarily as it is prohibited for anyone other than our experts to arbitrarily modify the product or attach parts. If the product fails because of such acts, our free service and warranty service will be forfeited.
* A qualified installer should install the product in compliance with the related regulations and laws of the concerned country and region. When you want to install and repair the product, contact our customer support team, and ask an expert.
* Do not install and use the product in a dusty or dirty place. Dust or foreign substances may cause failure or abnormal performance of the product.
* Do not install and use the product in a place where magnetism exists or its influence reaches the product or there is electromagnetic interference. Magnetism may damage the product or cause abnormal performance.
* When operating the product, do not wear loose clothing or jewelry, and if the hair is long, take precautions to tie it back so that the hair does not get caught in the joints of the robot.
* Do not enter the operation range or touch the robot while the robot is in operation. Otherwise, there is a risk of injury.
* Prevent the product from being damaged by transporting it in a packaged state and by storing it in a dry place with low humidity. Otherwise, the moisture inside the packaging material may cause the product to get damaged or to fail.
* When it comes to storing the product, avoid places where temperature and humidity may change easily. Store the product in a clean, cool, and dry place.
* When transporting the product, maintain proper posture, and two or more people should work together. Otherwise, you may suffer injury to parts of your body, including waist, arms, and legs.
* If you use lifting equipment to transport the product, follow the safety regulations and equipment usage guidelines in the concerned country and region.
* When transporting the product, fully understand the transportation-related contents of the manual and comply with the instructions. We are not responsible for any damage to or breaking of the product because of transportation by the customer.






[__SOURCE](1-elec/README.md)
# 1. Electrical Components
[__SOURCE](1-elec/VOLTAGE_1.md)
# 1.1. Voltage Check1 - Hi6-N Controller Internal 3-Phase Voltage Check Procedure

(1) Check the 3-phase power voltage inside the controller.

The power supply module(PSM) attached to the front of the controller is responsible for distributing and relaying various power sources. The 3-phase power is turned on and off via a magnetic switch within the power module. With the motor off, check that the voltage input to the power module is within a 10% tolerance of 220 V AC. If the measured voltage is outside the acceptable range, perform the following checks.

![](../_assets/1.전장/전압점검/전압점검1_en.PNG)<br>
Figure 1.1. 3-Phase Power Input to the Power Supply Module(PSM)

{% hint style="warning" %}
Be careful when measuring high voltages as there is a possibility of short circuiting between surrounding components and phases.
{% endhint %}

1) If the voltage on the controller nameplate is AC 220V<br>
If the controller input voltage is AC 220V, the voltage input from the external power switch or terminal block and the voltage measured at the internal control module must be the same. If there is a difference, check the three-phase power wiring.

2) If the voltage on the controller nameplate is not AC 220V<br>
If the controller input power is not AC 220V, the built-in transformer converts the three-phase power to AC 220V and connects it to the control module. Check that the voltage measured at the control module is within a 10% tolerance of AC 220V. If the measured voltage is outside the tolerance range, check the connection between the input and output terminals of the built-in transformer. The primary terminal of the built-in transformer must be connected to the voltage indicated on the controller nameplate.

[__SOURCE](1-elec/VOLTAGE_2.md)
# 1.2. Voltage Check2 – Hi6-N Controller 3-Phase Voltage Check Procedure

(1)	Check the voltage on the nameplate attached to the controller against the actual input voltage.

Check that the voltage actually supplied to the controller is within the allowable range of the voltage printed on the nameplate. The allowable input voltage range is within 10% of the value printed on the nameplate and must be at least AC 198 V for AC 220 V. The figure below illustrates how to measure the controller's input voltage. If the measured voltage is outside the allowable range, inspect the power system.

* Measurement on the power line side of the front switch

![](../_assets/1.전장/전압점검/전압점검2.PNG)<br>
(a) Hi6-N Controller

Figure 1.2. Measurement on the power line side of the power switch

{% hint style="warning" %}
Be careful when measuring high voltages, as there is a risk of short circuits in surrounding components and between phases.
{% endhint %}


[__SOURCE](1-elec/VOLTAGE_3.md)
# 1.3. Voltage Check3 – Hi6-T Controller Input Single-Phase Voltage Check Procedure

(1) Check the voltage on the nameplate attached to the controller against the actual input voltage.<br>
Check that the voltage actually supplied to the controller is within the allowable range of the voltage indicated on the nameplate. The allowable input voltage range is within 10% of the value indicated on the nameplate and must be at least AC 198V for AC 220V. The figure below illustrates how to measure the controller's input voltage. If the measured voltage is outside the allowable range, inspect the power system.

{% hint style="warning" %}
Be careful when measuring high voltages, as there is a risk of short circuits between nearby components and phases.
{% endhint %}

![](../_assets/1.전장/전압점검/전압점검3_en.PNG)<br>
Figure 1.3. H6-T15 Controller Single-Phase Power Input SMPS Terminal Block

[__SOURCE](1-elec/Parts_replacement_tips.md)
# 1.4. Component Replacement Guidelines
This section describes the guidelines for replacing individual components and circuit boards during troubleshooting.

### 1. Module Replacement Guidelines

{% hint style="warning" %}
When replacing a module, the operator should observe the following precautions.
{% endhint %}

① Before starting any work, be sure to turn off the power supply.<br>
② Ensure that the operator’s hands are clean to prevent oil or moisture from contaminating the circuit board. If it is necessary to handle the board, hold it by the edges. Avoid touching electronic components, circuit patterns, and especially connector contact areas.<br>
③ Ensure that the operator’s body(hands) and the controller are at the same electrical potential to prevent electrostatic discharge(ESD).<br>
④ Each circuit board is equipped with multiple connectors. When replacing a board, insert all connectors accurately and securely to prevent incorrect insertion, omission, or loose connections. Ensure that the connector nameplates match the corresponding names printed on the circuit board before insertion.

### 1.1. Main Module Replacement Guidelines

{% hint style="warning" %}
Before removing the main module, be sure to complete the following preparations.
{% endhint %}

① Before replacing the main module, back up all required programs and integer data using the HR-VIEW software on a notebook PC or a USB memory device.<br>
② Taught programs and integer data are stored in the RAM of the main module.
Therefore, when the module is replaced with a new board, the previously used programs and integer data will not be available.<br>
③ After replacement, load the previously backed-up data onto the new board and continue operation.<br>

After observing the above precautions, replace the circuit board by following the procedure described below.

#### 1.1.1. Removal of the Main Module
① First, disconnect the input power supply to the controller.<br>
② Disconnect all connectors connected to the module. For connectors secured with screws, loosen them using an appropriate screwdriver and remove the connectors carefully to avoid applying excessive force.<br>
③ Loosen the upper and lower mounting screws slightly, move the module upward, and then pull it out.<br>

#### 1.1.2. Installation of the Main Module
① First, verify that the controller input power is turned OFF.<br>
② Hang the replacement module onto the upper and lower mounting screws, then secure it by tightening the mounting screws.<br>
③ Reconnect all connectors to the module.
For connectors secured with screws, use an appropriate screwdriver and tighten them carefully to avoid stressing the connectors.<br>
④ Double-check that the communication cables are connected correctly and that no steps have been missed.<br>

### 1.2. Drive Module Replacement Guidelines

{% hint style="warning" %}
When replacing the servo drive module, the operator must observe the following precautions.
{% endhint %}

Since compatibility may not be guaranteed with servo drive modules of different models, be sure to verify the nameplate on the front panel before replacement.

#### 1.2.1. Removal of the Servo Drive Unit
① First, turn off the input power supply.<br>
② Loosen the fixing bolts of the protective cover on the servo drive unit and remove the cover.<br>
③ Disconnect the wiring secured to the terminal block by screws.<br>
④ Disconnect all connected connectors.<br>
⑤ Remove the screws securing the servo drive unit.<br>
⑥ Remove the servo drive unit. The servo drive unit is heavy; use caution to avoid injury when removing it. Also, take care not to damage the adjacent wiring.<br>

#### 1.2.2. Installation of the Servo Drive Unit
① First, ensure that the input power supply is turned OFF.<br>
② Carefully lift and slide the servo drive unit into position. The servo drive unit is heavy; use caution to avoid injury while installing it. Also, take care not to damage adjacent wiring.<br>
③ Secure the servo drive unit with screws.<br>
④ Tighten the wiring to the terminal block using screws.<br>
⑤ Connect all connectors.<br>
⑥ Fasten the protective cover of the servo drive unit with bolts.<br>
⑦ Double-check that no steps have been missed.<br>

### 1.3. PSM(Power Supply Module) Replacement Guidelines 
{% hint style="warning" %}
The PSM is a composite power supply unit used as the main control power source.
As it is a precision device, special care must be taken during handling.
{% endhint %}

#### 1.3.1. Removal of the PSM(Power Supply Module)
① First, turn off the input power supply.<br>
② Disconnect all connectors connected to the module.<br>
③ Loosen the upper and lower mounting screws slightly, move the module upward, and then pull it out. The PSM is heavy; use caution to avoid injury when removing it. Also, take care not to damage adjacent wiring. Do not pull the module out suddenly or with excessive force, as this may result in injury.<br>

#### 1.3.2. Installation of the PSM(Power Supply Module)
① First, verify that the controller input power is turned OFF.<br>
② Hang the replacement module onto the upper and lower mounting screws, then secure it by tightening the mounting screws. The PSM is heavy; use caution to avoid injury during installation. Also, take care not to damage adjacent wiring.
Do not insert the module suddenly or with excessive force, as this may result in injury.<br>
③ Reconnect all connectors to the module. For connectors secured with screws, use an appropriate screwdriver and tighten them carefully to avoid stressing the connectors.<br>
④ Double-check that all connectors are connected correctly and that no steps have been missed.<br>

[__SOURCE](1-elec/Adjustment_tips.md)
# 1.5. Adjustment Guidelines

This controller is fully adjusted at the factory prior to shipment and normally requires no additional adjustment. However, if components are replaced, certain adjustments may be required. This section explains the locations and procedures for those adjustments. Do not perform any adjustments unless absolutely necessary. Even if a problem occurs, do not make any adjustments unless the cause has been clearly identified, as improper adjustment may result in malfunction or damage.

### 1. Adjustment of Power System 
If a fault occurs in the power system, or if the power supply configuration has been changed, measure each power supply voltage and adjust any values that deviate from the specified reference levels(Measurements must be taken using a digital voltmeter).

### 1.1. Adjustment of the Hi6-N Controller Power System
![](../_assets/1.전장/조정요령/Hi6-N제어기%20전원%20기준치_en.PNG)<br>
Figure 1. Reference Power Supply Voltage Levels of the Hi6-N Controller

(Note 1) If the measured value is outside the specified reference range, replace the PSM.<br>
(Note 2) First, verify the reference value at the specified measurement point.
Then, if possible, measure the voltage between the pins of the terminal block or connector closest to the robot encoder. At this point, the reference value must be DC 5.1V ± 0.1V.

### 1.2. Adjustment of the Hi6-T Controller Power System

![](../_assets/1.전장/조정요령/Hi6-T제어기%20전원%20기준치_en.PNG)<br>
Figure 2. Reference Power Supply Voltage Levels of the Hi6-T Controller

(Note 1) If the measured value is outside the specified reference range, replace the PSM.
(Note 2) First, verify the reference value at the specified measurement point.
Then, if possible, measure the voltage between the pins of the terminal block or connector closest to the robot encoder. At this point, the reference value must be DC 5.1V ± 0.1V.

### 2. Transformer(TR2)
{% hint style="warning" %}
For the Hi6-N controller, the output voltage of the transformer(TR2) must be AC 220V. The secondary-side terminals are connected according to the power specifications of the internal components; do not touch or modify them under any circumstances.
{% endhint %}

The input power supply for this controller must be AC 220V, 3-phases. Controllers with other voltage specifications are factory-adjusted prior to shipment; therefore, the transformer taps must not be changed without authorization from the manufacturer’s service personnel.


[__SOURCE](2-servo-control-board-part/README.md)
# 2. Servo AMP Board
[__SOURCE](2-servo-control-board-part/E02500.md)
# 2.1. E02500 AMP Regenerative Discharge Resistor Overheat

### 1. Overview

This error relates to the overheating of the regenerative resistor, which dissipates the regenerative power generated during robot deceleration or descent in the direction of gravity. It can occur when the regenerative discharge capacity is exceeded due to degraded cooling fan performance, sudden rapid movements, or continuous robot operation.

### 2. Causes

{% hint style="info" %}

The temperature of the regenerative discharge resistor has risen above the threshold. This is caused by excessive robot playback speed or an issue with the cooling system.

* <Cases occurring at a specific step depending on the robot's playback speed>

(1) Please check for errors by adjusting the robot's playback speed.

(2) Please inspect the resistance value of the regenerative discharge resistor.

* <Cases occurring more than 5 minutes after the robot has started>

(3)	Please inspect the controller's cooling system and the amount of regenerative power.

-> Check the operating status of each fan.

-> Check the power supply voltage of the fans.

(4)	Please inspect the amount of regenerative power generated by the robot.

-> Check for errors by lowering the robot's playback speed.

{% endhint %}

(1) Please check for errors by adjusting the robot's playback speed.

During robot deceleration or descent in the direction of gravity, the DC voltage of the servo drive increases. To prevent component damage caused by this voltage spike, power is dissipated through the regenerative discharge resistor. Errors can occur if the robot undergoes sudden deceleration or moves at high speeds in the direction of gravity. Please verify whether the error persists when the robot's playback speed is modified.

* Adjusting the Robot Playback Speed

A regenerative resistor overheat error may occur if the regenerative power generated by the robot's movement exceeds the controller's design specifications. Please operate the robot after lowering the speed of the specific step where the error occurs and check if the error is resolved.


(2)	Please inspect the resistance value of the regenerative discharge resistor.

* Checking the Regenerative Discharge Resistance Value

If the resistance value measured at the end of the CNDR cable deviates by more than 10% from the value specified in the manual, the resistor is defective. Please replace the resistor. Refer to the previous page for the detailed measurement procedure.

 (2)-1. Hi6-N Controller

-> Medium-sized (H6D6X) Regenerative Discharge Resistance: 5Ω (N00)

-> Large-sized (H6D6X) Regenerative Discharge Resistance: 4Ω (N80)

-> Small-sized (H6D6A) Regenerative Discharge Resistance: 15Ω (N30)

(2)-2. Hi6-T Controller

-> Regenerative Discharge Resistance: 20Ω

(3)	Please inspect the controller's cooling conditions and the amount of regenerative power.

If the regenerative resistor overheat error occurs more than 5 minutes after the robot starts, it indicates either a malfunction in the controller's cooling system or that the robot's playback speed exceeds the controller's design specifications. Fans are installed at the rear of the controller to cool the heat sinks of the servo drive units and the regenerative discharge resistors.

![](../_assets/2.서보AMP/E02500/E02500_제어기_후면_팬.PNG  )

Table 1-1 Hi6 Controller Fan Installation Locations

* Checking the Operating Status of Each Fan

If a fan does not rotate or its speed is abnormally low, please replace the corresponding fan. The lifespan of a fan varies depending on the operating environment and total runtime.


* Checking the Fan Power Supply Voltage

If none of the fans are operating, please check the input voltage to the fans. The fan input voltage is set to AC 220V, with an allowable tolerance within ±10% of the rated voltage. If the voltage is more than 10% lower than the rated value, the cooling efficiency will decrease due to the reduced fan speed. If the voltage is low, please check the fan power connector (CNFN2) and the main input voltage of the controller.

(4)	Please inspect the amount of regenerative power generated by the robot.

* Check for errors based on the robot's playback speed.

If an overheat error occurs during continuous playback for more than 5 minutes, it is because the robot's repetitive movements have exceeded the controller's cooling capacity. Please verify if the error persists after lowering the robot's playback speed. If lowering the speed resolves the regenerative resistor overheat error but prevents you from achieving the required cycle time (operating speed), please contact our technical support department.
[__SOURCE](2-servo-control-board-part/E02501.md)
# 2.2. E02501 AMP Regenerative Discharge Resistor Open Circuit, Resistor, or Circuit Error

### 1. Overview

This error relates to the regenerative resistor, which dissipates the power generated during robot deceleration or descent in the direction of gravity. It can be caused by a failure in the overheat detection sensor circuit, an open circuit in the resistor, or an excessive 3-phase power supply voltage.

### 2. Causes and Inspection Methods

{% hint style="info" %}
Overheat errors also occur in the event of an open circuit in the resistor or an abnormality in the discharge control. Additionally, they can be caused by deviations in the regenerative discharge resistance value or an increase in the 3-phase power supply voltage.

* <Cases occurring immediately upon Motor ON>

(1)	Please inspect the resistance value of the regenerative discharge resistor.

-> Check the resistance value at the CNDR cable.

(2)	Please inspect the servo drive unit.

-> Check the system after replacing the servo drive unit.

(3)	Please inspect power-related components.

-> Check the internal 3-phase voltage of the controller.

-> Check the input 3-phase voltage of the controller.

{% endhint %}

(1)	Please inspect the resistance value of the regenerative discharge resistor.

An overheat error can also occur due to an open circuit in the resistor or an increase in the regenerative discharge resistance value.
 
* Checking for an Open Circuit in the Regenerative Resistor

f the resistance value measured at the end of the CNDR cable is in the mega-ohm (MΩ) range, it indicates an open circuit in the resistor or a poor internal wiring connection. Please replace the regenerative resistor with a known functional unit or repair the wiring.

![](../_assets/2.서보AMP/E02501/E02501_회생저항_단선점검_N제어기.PNG)

(a) Hi6-N Controller (BD651/BD653 Board)

![](../_assets/2.서보AMP/E02501/E02501_회생저항_단선점검_T제어기.PNG  )

(b) Hi6-T Controller (BD667T Board)

Figure 1.1 Measuring the Resistance Value at CNDR

(2)	Please inspect power-related components.

Overheat errors can also occur in the event of an abnormality in the discharge control circuit.

* Drive Unit Replacement and Inspection

Please replace the module that detects regenerative discharge resistor overheating and check if the error recurs. A circuit failure within the module can cause the error to persist.

(2)-1. Hi6-N Controller

-> Servo Drive Unit for Medium-sized Robots: H6D6X

-> Servo Drive Unit for Small-sized Robots: H6D6A

(2)-2 Hi6-T Controller

-> BD667T


(3)	Please inspect power-related components.

Overheat errors can occur due to an open circuit in the resistor or an abnormality in the discharge control. Additionally, they may be caused by deviations in the regenerative discharge resistance value or an increase in the 3-phase power supply voltage.

* Checking the Internal 3-Phase Voltage of the Controller

 Regenerative discharge operation begins at approximately DC 375V. If a voltage of AC 242V or higher is input to the servo drive unit, a regenerative discharge resistor overheat error may occur the moment the motor is turned ON. If the input voltage exceeds the allowable range, please perform an inspection following the "Controller Input Voltage Inspection Procedure" and the "Controller Internal 3-Phase Voltage Inspection Procedure."

-> Servo Drive Unit Input Voltage Specification: 3-Phase AC 220V

-> Allowable Range during Motor ON: 198V ~ 242V

[__SOURCE](2-servo-control-board-part/E02502.md)
# 2.3. E02501 AMP Regenerative Discharge Resistor Detection Circuit Error

### 1. Overview

This error relates to the overheating of the regenerative resistor, which dissipates the regenerative power generated during robot deceleration or descent in the direction of gravity. It can be caused by a failure in the overheat detection sensor circuit or cable-related issues.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An abnormality has occurred in the path used to detect overheat errors, or the resistance value has changed.

* <Cases occurring even when the Motor is OFF>

(1)	Please inspect the cables related to overheat error detection. 

-> Check the resistance of the CNTR cable.

(2) Please inspect the components related to overheat error detection. 

-> Hi6-N Controller: Check after replacing the BD640 board. 

-> Hi6-T Controller: Check after replacing the BD641 board. 

-> Check after replacing the servo drive unit.

{% endhint %}

(1) Please inspect the overheat error detection cable.

The regenerative resistor overheat error is detected by the servo drive unit by monitoring the ON/OFF state of the thermal sensors attached to both ends of the regenerative resistor via the CNTR connector. In the Hi6-N controller, errors detected by the BD651/BD653 boards are transmitted through the BD652/BD654 and finally processed as software alerts by the BD640 board.

![](../_assets/2.서보AMP/E02502/E02502_회생저항_과열검지케이블_N제어기.PNG  )

(a) Hi6-N Controller

Errors detected in the Hi6-T controller are transmitted from the BD667T board through the BD602T and are processed by software on the BD641T board.

![](../_assets/2.서보AMP/E02502/E02502_회생저항_과열검지케이블_T제어기.PNG  )

(b) Hi6-T15 Controller

Figure 1.1 Component Layout for Regenerative Resistor Overheat Errors

* CNTR Cable Inspection 

Please check the condition of the sensor at the CNTR connector, which connects to the overheat detection sensor. Under normal conditions, the sensor resistance should measure less than 0.1Ω.

![](../_assets/2.서보AMP/E02502/E02502_회생저항센서_단선측정_N제어기.PNG  )

(a) Hi6-N Controller

![](../_assets/2.서보AMP/E02502/E02502_회생저항센서_단선측정_T제어기.PNG  )

(b) Hi6-T15 Controller

Figure 1.2 Measuring the Resistance Value at CNTR

(2) Please inspect the components related to overheat error detection.

* Servo Control Board Replacement and Inspection
 
 If the error is resolved after replacing the servo control board with a known functional unit, the original board is defective. Please replace it with a functional board to resume operation.

-> Hi6-N Controller: BD640

-> Hi6-T Controller: BD641T


* Servo Drive Unit Replacement and Inspection

The modules responsible for detecting regenerative discharge resistor overheat errors are as follows:

-> Hi6-N Controller: H6D6X (Medium-sized) or H6D6A (Small-sized) (excluding the servo board).

-> Hi6-T Controller: BD667T

Please identify the components of the controller currently in use before proceeding with the inspection. Verify whether the error recurs after replacing the suspected part with a known functional unit.

[__SOURCE](2-servo-control-board-part/E02503.md)
# 2.4. E02503 AMP PN Overvoltage Occurred

### 1. Overview

The DC voltage (P-N) of the servo drive unit that powers the motor has exceeded the predefined threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error may occur during sudden changes in the robot's movement. It can also be caused by an increase in the regenerative discharge resistance value.

* <Cases occurring at a specific step depending on the robot's playback speed>

(1) Please check for errors by adjusting the robot's playback speed.

(2) Please inspect the resistance value of the regenerative discharge resistor.

{% endhint %}

(1) Please check for errors according to the robot's playback speed.

Excessive voltage errors can occur when the robot decelerates abruptly or descends rapidly in the direction of gravity. Please verify whether the error persists depending on the robot's playback speed. Additionally, AMP overvoltage errors may be caused by a defective regenerative discharge resistance value or a malfunction in the regenerative discharge control system.

* Changing the Robot Playback Speed

An overvoltage error may occur if the regenerative power generated by the robot's movement exceeds the controller's design specifications. Please reduce the speed of the step where the error occurs and check if the issue persists. If the error does not occur at a lower speed, please adjust and use the modified step speed.

(2) Please check for errors according to the robot's playback speed.

* Inspection of Regenerative Discharge Resistance Value

If the regenerative resistance value is higher than the specified value, regenerative discharge may not function properly, leading to overvoltage errors. The specifications for regenerative resistance may vary depending on the controller's model and specifications. Please refer to the manual and the controller check sheet provided at the time of purchase. If the measured resistance value deviates by more than 10% from the specifications, the component must be replaced.

(2)-1. Hi6-N Controller - Regenerative Discharge Resistance Value

-> Mid-sized models (Hi6-N00, H6D6X): 5 ohm (N00)
-> Large-sized models (Hi6-N80, H6D6X): 4 ohm (N80)
-> Small-sized models (Hi6-N30, H6D6A): 15 ohm (N30)

(2)-2. Hi6-T Controller - Regenerative Discharge Resistance Value
-> 20ohm

![](../_assets/2.서보AMP/E02503/E02503_회생저항_단선점검_N제어기.PNG  )

(a) Hi6-N Controller

![](../_assets/2.서보AMP/E02503/E02503_회생저항_단선점검_T제어기.PNG  )

(b) Hi6-T Controller

Figure 1.1 Measuring the resistance value at CNDR
[__SOURCE](2-servo-control-board-part/E02504.md)
# 2.5. E02504 AMP Diode Module Error or AC Input Voltage Exceeded

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motor has exceeded the set threshold of DC 395V.

### 2. Causes and Inspection Methods

{% hint style="info" %}

An error in the diode module has caused the PN voltage to fall outside the allowable range. This error can also occur if the 3-phase voltage input to the servo drive module (AMP) is abnormally high.

* <If the error consistently occurs at the moment the motor is turned ON>

(1)	Inspect components related to the power supply.

-> Replace the servo drive unit and check if the error persists.

(2) Inspect the power supply voltage.

-> Check the 3-phase voltage inside the controller.

-> Check the 3-phase input voltage supplied to the controller.

{% endhint %}

(1) Please inspect components related to the power supply.

* Replacement Inspection of the Servo Drive Unit

Please replace the module that detects the AMP overvoltage error and verify if the error recurs. Continuous errors may occur due to a failure in the module's internal circuitry.

(1)-1. Hi6-N Controller

-> Servo drive unit for mid-sized robots: H6D6X

-> Servo drive unit for small-sized robots: H6D6A

(1)-2. Hi6-T Controller

-> Servo drive unit for small-sized robots: BD667T

(2) Please inspect the power supply voltage.

* Hi6-N Controller: 3-Phase Voltage Inspection 

If a voltage of AC 242V or higher is input to the servo drive unit, an overvoltage error may occur the moment the motor is turned ON. If the input voltage exceeds the allowable range, please inspect the voltage according to the "Controller Input Voltage Inspection Procedure" and the "Internal 3-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: 3-Phase AC 220V

-> Allowable Range (Motor ON): 198V ~ 242V

* Hi6-T Controller: Single-Phase Voltage Inspection 

If a voltage of AC 242V or higher is input to the servo drive unit, an overvoltage error may occur the moment the motor is turned ON. If the input voltage exceeds the allowable range, please inspect the voltage according to the "Controller Input Voltage Inspection Procedure" and the "Internal Single-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: Single-Phase AC 220V

-> Allowable Range (Motor ON): 198V ~ 242V


[__SOURCE](2-servo-control-board-part/E02505.md)
# 2.6. E02505 AMP PN Overvoltage Detection Path Error or Discharge Error

Previous Error Code: E0011 AMP Overvoltage (P-N) Occurred

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motor has exceeded the set threshold.

### 2. Causes and Inspection Methods

{% hint style="info" %}

A failure has occurred in the path detecting the PN voltage drop from the diode module or within the PN discharge circuit.

* <If the error consistently occurs even when the motor is OFF>

(1)	Hi6-N Controller

-> Replace the BD640 board and check if the error persists.

-> Replace the servo drive unit and check if the error persists.

(2)	Hi6-T Controller

-> Replace the BD641T board and check if the error persists.

-> Replace the BD602T board and check if the error persists.

-> Replace the BD667T board and check if the error persists.

{% endhint %}

(1)	Hi6-N Controller

An overvoltage error in the Hi6-N controller AMP is detected by the servo drive unit when the DC power (P-N) supplied to the unit exceeds the preset level. The detected error is then processed by the BD640 board via the AMP boards (BD651/BD652/BD653/BD654).

-> BD640 Replacement Inspection

Replace the BD640 with a known functional board. If the error does not recur, the original board is defective. Please replace it with a new BD640 board for continued use.

-> Servo Drive Unit Replacement Inspection

The modules responsible for detecting AMP overvoltage errors are as follows:

* Hi6-N Controller: Mid-sized H6D6X, Small-sized H6D6A (Excluding servo boards)

Please check the components of the controller currently in use before proceeding with the inspection. Replace the suspected part with a known functional unit to verify whether the error recurs.

![](../_assets/2.서보AMP/E02505/E02505_과전압_부품교체_N제어기_en.PNG)

Figure 1.1 Component Layout for Overvoltage Errors in Hi6-N Controllers

<br>

(2)	Hi6-T Controller

An overvoltage error in the Hi6-T controller AMP is detected by the servo drive unit when the DC power (P-N) supplied to the unit exceeds the preset level. The detected error is transmitted from the BD667T through the BD602T board and is then processed by the BD641T board.

-> BD641T Replacement Inspection

Replace the BD641T with a known functional board. If the error does not recur, the original board is defective. Please replace it with a new BD641T board.

-> BD602T Replacement Inspection

Replace the BD602T with a known functional board. If the error does not recur, the original board is defective. Please replace it with a new BD602T board.

-> BD667T Replacement Inspection

Replace the BD667T with a known functional board. If the error does not recur, the original board is defective. Please replace it with a new BD667T board.

Please check the components of the controller currently in use before proceeding with the inspection. Replace the suspected part with a known functional unit to verify whether the error recurs.

![](../_assets/2.서보AMP/E02505/E02505_과전압_부품교체_T제어기.PNG)

Figure 1.2 Component Layout for Overvoltage Errors in Hi6-T Controllers
[__SOURCE](2-servo-control-board-part/E02506.md)
# E02506 AMP PN Under-voltage Occurred

### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motor has been measured at or below the under-voltage setpoint.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This error may occur at specific steps depending on the robot's playback speed, caused by a drop in PN voltage due to high energy consumption. It can also be caused by an unstable 3-phase power supply to the controller.

* <If the error occurs at specific steps depending on the robot's playback speed>

(1)	Check for errors by changing the robot's playback speed.

(2) Inspect the controller power supply voltage.

-> Inspect the 3-phase or single-phase input voltage of the controller while the robot is in operation.

-> If the input voltage is not 220V, inspect the internal 3-phase or single-phase voltage.

{% endhint %}

(1) Please check for errors by changing the robot's playback speed.

An AMP under-voltage error occurs when the input power capacity is insufficient or when the robot undergoes rapid acceleration. Please verify whether the error persists depending on the robot's playback speed and monitor any fluctuations in the 3-phase voltage input to the servo drive unit.

* Changing the Robot Playback Speed

An under-voltage error may occur if the instantaneous power demand from the robot's movement exceeds the controller's design specifications. Please reduce the speed of the step where the error occurs and check if the issue persists. If the error does not occur at a lower speed, please adjust and use the modified step speed.


(2) Please inspect the controller power supply voltage.

* Hi6-N Controller: 3-Phase Voltage Inspection at the Error Step 

An AMP under-voltage error is triggered at approximately DC 142V (or 210V). The error may occur if the 3-phase voltage input to the servo drive unit drops to AC 100V (or 148V) or below during the step where the error is generated. If the input voltage falls outside the allowable range, please inspect the voltage according to the "Controller 3-Phase Input Voltage Inspection Procedure" and the "Internal 3-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: 3-Phase AC 220V

-> Allowable Range (Motor ON): AC 198V – 242V


* Hi6-T Controller: Single-Phase Voltage Inspection at the Error Step 

An AMP under-voltage error is triggered at approximately DC 142V (or 210V). The error may occur if the single-phase voltage input to the servo drive unit drops to AC 100V (or 148V) or below during the step where the error is generated. If the input voltage falls outside the allowable range, please inspect the voltage according to the "Controller Single-Phase Input Voltage Inspection Procedure" and the "Internal Single-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: Single-Phase AC 220V

-> Allowable Range (Motor ON): AC 198V ~ 242V

[__SOURCE](2-servo-control-board-part/E02507.md)
# 2.8. E02507 AMP Diode Module Error or AC Input Voltage Insufficient


Previous Error Code: E0033 AMP PN Under-voltage Occurred


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motor has been measured at or below the under-voltage setpoint.

### 2. Causes and Inspection Methods

{% hint style="info" %}

The PN voltage failed to charge due to an error in the diode module. This error can also be caused by a drop in the AC voltage input to the servo drive unit.

* <If the error occurs at the moment the motor is turned ON>

  * Hi6-N Controller

     (1) Inspect components related to the power supply.

     -> Replace the servo drive unit and check if the issue persists.

     (2) Inspect the controller power supply voltage.

     -> Check the internal 3-phase voltage of the controller.

     -> Check the 3-phase input voltage supplied to the controller.

  * Hi6-T Controller

     (3)	Inspect components related to the power supply.
     
     -> Replace the BD667T and check if the error persists.

     (4)	Inspect the controller power supply voltage.

     ->	Check the internal single-phase voltage of the controller.

     ->	Check the single-phase input voltage supplied to the controller.

{% endhint %}


* Hi6-N Controller

(1)	Please inspect components related to the power supply.

An AMP under-voltage error occurs when the 3-phase AC 220V power input to the servo drive unit falls outside the allowable range. It can also occur if regenerative discharge is triggered when the motor is turned ON due to a malfunction in the regenerative discharge control circuit.

** Replacement Inspection of the Servo Drive Unit

Please replace the module that detects the AMP overvoltage error and verify if the error recurs. Continuous errors may occur due to a failure in the module's internal circuitry.

The modules responsible for detecting AMP under-voltage errors are as follows:

-> Mid-sized models: H6D6X

-> Small-sized models: H6D6A


(2)	Please inspect the controller power supply voltage.

** 3-Phase Voltage Inspection

An AMP under-voltage error is triggered at approximately DC 142V. The error may occur if the motor is turned ON while the voltage input to the servo drive unit is AC 100V or below. If the input voltage falls outside the allowable range, please inspect the voltage according to the "Controller 3-Phase Input Voltage Inspection Procedure" and the "Internal 3-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: 3-Phase AC 220V

-> Allowable Range (Motor ON): AC 198V ~ 242V


* Hi6-T Controller

(3)	Please inspect components related to the power supply.

An AMP under-voltage error occurs when the single-phase AC 220V power input to the servo drive unit falls outside the allowable range. It can also occur if regenerative discharge is triggered when the motor is turned ON due to a malfunction in the regenerative discharge control circuit.

**	Replacement Inspection of the Servo Drive Unit

Please replace the module that detects the AMP overvoltage error and verify if the error recurs. Continuous errors may occur due to a failure in the module's internal circuitry.

The module responsible for detecting AMP under-voltage errors is as follows:

->	BD667T Board


(4)	Please inspect the controller power supply voltage.

**	Single-Phase Voltage Inspection

An AMP under-voltage error is triggered at approximately DC 142V. The error may occur if the motor is turned ON while the voltage input to the servo drive unit is AC 100V or below. If the input voltage falls outside the allowable range, please inspect the voltage according to the "Controller Single-Phase Input Voltage Inspection Procedure" and the "Internal Single-Phase Voltage Inspection Procedure."

-> Servo Drive Input Voltage Specification: Single-Phase AC 220V

-> Allowable Range (Motor ON): AC 198V ~ 242V




[__SOURCE](2-servo-control-board-part/E02508.md)
# 2.9. E02508 AMP PN Under-voltage Detection Path Error or Discharge Error


Previous Error Code: E0033 AMP PN Under-voltage Occurred


### 1. Overview

The DC link voltage (P-N) of the servo drive unit that powers the motor has been measured at or below the under-voltage setpoint.

### 2. Causes and Inspection Methods

{% hint style="info" %}

A failure has occurred in the path detecting the PN voltage drop from the diode module or within the PN discharge circuit.

* <If the error occurs even when the motor is OFF>

  * Hi6-N Controller

     (1)	Inspect components related to under-voltage error detection.
     
     -> Replace the BD640 board and check if the error persists.

     -> Replace the servo drive unit and check if the error persists.

    
  * Hi6-T Controller

     (2)	Inspect components related to under-voltage error detection.
     
     -> Replace the BD641T board and check if the error persists.

     -> Replace the BD602T board and check if the error persists.	

     -> Replace the BD667T and check if the error persists.

{% endhint %}

(1)	Please inspect components related to under-voltage error detection.

* BD640 Replacement Inspection

   Replace the BD640 with a known functional board. If the error does not recur, the original board is defective.

* Servo Drive Unit Replacement Inspection

   The modules responsible for detecting AMP under-voltage errors are as follows:

  -> Hi6-N Controller: Mid-sized H6D6X, Small-sized H6D6A (Excluding servo boards)

  Please check the components of the controller currently in use before proceeding with the inspection. Replace the suspected part with a known functional unit to verify whether the error recurs.


![](../_assets/2.서보AMP/E02508/E02508_과전압_부품교체_N제어기_en.PNG  )

Figure 1.1 Replacement of BD640 and Servo Drive Unit

<br>


(2)	Please inspect components related to under-voltage error detection.

*  BD641T Replacement Inspection

   Replace the BD641T with a known functional board. If the error does not recur, the original board is defective.


*  BD602T Replacement Inspection

   Replace the BD602T with a known functional board. If the error does not recur, the original board is defective.


*  BD667T Replacement Inspection

   Replace the BD667T, which is the module responsible for detecting AMP under-voltage errors, with a known functional board. If the error does not recur, the original board is defective.

   Please check the components of the controller currently in use before proceeding with the inspection. Replace the suspected part with a known functional unit to verify whether the error recurs.



![](../_assets/2.서보AMP/E02508/E02508_과전압_부품교체_T제어기.PNG)

Figure 1.1 Replacement of BD641T, BD602T, and BD667T

[__SOURCE](2-servo-control-board-part/E02520.md)
# 2.10. E02520 (Axis ○) IPM Fault

### 1. Overview

A fault output has been generated from the IPM (Intelligent Power Module), which is the switching element within the servo drive unit that powers the motor. An IPM fault can be caused by an increase in the heatsink temperature, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Methods

{% hint style="info" %}

* <If the error occurs at the moment the motor is turned ON or occurs intermittently>

(1)	Please inspect the components used for motor drive.

->	Check the output cables connected to the servo drive unit.

->	Inspect the terminals of the switching elements (IPM) within the servo drive unit.

->	Replace the servo board and verify if the error persists.

*	Hi6-N Controller: BD640

*	Hi6-T Controller: BD641T

->	Replace the servo drive unit and verify if the error persists.

*	Hi6-N Controller: Mid-sized H6D6X, Small-sized H6D6A (Excluding servo boards)

*	Hi6-T Controller: BD657T, BD658T

->	Replace the servo motor and verify if the error persists.


<If the error occurs after the robot has been operating for 5 minutes or longer>

(2)	Please inspect the cooling fans of the controller.

->	Check the operational status of each fan.

->	Inspect the power supply voltage provided to the fans.

{% endhint %}

(1)	Please inspect the components used for motor drive.

The servo drive unit, which powers the motor, receives commands from the servo board (BD640) via a board-to-board direct connector. The current output from the internal amplification circuit is then transmitted to the motor through the wiring connected to each axis's connector.

->	Inspection of the output cables connected to the servo drive unit

Inspect the condition of the wiring connecting the servo drive unit to the motor. During inspection, ensure the controller power is OFF, disconnect the connector from the servo drive unit, and measure the resistance between each phase and the ground on the cable side to check for short circuits.



![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_서보구동장치케이블점검_N제어기_en.PNG)

(a) Hi6-N Controller

![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_서보구동장치케이블점검_T제어기.PNG)

(b) Hi6-T Controller

Figure 1.1 Inspection of Servo Drive Unit Output Cables

<br>


->	Inspection of Switching Elements in the Servo Drive Unit

The switching elements of the servo drive unit output AC current for each phase by switching the DC voltage supplied from the diode module. If a short circuit occurs at the internal terminals of the switching element, overcurrent flows, triggering an IPM fault error. With the connectors disconnected, check for a short circuit between the output terminals (U, V, or W) of the servo drive unit and P or N. If a short circuit is confirmed, the servo drive unit must be replaced, and the cables connecting the servo drive unit to the motor must also be inspected.

*	Hi6-N Controller

    -	Servo drive unit for mid-sized robots: H6D6X (Excluding servo boards)

    -	Servo drive unit for small-sized robots: H6D6A (Excluding servo boards)


*	Hi6-T Controller

    -	Main-axis Servo Drive Unit: BD658T

    -	Sub-axis Servo Drive Unit: BD657T

![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_서보구동장치스위칭소자점검_N제어기.PNG)

(a) Hi6-N Controller (H6D6X / H6D6A)

![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_서보구동장치스위칭소자점검_T제어기.PNG)

(b) Hi6-T Controller (BD658T / BD657T)

Figure 1.2 Switching Element Short-Circuit Inspection

<br>

->	Servo Board Replacement Inspection

If the error does not recur after replacing the servo board, the original board is defective. Please replace the servo board with a known functional unit.

*	Hi6-N Controller: BD640

*	Hi6-T Controller: BD641T


->	Servo Drive Unit Replacement Inspection

If the error does not recur after replacing the servo drive unit, the original unit is defective. Please replace the servo drive unit with a known functional unit.

*	Hi6-N Controller

    -	Servo drive unit for mid-sized robots: H6D6X (Excluding servo boards)

    -	Servo drive unit for small-sized robots: H6D6A (Excluding servo boards)

*	Hi6-T Controller

    -	Main-axis servo drive unit: BD658T

    -	Sub-axis servo drive unit: BD657T


->	Servo Motor Replacement Inspection

f the error does not recur after replacing the servo motor, the original motor is defective. Please replace the servo motor with a known functional unit. The figure below illustrates the location of each axis motor for the robot. For other robot models, please refer to the corresponding mechanical maintenance manual for replacement instructions.

![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_HS165로봇.PNG)

Figure 1.3 Motor Locations for Each Axis of the Robot

<br>

(2)	Please inspect the controller's cooling fans.

f an IPM fault error occurs after the robot has been operating for 5 minutes or longer, it indicates that the controller's cooling system is malfunctioning, causing the IPM to exceed its allowable operating temperature specification. Fans are installed at the rear of the controller to cool the servo drive unit's heatsink and the regenerative discharge resistor.

<br>


Table 1-1 Installation Locations of Hi6 Controller Fans

![](../_assets/2.서보AMP/E02520/E02520_제어기_후면_팬.PNG)


->	Inspection of Fan Operational Status

If a fan is not rotating or its speed is abnormally low, please replace the corresponding fan. The lifespan of a fan varies depending on the operating environment and usage hours.


->	Inspection of Fan Power Supply Voltage

If all fans are inoperative, please verify the fan input voltage. The fan input voltage is set to AC 220V, with an allowable range within 10% of the rated voltage. If the voltage is more than 10% below the rating, the cooling efficiency will decrease due to the reduced fan rotation speed. If the voltage is low, please inspect the power connectors for the rear cooling fans and the overall input voltage of the controller.

[__SOURCE](2-servo-control-board-part/E02521.md)
# 2.11. E02521 (Axis ○) IPM Fault - Gate Drive Power Under-voltage

### 1. Overview

A fault output has been generated from the IPM (Intelligent Power Module), the switching element within the servo drive unit. While IPM faults can generally be caused by heatsink temperature rise, control voltage drops, or overcurrent, this specific error is detected when an IPM fault occurs while the servo is OFF. Since the IPM only monitors for control voltage drops during the servo-off state, please inspect items related to the amplifier's gate drive power supply.

### 2. Causes and Inspection Methods

{% hint style="info" %}

* < If the IPM fault error occurs while the servo is OFF >

(1) Please inspect the components used for motor drive.

->  Inspect the output cables connected to the servo drive unit.

->  Replace the servo drive unit and verify if the error persists.

->  Replace the servo board and verify if the error persists.

{% endhint %}

(1)	Please inspect the components used for motor drive.

The servo drive unit, which powers the motor, receives commands from the servo board via a board-to-board connector linked to the interface board. The current output from the internal amplification circuit is then transmitted to the motor through the wiring connected to each axis's connector.

->  Inspection of the output cables connected to the servo drive unit

Inspect the condition of the wiring connecting the servo drive unit to the motor. During inspection, ensure the controller power is OFF, disconnect the connector from the servo drive unit, and measure the resistance between each phase and the ground on the cable side to check for short circuits.


![](../_assets/2.서보AMP/E02521/E02521_IPM폴트_서보구동장치케이블점검_N제어기_en.PNG)

(a) Hi6-N Controller

![](../_assets/2.서보AMP/E02521/E02521_IPM폴트_서보구동장치케이블점검_T제어기.PNG)

(b) Hi6-T Controller

Figure 1.1 Inspection of Servo Drive Unit Output Cables



->  Servo Drive Unit Replacement Inspection

If the error does not recur after replacing the servo drive unit, the original unit is defective. Please replace the servo drive unit with a known functional unit.

*   Hi6-N Controller

    -   Servo drive unit for mid-sized robots: H6D6X
    -   Servo drive unit for small-sized robots: H6D6A

*   Hi6-T15 Controller

    -   Main 3-axis servo drive unit: BD658T
    -   Sub 3-axis servo drive unit: BD657T


->  Servo Board (BD544) Replacement Inspection

If the error does not recur after replacing the servo board, the original board is defective. Please replace the servo board with a known functional unit.

*   Hi6-N Controller: BD640
*   Hi6-T15 Controller: BD641T
[__SOURCE](2-servo-control-board-part/E02522.md)
# 2.12. E02522 (Axis ○) IPM Fault – Specific Step

### 1. Overview

A fault output has been generated from the IPM (Intelligent Power Module), which is the switching element within the servo drive unit that powers the motor. An IPM fault can be caused by an increase in the heatsink temperature, a drop in the IPM control voltage, or an overcurrent output.

### 2. Causes and Inspection Methods

{% hint style="info" %}

* < If the error occurs at a specific step>

(1)	Please inspect the robot at the step where the error occurs.

->  Inspect the robot wiring at the position where the error is triggered.

->  Reduce the robot's playback speed and verify if the error persists.

->  Change the interpolation of the taught step and verify if the error persists.

{% endhint %}


(1)	Please inspect the robot at the step where the error occurs.

An IPM fault error occurring at a specific step can be caused by significant damage to the mechanical wiring at that taught position, or by excessive changes in axis speed during posture transitions within the taught program.


->  Inspection of internal wiring at the position where the error occurs

Inspect the condition of the internal wiring connected to the motor of the corresponding axis. During inspection, ensure the controller power is OFF, disconnect the output connector from the servo drive unit, and measure the resistance between each phase and the ground on the cable side to check for short circuits.

![](../_assets/2.서보AMP/E02522/E02522_HS165_축별기내배선_점검위치.PNG)

Figure 1.1 Internal Wiring Inspection Points for Each Axis of the Robot


-> Verify the error by reducing the robot's playback speed

If the error occurs at a step where a posture transition causes a sudden change in axis speed, reduce the playback speed to verify the error. If the error is resolved by lowering the speed, adjust the teaching speed of the corresponding step and save the task program before use.

->  Verify the error by changing the interpolation of the taught step

If axis speed fluctuations remain extreme even after reducing the playback speed below 75%, change the interpolation of the taught step to 'P' (Point-to-Point) and verify the error. If the error is resolved by changing the interpolation at the same playback speed, please modify the teaching points.

[__SOURCE](2-servo-control-board-part/E02541.md)
# 2.13. E02541 Drive Unit Control Voltage Drop

### 1. Overview

The +15V control power supplied to the servo drive unit has dropped below the threshold. This error is detected through different paths depending on the controller model and is then transmitted to the servo board.

*   Hi6-N: Detected at the servo drive unit.
*   Hi6-T: Detected at the backplane board (BD602T).

### 2. Causes and Inspection Methods

{% hint style="info" %}

*   <Checking the Power LEDs>

    (1)	Please check the power status LEDs.

    ->  Hi6-N: Check the "POW" LED on the servo drive unit.

    ->  Hi6-T: Check "LED5" on the backplane board (BD602T).

    ->  Check the "DC OK" LED on the CMSMPS (Control Main Switched Mode Power Supply).


*   <If both Board LEDs and SMPS LEDs are OFF>

    (2)	Please verify the output of the control power supply unit.

    ->  Hi6-N

    *  Disconnect the CN24VB1 connector from the BD640 and check if the "SMPS OK" LED on the PSM turns ON.

    *  Remove the BD640 board and check the "POW" LED on the servo drive unit.

    ->  Hi6-T 

    *   Disconnect the CN24VB1 connector from the BD602T and check if the "DC OK" LED on the CMSMPS turns ON.

    *   Remove the BD641T board and check "LED5" on the backplane board (BD602T).


    (3)	Please inspect the control power supply unit.

    ->  Verify the input voltage supplied to the CMSMPS.

    ->  Replace the CMSMPS and check if the LEDs turn ON.

    * <If only the Board LEDs are OFF>

    (4)	Replace the relevant components and check the power status LEDs.

    -> Hi6-N

    * Replace the CN24VB1 cable connecting the PSM and BD640, then check the LED status.

    * Replace the servo board and check the LED status.

    * Replace the servo drive unit and check the LED status.

    ->  Hi6-T

    * Replace the CN24VB1 cable connecting the CMSMPS and the backplane board (BD602T), then check the LED status.

    * Replace the servo board and check the LED status.

    * Replace the backplane board (BD602T) and check the LED status.


{% endhint %}


(1)	Please check the power status LEDs.

The "Drive Unit Control Voltage Drop" error occurs due to a drop in the +15V control power. This condition is detected through different paths depending on the controller model and then transmitted to the servo board.

*   Hi6-N : Detected at the servo drive unit.

*   Hi6-T : Detected at the backplane board (BD602T).

![](../_assets/2.서보AMP/E02541/E02541_서보구동장치_POW_LED_위치_N제어기_en.PNG)

(a) Location of the "POW LED" on the Hi6-N controller servo drive unit

![](../_assets/2.서보AMP/E02541/E02541_백플레인보드_LED5_위치_T제어기.PNG)

(b) Location of "LED5" on the Hi6-T controller backplane board

Figure 1.1 Locations of Controller Power Status LEDs

<br>


(2)	Please verify the output of the control power supply unit.

->  Hi6-N

*   Disconnect the CN24VB1 connector from the BD640, then check if the "SMPS OK" LED on the PSM turns ON.

*   Remove the BD640 board, then check the "POW" LED on the servo drive unit.

->  Hi6-T

*   Disconnect the CN24VB1 connector from the BD602T, then check if the "DC OK" LED on the CMSMPS turns ON.

*   Remove the BD641T board, then check "LED5" on the backplane board (BD602T).

(3)	Please inspect the control power supply unit.

->  Verify the input voltage supplied to the CMSMPS.

->  Replace the CMSMPS and verify the status of the LEDs.

(4)	Replace the relevant components and check the power status LEDs.

->  Hi6-N

*   Replace the CN24VB1 cable connecting the PSM and BD640, then check the LED status.

*   Replace the servo board and check the LED status.

*   Replace the servo drive unit and check the LED status.

->  Hi6-T

*   Replace the CN24VB1 cable connecting the CMSMPS and the backplane board (BD602T), then check the LED status.

*   Replace the servo board and check the LED status.

*   Replace the backplane board (BD602T) and check the LED status.



[__SOURCE](3-safety-board-part/README.md)
# 3. Safety Signal Board
[__SOURCE](3-safety-board-part/E00002.md)
# 3.1. E00002. Hardware Limit Switch Triggered

### 1. Overview

The limit switch installed at the end of the operating range for each robot axis has been triggered. For safety reasons, the robot stops immediately and cannot be operated normally until it is moved back into a safe operating range using the appropriate procedures.

### 2. Causes and Inspections

{% hint style="info" %}

**(1) Verify if the robot has actually exceeded its operating range.**
* Recovery procedure for operating range excursions

**(2) If the error occurs even though the robot is within its operating range**
* How to inspect from the system board connector (CNLS) <br>
* How to inspect from the wire harness (C(M)ER1 or C(M)EC1) <br>
* How to inspect the limit switches and internal body wiring <br>
* How to inspect the safety board (BD632)<br>

{% endhint %}

#### (1) Verify if the robot has actually exceeded its operating range.
Check if the robot has physically moved outside its designated operating range. If a Soft Limit Error has occurred simultaneously, it confirms that the robot has exceeded its operating range. Move the robot back into the safe operating range using the appropriate manual operations. <br><br>

The operating range varies depending on the robot model. Since the installation positions of the limit switches may also differ, please refer to the "Operating Range Limits" section in the maintenance manual for the specific robot model.

![](../_assets/3-Safety-io/E00002/그림1.jpg)<br>
Figure 1 Example of hardware limit switch installation positions

![](../_assets/3-Safety-io/E00002/그림2.png)<br>
Figure 2 Example of hardware limit switch operating range (S Axis)

### [Recovery procedure for operating range excursions]
To move the robot while the hardware limit switch is engaged, you must follow the conditions and steps outlined below:

A) Enter System mode from Manual mode. B) Grip the Enabling Switch on the Teach Pendant. > 『Manual Mode』 + 『System』 + 『TP Enabling Switch ON』

C) Turn the motors ON in this state. D) Use the Jog keys to move the robot back into the safe operating range.

#### (2) If the error occurs even though the robot is within the operating range
First, check the dedicated input signal window on the Teach Pendant to see if the **Over-Travel (Limit)** item is continuously being input. You can view this window by selecting **"『Window Layout』 → 『Select』 → 『System Input』"**. If the **Over-Travel** item is highlighted in **yellow**, it indicates an error state.


### [Caution]
In Manual mode, the Enabling Switch on the Teach Pendant must be **ON** for monitoring. In Auto mode, monitoring is active regardless of the Enabling Switch status.

![](../_assets/3-Safety-io/E00002/그림3.png)<br>
Figure 3 Over-Travel monitoring display in the System Input window

In such cases, the cause can be found in components related to the limit switches. As shown in the following figure, the limit switches are connected from the robot body to the system board of the controller via the "CEC1 – CER1" cables for the Hi6-N model, or the "CMEC1 – CMER1" cables for the Hi6-T model.

![](../_assets/3-Safety-io/E00002/그림4_en.png)<br>
Figure 4 Wiring structure of the hardware limit switches


The main inspection points and sequence are as follows:

A) System Board <br>
B) Internal Controller Wiring and Connectors<br>
C) Wire Harness and Connectors<br>
D) Limit Switches and Internal Body Wiring<br>

You must jumper the limit switch input lines at the appropriate points and verify if the Over-Travel item in the monitoring window changes to white. <br>
Please proceed according to the following steps.


### [How to inspect from the system board connector (CNLS)]

{% hint style="warning" %}

Warning<br> 
Always ensure that the controller power is turned OFF when connecting or removing cables. Electrical hazards can lead to personal injury or property damage.

{% endhint %}

This procedure determines whether the system board itself is faulty. As shown in the figure below, jumper (short-circuit) the pins related to the limit switch input on the CNLS connector. Then, check the Over-Travel status in the dedicated input signal monitoring window.

① If the status changes to white: The system board is faulty. Replace the board.<br>
② If the status remains yellow (error state): The system board is functioning correctly. Inspect for faults in the section from the system board to the robot's hardware limit switches.<br>

![](../_assets/3-Safety-io/E00002/그림5_en.png)<br>
Figure 5 Hi6-N System Board

![](../_assets/3-Safety-io/E00002/그림6_en.png)<br>
Figure 6 Hi6-T System Board


###  How to inspect from the wire harness (C(M)ER1 or C(M)EC1)

{% hint style="warning" %}

Warning<br> 
Always ensure that the controller power is turned OFF when connecting or disconnecting cables. Electrical hazards can lead to personal injury or property damage.

{% endhint %}

This procedure is used to determine if the cable is faulty through the C(M)ER1 or C(M)EC1 wire harness connectors. First, remove the C(M)EC1 wire harness from the controller. Then, jumper-short the pins related to the limit switch on the C(M)EC1 connector mounted on the controller. In this state, check the Over-Travel item through the dedicated input signal monitoring window.

① If the status changes to white: <br>
The fault lies in the cable or the connector between the controller's internal C(M)EC1 connector and the system board. Inspect or replace these components.

② If the status remains yellow (error state): <br>
The fault is located in the section between the C(M)EC1 connector and the robot body's limit switches.

Reconnect the C(M)EC1 wire harness, then disconnect the C(M)ER1 wire harness from the robot body. Jumper-short the pins related to the limit switch on the C(M)ER1 connector of the wire harness. In this state, check the status of the Over-Travel item in the dedicated input signal monitoring window.

① If the status changes to white: <br>
The fault lies in the wire harness cable or the connectors between the C(M)ER1 and C(M)EC1 connectors. Inspect or replace the wire harness.

② If the status remains yellow (error state): <br>
The fault is located in the section from the robot body's C(M)ER1 connector to the limit switches. Check the internal body wiring or the switches themselves.

![](../_assets/3-Safety-io/E00002/그림7_en.png)<br>
Figure 7 Hardware Limit Switch Harness C(M)EC Structure

### [How to Inspect the Limit Switch and Internal Wiring of the Main Unit]

{% hint style="warning" %}

**Warning**  
Always ensure that the controller power is turned off before connecting or disconnecting any cables.  
Electrical hazards may result in serious personal injury or property damage.

{% endhint %}

After disconnecting the CER1 wire harness from the main unit, use a multimeter to perform a short-circuit test on the limit switch–related lines at the CER1 connector of the main unit.

① If the resistance is measured as **open**,<br>
the limit switch itself or the connector between the limit switch and CER1 may be faulty.  
Inspect the components or replace them as necessary.

② If the resistance is measured as **short**,<br>
check for faults in other parts of the system.  
Please contact our technical support.

![](../_assets/3-Safety-io/E00002/그림8_en.png)<br>
Figure 8 Hardware Limit Switch Harness C(M)ER Structure

### [How to Inspect the Safety Board (BD632)]

![](../_assets/3-Safety-io/E00002/그림9_en.png)<br>
**Figure 9** Safety Board (BD632)

1) How to check the IO power status<br>
A. Verify that the two LEDs shown in the figure above are lit **green**.<br>
B. If the IO power LED is **red** or **off**, check whether the indicated fuse is in normal condition.<br>
C. If the fuse is blown, replace it with a new one.<br>

2) How to check whether the IO power becomes unstable when the motor is ON<br>
A. When the motor is ON, verify that the IO power LED is lit **green**.<br>
B. If the LED turns **red** or turns **off** at the moment the motor is turned ON, the IO power is unstable during motor operation.<br>

3) If the IO power status is unstable<br>
A. Check the connection of the IO power connector.<br>
B. Inspect the IO power cable.<br>
C. Check the grounding condition of the Safety Board (BD632) <br> 
(ground cable and grounding terminal connection status).<br>



[__SOURCE](3-safety-board-part/E00014.md)
# 3.2. E0014. Momentary Contact of Safety Switches (EM, OTR, TS, etc.)

### 1. Overview

For some reason, the motor power supplied to the amplifier has been cut off.  
The main controller checks the safety signals to identify the cause of the motor power shutdown.  
If no abnormal condition is detected in the safety signal inputs, this message is displayed.

The figure below shows the configuration of various safety signals that can interrupt the motor power.  
The main controller periodically monitors the ON/OFF status of these safety signals.  
If a momentary contact failure occurs for a duration shorter than the monitoring cycle, the main controller may not detect it and will display this message.

![](../_assets/3-Safety-io/E00014/그림1.png)<br>
**Figure 1** Conceptual Diagram of the Safety Circuit for Motor Power Switching

### 2. Causes and Inspection

{% hint style="info" %}

(1) Check the DC 24 V power supply and cable condition.<br>

(2) Check the safety switches and signal wiring.<br>

(3) Check the system board and electrical module.<br>

{% endhint %}

### (1) Check the DC 24 V Power Supply and Cable Condition

Verify that the DC 24 V control power is being supplied normally to the system board.  
If there is an issue with the power supply, it may affect the safety sequence of the system board and cause this error.

For the **Hi6-N controller**, power is supplied through the following connections:  
- Electrical module connectors **CN24VB3** and **CN24VB4**  
- System board connectors **CNSMPS1** and **CNSMPS2**

Check whether the power supply voltage is fluctuating or if there are any abnormalities in the cables.

![](../_assets/3-Safety-io/E00014/그림2_en.png)<br>
**Figure 2** DC 24 V Power Connection and Voltage Check Method for the Hi6-N System Board (BD632)

For the **Hi6-T controller**, power is supplied through:  
- **SMPS & BUFFER connector**  
- Backplane board connector **CN24VB1**  
- Board-to-board connections between the backplane board and the system board

Check whether the power supply voltage is fluctuating or if there are any abnormalities in the cables.

![](../_assets/3-Safety-io/E00014/그림3_en.png)<br>
**Figure 3** DC 24 V Power Connection for the Hi6-T Controller

### (2) Check the Safety Switches and Signal Wiring

A condition may occur where the safety switch input momentarily turns OFF for a duration too short for the MAIN board to recognize.

Possible causes include:

- **Safety switch failure**
- **Wiring failure**: damage such as cuts or abrasion of the cable
- **Improper cable routing**:  
  Signal cables must be routed at least **10 cm** away from power lines or cables that carry high current.  
  Alternatively, electronic shielding should be applied using metal plates or equivalent shielding materials.

{% hint style="warning" %}

**Caution**  
Disabling or bypassing safety-related functions must be used **for testing purposes only** and must be restored immediately after testing.  
Operating the system while safety functions are ignored may lead to serious safety hazards.

{% endhint %}

The following types of safety switches can be used and must be connected through the system board.  
Please refer to the specifications corresponding to the safety switches currently in use.

![](../_assets/3-Safety-io/E00014/그림4_en.png)<br>
![](../_assets/3-Safety-io/E00014/그림5_en.png)<br>
![](../_assets/3-Safety-io/E00014/그림6_en.png)<br>

{% hint style="warning" %}

**Caution**  
Disabling or bypassing safety-related functions must be used **for testing purposes only** and must be restored to their original state immediately.  
Operating the system while safety functions are ignored may cause serious safety-related issues.

{% endhint %}

Other safety-related and system operation switches that may affect this error include the following:

![](../_assets/3-Safety-io/E00014/그림7_en.png)<br>
![](../_assets/3-Safety-io/E00014/그림8_en.png)<br>
![](../_assets/3-Safety-io/E00014/그림9_en.png)<br>


### (3) Check the System Board and Electrical Module

- **Cabling failure (wires, connectors, etc.)**

For the **Hi6-N controller**, check the cabling between the electrical module  
(**PSM or PDM**), where the electromagnetic contactor is installed, and the system board that collects the monitoring signals.

The cable name is **CNMC**, and it is routed from the lower front side of the system board to the electrical module.  
Check the connector connection status of this cable.

![](../_assets/3-Safety-io/E00014/그림14.png)<br>
**Figure 4** Hi6-N Controller

For the **Hi6-T controller**, the electromagnetic contactor is installed on the PCB board, and the monitoring signals are connected to the system board through **board-to-board** connections.  
Check the board-to-board connection status.

![](../_assets/3-Safety-io/E00014/그림15_en.png)<br>
**Figure 5** CNMC Cable Between the Electrical Module and the System Board

- **System Board Failure**

A failure in the input signal processing circuitry inside the system board may also cause this error.  
Replace the system board to verify.

- **Electrical Module Failure (Hi6-N Controller Only)**

Failures inside the electrical module can be broadly classified into the following components:
- Electrical board (**BD6C2**)
- Electromagnetic contactors (**MC1**, **MC2**)
- Wiring between the electrical board and the electromagnetic contactors

However, since it is difficult to inspect the inside of the electrical module at a site where the robot is already installed,  
replace the entire electrical module.

![](../_assets/3-Safety-io/E00014/그림16_en.png)<br>
**Figure 6** Electrical Module Structure and Nomenclature for the Hi6-N Controller

[__SOURCE](3-safety-board-part/E00043.md)
# 3.3. E0043. Auto Mode Safety Guard (Auto Guard) Switch Connection Error

### 1. Overview

A connection error has occurred in the safety plug (Auto Guard) switch while in **Auto mode**.  
In Auto mode, the motor ON state cannot be maintained when this error occurs.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) When the input of the Auto Mode Safety Guard switches (**SGA1**, **SGA2**) is unstable  
- How to check the input status of the Auto Mode Safety Guard switches (SGA1, SGA2)

(2) When the error occurs regardless of the input state of the Auto Mode Safety Guard switches (**SGA1**, **SGA2**)  
- How to inspect the Safety Board (BD632)  
- How to check the connection status with the Teaching Pendant (TP630)

{% endhint %}

### (1) When the input of the Auto Mode Safety Guard switches (SGA1, SGA2) is unstable

- How to check the input status of the Auto Mode Safety Guard switches (SGA1, SGA2)

![](../_assets/3-Safety-io/E00043/그림1.png)<br>

1) Use the system input screen on the Teaching Pendant (TP) to check the Auto Safety Guard signal input status and identify which Auto Safety Guard signals are currently active  
&nbsp;&nbsp;&nbsp;&nbsp;(SGA1 on the left, SGA2 on the right).

2) At the **TBEM terminal**, check the connection status of the **SGA1** and **SGA2** terminals, the condition of the cables, and whether there are any abnormalities in the input switches.

![](../_assets/3-Safety-io/E00043/그림2.png)<br>

### (2) When the error occurs regardless of the input state of the Auto Mode Safety Guard switches (SGA1, SGA2)

- How to inspect the Safety Board (BD632)

![](../_assets/3-Safety-io/E00043/그림3_en.png)<br>


1) How to check the IO power status<br>
A. Verify that the two LEDs shown in the figure above are lit **green**.<br>
B. If the IO power LED is **red** or **off**, check whether the indicated fuse is in normal condition.<br>
C. If the fuse is blown, replace it with a new one.<br>

2) How to check whether the IO power becomes unstable when the motor is ON<br>
A. When the motor is ON, verify that the IO power LED is lit **green**.<br>
B. If the LED turns **red** or turns **off** at the moment the motor is turned ON, the IO power is unstable during motor operation.<br>

3) If the IO power status is unstable<br>
A. Check the connection of the IO power connector.<br>
B. Inspect the IO power cable.<br>
C. Check the grounding condition of the Safety Board (BD632, ground cable and grounding terminal connection status).<br>

- How to check the connection status with the Teaching Pendant (TP630)

![](../_assets/3-Safety-io/E00043/그림4.png)<br>

1) Check the connection status of the **CNTP** connector.<br>
2) Inspect the **CNTP cable**  <br>
– Check for cable damage  <br>
– Verify that the cable length is **40 m or less**  <br>
– Use a **certified cable**<br>
3) Check the grounding condition of the Safety Board (**BD632**)  
– Ground cable condition  
– Ground terminal connection status



[__SOURCE](3-safety-board-part/E02200.md)
# 3.4. E02200. Main Unit Limit Switch Activated

### 1. Overview

The limit switch installed at the end of the operating range of each robot axis has been activated.  
For safety reasons, the robot stops immediately and normal operation cannot be resumed until the robot is moved back into a safe operating range using an appropriate recovery method.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) The robot has moved beyond the hardware operating range.

(2) Move the robot back into the operating range.  
- Recovery method when the robot has moved outside the operating range

{% endhint %}

### (1) The robot has moved beyond the hardware operating range

Check once again whether the robot has actually moved outside the operating range.  
A software limit error is likely to have occurred simultaneously, indicating that the robot has exceeded its maximum operating range.  
Using an appropriate operation method, move the robot back into the operating range.

![](../_assets/3-Safety-io/E02200/그림1.png)<br>
**Figure 1** Occurrence of E02200: Main Unit Limit Switch Activated

The operating range varies depending on the robot model.  
Accordingly, the installation position of the limit switches may also differ.  
Refer to the **“Operating Range Limitation”** section in the corresponding mechanical maintenance manual.

![](../_assets/3-Safety-io/E02200/그림2.png)<br>
**Figure 2** Example of Hardware Limit Switch Installation Positions

![](../_assets/3-Safety-io/E02200/그림3.png)<br>
**Figure 3** Example of Hardware Limit Switch Operating Range  
(S-axis)

### (2) Move the robot back into the operating range

Refer to the following recovery method for operating range violation and move the robot back into the operating range.

- Recovery method when the robot has moved outside the operating range

To move the robot while the hardware limit switch is activated, execute the following conditions and steps in order.

A) Enter **System mode** from **Manual mode**.<br>
B) Hold the **Enabling Switch** on the Teaching Pendant (TP).<br>

『Manual Mode』 + 『System』 + 『TP Enabling Switch ON』

C) In this state, turn the **Motor ON**.<br>
D) Use the **Jog keys** to move the robot back into the operating range.<br>

[__SOURCE](3-safety-board-part/E02201_E2208.md)
# 3.5. E02001 ~ E02208 Hardware Limit Switch Inspection Method

### 1. Causes and Inspection Methods

If the hardware limit switch operates abnormally, refer to the following inspection methods.

### (1) Switch Status Monitoring

The hardware limit input status can be checked through the dedicated input signal screen on the Teaching Pendant (TP).  
This screen can be accessed by selecting  
**『Window Setup』 → 『Select』 → 『System Input』**.

If the **Limit (Over-Travel)** item is displayed in **yellow**, the hardware limit switch is activated (open),  
indicating that the robot has moved outside the hardware operating range.

- **Caution:**  
  In **Manual mode**, monitoring is available only when the **Enabling Switch** on the Teaching Pendant is turned **ON**.  
  In **Auto mode**, monitoring is available regardless of the Enabling Switch state.

![](../_assets/3-Safety-io/E02201_2208/그림1.png)<br>
**Figure 1** Hardware Limit Switch Input Status Display (Teaching Pendant Screen)

### (2) Hardware Limit Switch Wiring Structure

To identify the cause within the components related to the hardware limit switch, it is necessary to understand the wiring structure.  
As shown in the figure below, the hardware limit switch signal starts from the limit switch inside the robot mechanical unit and is connected via cables to the system board inside the controller.

- Limit switch and internal robot mechanical unit wiring  
- Wire harness and connectors  
  (For Hi6-N: **CER1 – CEC1**, for Hi6-T: **CMER1 – CMEC1**)  
- Internal controller wiring and connectors  
  (For Hi6-N: **CEC1 – CNLS**, for Hi6-T: **CMEC1 – CNLS1**)  
- System board  
  (For Hi6-N: **BD632**, for Hi6-T: **BD632T**)

![](../_assets/3-Safety-io/E02201_2208/그림2_en.png)<br>
(a) Hi6-N Controller

![](../_assets/3-Safety-io/E02201_2208/그림3_en.png)<br>
(b) Hi6-T Controller

**Figure 2** Hardware Limit Switch Wiring Structure


### (3) Hardware Limit Switch Inspection Method

#### Inspection via System Board Connector (CNLS)

{% hint style="warning" %}
**Warning**  
Always turn **OFF the controller power** before connecting or disconnecting cables.  
Electrical hazards may result in serious personal injury or property damage.
{% endhint %}

This inspection method is used to **determine whether the system board is faulty**.

As shown in the figure below, **jumper-short the pins related to the limit switch inputs** at the **CNLS connector** on the system board.  
Then check the **Limit (Over-Travel)** status in the **Dedicated Input Signal Monitoring** window.

- **① If the indication changes to white**  
  → The system board is faulty.  
  → Replace the system board.

- **② If the indication remains yellow (error state)**  
  → Check for faults in the section from the system board to the hardware limit switches in the robot body.

![](../_assets/3-Safety-io/E02201_2208/그림4_en.png)<br>
(a) Hi6-N System Board

![](../_assets/3-Safety-io/E02201_2208/그림5_en.png)<br>
(b) Hi6-T System Board

Figure 3 System Board

#### [Inspection Method at the Wire Harness (C(M)ER1 or C(M)EC1)]

{% hint style="warning" %}
When connecting or disconnecting cables, always perform the operation with the controller power turned OFF.  
Electrical hazards may cause personal injury or property damage.
{% endhint %}

This method is used to determine whether there is a cable failure through the wire harness connector C(M)ER1 or C(M)EC1.

First, disconnect the C(M)EC1 wire harness from the controller.  
Then, jumper-short the pins related to the limit switch (Limit SW) at the C(M)EC1 connector attached to the controller.

In this condition, check the **Limit (Over-Travel)** item in the dedicated input signal monitoring window.

① **If the status changes to white:**  
The cable or connector between the internal C(M)EC1 connector and the system board inside the controller is faulty.  
Inspect or replace the cable or connector.

② **If the status remains yellow (error state):**  
Check for a failure in the area after the C(M)EC1 connector up to the robot body limit switch.

![](../_assets/3-Safety-io/E02201_2208/그림6_en.png)<br>
(a) Hi6-N Controller

![](../_assets/3-Safety-io/E02201_2208/그림7_en.png)<br>
(b) Hi6-T Controller

Figure 4 Structure of the Hardware Limit SW Harness C(M)EC1

#### [How to Check the Limit SW and Internal Wiring of the Robot Body]

After removing the C(M)ER1 wire harness from the robot body, use a multimeter to perform a short test on the limit SW–related lines at the C(M)ER1 connector on the robot body to check for abnormalities.

① If the resistance is measured as open,<br>
This indicates a failure of the limit SW itself, or a fault in the connector or wiring between the limit SW and CER1.  
Inspect and repair or replace the faulty component.

② If the resistance is measured as short,<br>
A fault exists in another area. Further troubleshooting is required. Please contact our service department.

![](../_assets/3-Safety-io/E02201_2208/그림8_en.png)<br>
(a) Hi6-N Controller

![](../_assets/3-Safety-io/E02201_2208/그림9_en.png)<br>
(b) Hi6-T Controller

Figure 5 Structure of the Hardware Limit SW Harness C(M)ER1


[__SOURCE](3-safety-board-part/E02201.md)
# 3.6. E02201. Body Limit SW Input Mismatch (Safety Chain 1 OFF)

### 1. Overview

The robot has moved outside the software limit area. However, the input from the limit switches installed at the end of each robot axis operating range is not normal.  
Since the input of Safety Chain 1 differs from the input of Safety Chain 2, inspection is required.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) If the robot has NOT exceeded the hardware operating range  
* A problem exists in Safety Chain 1. Inspect the limit SW wiring.

(2) If the robot HAS exceeded the hardware operating range  
* A problem exists in Safety Chain 2. Inspect the limit SW wiring.

{% endhint %}

(1) When the robot has NOT exceeded the hardware operating range

![](../_assets/3-Safety-io/E02201/그림1.png)<br>
Figure 1 E02201 Body Limit SW Input Mismatch (Safety Chain 1 OFF) – Inside the hardware operating range

Since there is a problem in Safety Chain 1, inspect the limit SW wiring.

Although the robot is within the area where the hardware limit SW is installed, Safety Chain 1 is monitored as OFF.  
This condition may be caused by the following reasons:

* Hardware limit SW failure: The switch is damaged or opened (Open) for some reason.
* Wiring: The wiring is disconnected or damaged, causing poor contact.
* Connector: The connector is disconnected or damaged, resulting in disconnection or poor contact.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.

(2) When the robot HAS exceeded the hardware operating range
![](../_assets/3-Safety-io/E02201/그림2.png)<br>
Figure 2 E02201 Body Limit SW Input Mismatch (Safety Chain 1 OFF) – Outside the hardware operating range

Since there is a problem in Safety Chain 2, inspect the limit SW wiring.

Although the robot has moved outside the area where the hardware limit SW is installed, Safety Chain 2 fails to detect the abnormal condition.  
In other words, Safety Chain 2 remains continuously closed.

This condition may be caused by the following reasons:

* Hardware limit SW failure: The switch is damaged or short-circuited (Short) for some reason.
* Wiring: The two lines of a wire pair are short-circuited.
* Connector: The connector is damaged, causing a short circuit between pins.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.

[__SOURCE](3-safety-board-part/E02202.md)
# 3.7. E02202. Body Limit SW Input Mismatch (Safety Chain 2 OFF)

### 1. Overview

The robot has exceeded the soft limit range.  
However, the input from the limit switches installed at the end of each robot axis operating range is not normal.  
Since the inputs of Safety Chain 1 and Safety Chain 2 are different, inspection is required.

### 2. Causes and Inspection Method

{% hint style="info" %}

(1) When the hardware operating range has NOT been exceeded  
* Since there is a problem in Safety Chain 2, inspect the limit SW wiring.

(2) When the hardware operating range HAS been exceeded  
* Since there is a problem in Safety Chain 1, inspect the limit SW wiring.

{% endhint %}

(1) When the hardware operating range has NOT been exceeded

![](../_assets/3-Safety-io/E02202/그림1.png)<br>
Figure 1 E02202 Body Limit SW Input Mismatch (Safety Chain 2 OFF) – Inside the hardware operating range

Since there is a problem in Safety Chain 2, inspect the limit SW wiring.

Although the robot is located within the area where the hardware limit SW is installed, Safety Chain 2 is monitored as being OFF.  
This condition may be caused by the following reasons:

* Hardware limit SW failure: The switch is damaged or opened (Open) for some reason.
* Wiring: The wiring is disconnected or damaged, causing poor contact.
* Connector: The connector is disconnected or damaged, resulting in disconnection or poor contact.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.

(2) When the hardware operating range HAS been exceeded

![](../_assets/3-Safety-io/E02202/그림2.png)<br>
Figure 2 E02202 Body Limit SW Input Mismatch (Safety Chain 2 OFF) – Outside the hardware operating range

Since there is a problem in Safety Chain 1, inspect the limit SW wiring.

Although the robot has moved outside the area where the hardware limit SW is installed, Safety Chain 1 does not detect any abnormal condition.  
In other words, Safety Chain 1 remains continuously closed.

This condition may be caused by the following reasons:

* Hardware limit SW failure: The switch is damaged or short-circuited (Short) for some reason.
* Wiring: The two lines in a pair of wires are short-circuited.
* Connector: The connector is damaged, causing a short circuit between pins.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.

[__SOURCE](3-safety-board-part/E02206.md)
# 3.8. E02206. Body Limit SW Open Circuit or Not Connected

### 1. Overview

This is an abnormal condition in which the limit switch installed at the end of the operating range of each robot axis is detected as activated even though the robot has not exceeded the soft limit range.  
Since this is an abnormal condition, the limit SW wiring must be inspected.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This is an abnormal condition in which hardware limit switch operation is detected without exceeding the soft limit.

Inspect the switch and wiring system, as a problem may exist.

{% endhint %}

Occurrence of E02206 Body Limit SW Open Circuit or Not Connected

This is an abnormal condition in which the hardware limit SW operation is detected even though the soft limit has not been exceeded.  
Since there may be a problem with the switch or wiring system, inspection is required.

* Hardware limit SW failure: The switch is damaged or opened (open) for some reason.
* Wiring: The wiring is broken or damaged, causing poor contact.
* Connector: The connector is disconnected or damaged, resulting in an open-circuit due to poor connection.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.

[__SOURCE](3-safety-board-part/E02207.md)
# 3.9. E02207. Body Limit SW Input Mismatch (Safety Chain 1 OFF)

### 1. Overview

Although the robot has not exceeded the soft limit range, the limit switch installed at the end of the operating range of each robot axis is detected as being activated.  
Since the input state of Safety Chain 1 is different from that of Safety Chain 2, inspection is required.

### 2. Cause and Inspection Method

{% hint style="info" %}

This is an abnormal condition in which the hardware limit SW operation is detected even though the soft limit has not been exceeded.

Since there is a problem in the switch or wiring system, perform an inspection.

{% endhint %}

![](../_assets/3-Safety-io/E02207/그림1.png)<br>
Figure 1. Occurrence of E02207 Body Limit SW Input Mismatch (Safety Chain 1 OFF)

This is an abnormal condition in which the hardware limit SW operation is detected even though the soft limit has not been exceeded.  
The problem occurs because Safety Chain 1 is open. Inspect the related switches and wiring system.

* Hardware limit SW failure: The switch is damaged or opened for some reason.
* Wiring: The wiring is broken or damaged, causing poor contact.
* Connector: The connector is disconnected or damaged, resulting in an open-circuit or contact failure.

For detailed inspection points, refer to the section **“Hardware Limit Switch Inspection Method.”**

[__SOURCE](3-safety-board-part/E02208.md)
# 3.10. E02208. Body Limit SW Input Mismatch (Safety Chain 2 OFF)

### 1. Overview

Although the robot has not exceeded the soft limit area, the limit SW installed at the end of each axis motion range is detected as being activated.  
Since the input states of Safety Chain 1 and Safety Chain 2 are different, inspection is required.

### 2. Causes and Inspection Methods

{% hint style="info" %}

This is an abnormal condition in which the hardware limit SW operation is detected even though the soft limit has not been exceeded.

Inspect the switch and wiring system, as there may be a problem in these components.

{% endhint %}

![](../_assets/3-Safety-io/E02208/그림1.png)<br>
Figure 1 Occurrence of E02208 Body Limit SW Input Mismatch (Safety Chain 2 OFF)

This is an abnormal condition in which the hardware limit SW operation is detected even though the soft limit has not been exceeded.  
The problem occurs because Safety Chain 2 is opened (open).  
Inspect the related switches and wiring system.

* Hardware limit SW failure: The switch is damaged or opened (open) for some reason.
* Wiring: The wiring is broken or damaged, causing poor contact.
* Connector: The connector is disconnected or damaged, resulting in an open-circuit due to poor contact.

For detailed inspection points, refer to the section “Hardware Limit Switch Inspection Method”.
[__SOURCE](3-safety-board-part/E02260.md)
# 3.11. E02260. Magnetic Contactor (MC2) Failure / Detection Error During Servo ON Attempt

### 1. Overview

During an attempt to turn the servo ON, the magnetic contactor (MC2) did not operate.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) Inspect the monitoring system.<br>
(2) Inspect the magnetic contactor MC2.<br>
(3) Check the connection of the CNT1 cable and the open/close status of the CP of the power supply module.<br>
(4) Inspect the power board.<br>
(5) Inspect the power supply module (H6PSM30).<br>
(6) Inspect the servo amplifier.<br>
(7) If this error occurs in a system using two or more servo boards (BD640), check the DIP switch settings of the extended axis safety interface board (BD6H0).<br>

{% endhint %}

### (1) Inspect the Monitoring System

For the Hi6-N controller, check the cabling between the power module (PSM or PDM), where the magnetic contactor is installed, and the system board that collects the monitoring signals.  
The cable name is CNMC, and it is routed from the lower front side of the system board into the power module.  
Check the connector connection status of this cable.

![](../_assets/3-Safety-io/E02260/picture1.png)<br>
Figure 1 Hi6-N Controller

For the Hi6-T controller, the magnetic contactor is installed on the PCB board, and it is connected to the system board that collects the monitoring signals via a board-to-board connection.  
Check the board-to-board connection status.

![](../_assets/3-Safety-io/E02260/picture2_en.png)<br>
Figure 2 Hi6-T Controller

### (2) Inspect the Magnetic Contactor MC2

For the Hi6-N controller, check whether the magnetic contactor MC2 installed inside the power module operates normally.

![](../_assets/3-Safety-io/E02260/picture3.png)<br>
Figure 3 Hi6-N Controller (Magnetic contactor MC2 installed inside the power module)

For the Hi6-T controller, check whether the magnetic contactor MC2 installed on the Back Plane board operates normally.

![](../_assets/3-Safety-io/E02260/picture4.png)<br>
Figure 4 Hi6-T Controller (Magnetic contactor MC2 installed on the Back Plane board)

### (3) Check the Connection of the CNT1 Cable and the Open/Close Status of the CP of the Power Supply Module

For the Hi6-N controller, check the connection status of the CNT1 cable and the open/close status of the CP in the power module.

![](../_assets/3-Safety-io/E02260/picture7_en.png)<br>
Figure 5 Hi6-N Controller CNT1 Cable and CP

### (4) Inspect the Power Board

For the Hi6-N controller, inspect or replace the power board and cable wiring that relay signals between the system board and the magnetic contactor, as a problem may exist.

![](../_assets/3-Safety-io/E02260/picture5.png)<br>
Figure 6 Hi6-N Controller (Power board installed inside the power module)

For the Hi6-T controller, this item is not applicable because there is no corresponding cable wiring.

### (5) Inspect the Power Supply Module (H6PSM30)

Inspect the power supply module (H6PSM30) to verify that it is operating normally.

### (6) Inspect the Servo Amplifier

Inspect the servo amplifier to check for any abnormalities.

### (7) Check the DIP Switch Settings of the Extended Axis Safety Interface Board (BD6H0)  
(When Using Two or More Servo Boards (BD640))

If this error occurs in a system using two or more servo boards (BD640), check the DIP switch settings of the extended axis safety interface board (BD6H0).

When the axis configuration is changed in a system using two or more servo boards (BD640), the switches on the extended axis safety interface board must be adjusted.

As shown in the figure below, connect the extended axis safety interface board (BD6H0) and the servo boards (BD640) using the CNSSM1 to CNSSM4 connectors.  
If all four servo boards (BD640) are not connected, set the switches (SW1 to SW4) corresponding to the unconnected CNSSM numbers to the ON position.

**Example)** When using only two servo boards (BD640):
* Connect two SSMs using the CNSSM1 and CNSSM2 connectors.
* Set SW1 and SW2 to the OFF position.
* Set SW3 and SW4 to the ON position.

![](../_assets/3-Safety-io/E02260/picture6.png)<br>
Figure 7. DIP switch settings of the Extended Axis Safety Interface Board (BD6H0) 
[__SOURCE](3-safety-board-part/E02261.md)
# 3.12. E02261. MC2 Magnetic Contactor Failure/Detection Abnormality During Servo ON

### 1. Overview

While the servo is ON, the magnetic contactor MC2 turned OFF abnormally.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) Check the monitoring system.<br>
(2) Inspect the MC2 magnetic contactor.<br>
(3) Inspect the power distribution board.<br>
(4) Inspect the system board.<br>

{% endhint %}

For detailed inspection procedures, refer to **“E02260 MC2 Magnetic Contactor Failure/Detection Abnormality During Servo ON Attempt”**.

[__SOURCE](3-safety-board-part/E02280.md)
# 3.13. E02280. MC1 Magnetic Contactor Failure/Detection Abnormality During Servo ON Attempt

### 1. Overview

While attempting to turn the servo ON, the magnetic contactor MC1 did not operate.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) Check the monitoring system.<br>
(2) Inspect the MC1 magnetic contactor.<br>
(3) Inspect the power distribution board.<br>
(4) Inspect the system board.<br>

{% endhint %}

### (1) Check the monitoring system

For Hi6-N controller, check the cabling between the power module (PSM or PDM) where the magnetic contactor is installed and the system board that collects the monitoring signals. The cable name is CNMC and it enters the power module from the lower front of the system board. Inspect the connector connection status of this cable.

![](../_assets/3-Safety-io/E02280/그림1.png)<br>
Figure 1 Hi6-N Controller

For Hi6-T controller, the magnetic contactor is installed on the PCB board and connected to the system board via a board-to-board connection. Inspect the board-to-board connection status.

![](../_assets/3-Safety-io/E02280/그림2_en.png)<br>
Figure 2 Hi6-T Controller

### (2) Inspect the MC1 Magnetic Contactor

For Hi6-N controller, check if the MC1 magnetic contactor inside the power module operates normally.

![](../_assets/3-Safety-io/E02280/그림3.png)<br>
Figure 3 Hi6-N Controller (MC1 Magnetic Contactor installed inside the power module)

For Hi6-T controller, check whether the MC2 magnetic contactor on the Back Plane board operates normally.

![](../_assets/3-Safety-io/E02280/그림4.png)<br>
Figure 4 Hi6-T Controller (MC2 Magnetic Contactor installed on the Back Plane board)

### (3) Inspect the Power Board

For Hi6-N controller, inspect or replace the power board and related cable wiring that relay signals between the system board and the magnetic contactor, as issues may occur there.

![](../_assets/3-Safety-io/E02280/그림5.png)<br>
Figure 5 Hi6-N Controller (Power board installed inside the power module)

For Hi6-T controller, this wiring does not exist, so no action is required.

### (4) Inspect the System Board

If there are no issues in the monitoring system, magnetic contactors, or power board, replace the system board.

[__SOURCE](3-safety-board-part/E02281.md)
# 3.14. E02281. MC1 Magnetic Contactor Fault/Detection Error During Servo ON

### 1. Overview

During Servo ON, the MC1 magnetic contactor is abnormally turned OFF.

### 2. Causes and Inspection Methods

{% hint style="info" %}

(1) Check the monitoring system.<br>
(2) Inspect the MC1 magnetic contactor.<br>
(3) Inspect the power board.<br>
(4) Inspect the system board.<br>

{% endhint %}

For detailed inspection procedures, refer to “E02280 MC1 Magnetic Contactor Fault/Detection Error During Servo ON.”

[__SOURCE](3-safety-board-part/E02301.md)
# 3.15. E2301. CPUERR Signal Mismatch (H6COM Task Error)

### 1. Overview

A CPUERR signal mismatch (H6COM task error) has occurred. This alarm can occur if the execution time or cycle of certain tasks in H6COM-T exceeds the normal range. In this case, the system cannot turn the motor ON.

### 2. Causes and Inspection

{% hint style="info" %}

(1) If the main task cycle is not within the normal range:
* The latest version of the software is not installed.
* Communication issues with external devices affect the system.

(2) If there is an issue with the safety board (BD632):
* Inspect the safety board (BD632).

{% endhint %}

### (1) If the main task cycle is not within the normal range

#### [When the latest version of the software is not installed]

Go to the TP screen: Service -> System Diagnosis -> System Version, and check whether the currently installed version is the latest software version.

![](../_assets/3-Safety-io/E02301/그림1.png)<br>
![](../_assets/3-Safety-io/E02301/그림2.png)<br>
![](../_assets/3-Safety-io/E02301/그림3.png)<br>
![](../_assets/3-Safety-io/E02301/그림4.png)<br>

#### [When communication issues with external equipment affect the system]

The system may be affected depending on whether communication with external equipment is active or not. In this case, compare the task execution time of `/tIOMain0` with communication enabled and disabled.

If the maximum execution time exceeds 10,000 usec, consult with the software development team regarding usage conditions.

#### [How to check task execution time]
Go to: Window Adjustment -> Split (Top/Bottom) -> Select the lower window -> Press the Select button -> Choose Task Monitor

![](../_assets/3-Safety-io/E02301/그림5.png)<br>
![](../_assets/3-Safety-io/E02301/그림6.png)<br>
![](../_assets/3-Safety-io/E02301/그림7.png)<br>
![](../_assets/3-Safety-io/E02301/그림8.png)<br>

Press the initialization button and, after a certain time (approximately 10 minutes), check the maximum execution time.

### (2) If there is an issue with the safety board (BD632)

#### [How to check the safety board (BD632)]
![](../_assets/3-Safety-io/E02301/그림9_en.png)<br>

1) **How to check IO power status**  
A. Check whether the two LEDs in the figure above are lit green.  
B. If the IO power LED is red or off, check whether the indicated fuse is intact.  
C. If the fuse is blown, replace it.

2) **Check if IO power is unstable when the motor is ON**  
A. Check whether the IO power LED is green when the motor is ON.  
B. If the LED turns red or goes off the moment the motor turns ON, the IO power is unstable during motor operation.

3) **If IO power is unstable**  
A. Check the connection status of the IO power connector.  
B. Inspect the IO power cable.  
C. Check the grounding status of the safety board (BD632), including the grounding cable and grounding terminal connections.


[__SOURCE](3-safety-board-part/E64002.md)
# 3.16. E64002 H6COM-T Heartbeat Update Stopped Error

### 1. Overview

The safety board (BD632) did not receive a refreshed Heartbeat from the main control module (H6COM-T). In this case, the system will not allow motor ON.

### 2. Causes and Checks

{% hint style="info" %}

(1) If the main task cycle is out of the normal range:  
* The latest version of the software is not installed.  
* Communication issues with external equipment are affecting the system.

(2) Check the wiring condition of the inter-board communication cable.

(3) Inspect the safety board (BD632).

{% endhint %}

### (1) If the main task cycle is out of the normal range

#### [If the latest version of SW is not installed]

On the TP screen, navigate to **Service -> System Diagnosis -> System Version** and check whether the currently installed version is the latest software version.

![](../_assets/3-Safety-io/E64002/그림1.png)<br>
![](../_assets/3-Safety-io/E64002/그림2.png)<br>
![](../_assets/3-Safety-io/E64002/그림3.png)<br>
![](../_assets/3-Safety-io/E64002/그림4.png)<br>

#### [If communication issues with external devices affect the system]

System performance may be affected depending on whether communication with external devices is enabled. In this case, compare the task execution time of **/tIOMain0** depending on the communication status with external devices.

If the maximum execution time exceeds 10,000 usec, consult the robot software development team regarding the operating conditions.

#### [How to check task execution time]
Navigate to **창조정 -> Split (Up/Down) -> select the lower window -> Press the Select button -> Task Monitor**.

![](../_assets/3-Safety-io/E64002/그림5.png)<br>
![](../_assets/3-Safety-io/E64002/그림6.png)<br>
![](../_assets/3-Safety-io/E64002/그림7.png)<br>

Press the **Initialize** button, wait for a certain period (approximately 10 minutes), and then check the maximum execution time.

![](../_assets/3-Safety-io/E64002/그림8.png)<br>

### (2) Check the wiring status of inter-board communication cables

#### [Check the Ethernet cable connections between each module (Main Control Module (H6COM-T), Servo Board (BD640), Safety Board (BD632))]

![](../_assets/3-Safety-io/E64002/그림9_en.png)<br>

1) Items to Inspect  
A. Ethernet cable between Main Control Module (H6COM-T) ↔ Servo Board (BD640)  
B. Ethernet cable between Servo Board (BD640) ↔ Safety Board (BD632)  

2) Inspection Checklist  
A. Verify that both connectors at each end of the cable are securely connected  
B. Visually check the cable for breaks, crimp damage, kinks, or other physical damage  
C. Inspect connector pins (terminals) for rust, contamination, or bending  

3) Inspection Procedure  
A. With power OFF, disconnect and reconnect the cables  
B. Ensure a full click ('snap') is heard when reinserting the connectors  
C. If necessary, replace the cable with a spare and retry  
D. Recheck the connection sequence and confirm the correct LAN port is used  

4) Additional Checks  
A. Check the Link/Act LED status on the Servo Board (BD640) and Safety Board (BD632)  
- Normal: Green (left) blinking, Yellow (right) ON  
- Abnormal: Green (left) & Yellow (right) OFF or continuously ON  

![](../_assets/3-Safety-io/E64002/그림10.png)<br>

B. If disconnections occur repeatedly, consider the possibility of internal cable break → replace the cable  
C. Inspect for possible damage to the Ethernet connector (PCB terminal)

### (3) Inspect the Safety Board (BD632)

#### [How to Inspect the Safety Board (BD632)]

![](../_assets/3-Safety-io/E64002/그림11_en.png)<br>

1) Check the power status  
A. Verify that the two power LEDs shown in the figure are lit green  
B. If the power LED is red or OFF, check whether the indicated fuses are intact  
C. If a fuse is blown, replace the fuse  

2) Verify if the power is unstable when the motor is ON  
A. Check that the power LED is green when the motor is ON  
B. If the LED turns red or OFF when the motor starts, the power is unstable during motor ON

3) If the power is unstable  
A. Check the power connector for proper seating  
B. Inspect the power cable  
C. Check the grounding of the Safety Board (BD632) – verify grounding cable and terminal connections  

4) Verify that the Safety Board boots normally  
A. After the main control module (H6COM-T) has fully booted (approximately 50 seconds after power ON), two 7-segment displays should show 'S'  
B. The ECAT LED should not show any red blinking or steady ON  

5) If all checks from 1) to 4) show no abnormalities but communication issues persist, replace the Safety Board (BD632)
`

[__SOURCE](3-safety-board-part/E64003.md)
# 3.17. E64003 Servo Board (BD640) Status Input Error

### 1. Overview

The Safety Board (BD632) detected an abnormal input from the servo board (BD640) status signals. Inspection of the servo board (BD640) is required.

### 2. Causes and Checks

{% hint style="info" %}

(1) Check the CNSV connector and wiring for proper condition.<br>
(2) Inspect the servo board (BD640).<br>
(3) Inspect the Safety Board (BD632).<br>

{% endhint %}

(1) Check the CNSV connector and wiring status.  
* How to inspect the connection with the servo board (BD640):

![](../_assets/3-Safety-io/E64003/그림1.png)<br>

1) Verify the LED blinking status (observe after H6COM-T is fully booted, ~50 seconds after power on).  
   - Two LEDs should blink at approximately 0.5-second intervals for normal operation.  
2) Check the CNSV connector seating.  
3) Inspect the CNSV cable for damage or loose connections.  
4) Check the Safety Board (BD632) grounding status (ground cable and terminal connections).

(2) Inspect the servo board (BD640).  
* How to inspect the servo board (BD640):

![](../_assets/3-Safety-io/E64003/그림2.png)<br>

1) Observe the FND status values changing sequentially (observe after H6COM-T is fully booted, ~50 seconds after power on).  
   - If the FND does not operate: verify 24V power supply and replace the board if necessary.  
   - FND value P.001: initialization in progress. If it does not change to P.002, check EtherCAT connection, BD632 boot status, and main computer boot status.  
   - FND value P.002: normal operation.
2) If servo board errors persist even after initialization, check the version compatibility between the Main COM, Servo Board (BD640), and Safety Board (BD632).

3) If errors continue despite version compatibility being correct, replace the Servo Board (BD640).

(3) Check the Safety Board (BD632).

* How to inspect the Safety Board (BD632)
![](../_assets/3-Safety-io/E64003/그림3_en.png)

1) Verify the IO power status:  
A. Confirm that the two LEDs shown in the figure are lit green.  
B. If the IO power LEDs are red or off, check the fuses indicated to ensure they are intact.  
C. If a fuse is blown, replace it.

2) Check if the IO power is unstable when the motor is ON:  
A. Confirm that the IO power LED is green during motor ON.  
B. If the LED turns red or goes off at the moment the motor is ON, the IO power is unstable during motor operation.

3) If the IO power is unstable:  
A. Check the connection status of the IO power connector.  
B. Inspect the IO power cable.  
C. Verify the grounding of the Safety Board (BD632), including grounding cables and terminal connections.

[__SOURCE](3-safety-board-part/E64035.md)
# 3.18. E64035. Safety Module Status Output (SFST) Mismatch (Safety Chain 2 OFF)

### 1. Overview

A mismatch in the safety module status output (SFST) has occurred. Inspection of the Safety Board (BD632) is required.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the Safety Board (BD632).

{% endhint %}

### (1)	Check the Safety Board (BD632)

#### [How to inspect the Safety Board (BD632)]
![](../_assets/3-Safety-io/E64035/그림1_en.png)<br>

1)	Check the IO power status<br>
A.	Verify that the two LEDs shown in the figure above are lit green.<br>
B.	If the IO power LED is red or off, check that the indicated fuses are intact.<br>
C.	If a fuse is blown, replace it.<br>

2)	Check if the IO power is unstable during motor ON<br>
A.	Verify that the IO power LED is green when the motor is ON.<br>
B.	If the LED turns red or goes off at the moment the motor turns ON, the IO power is unstable during motor ON.<br>

3)	If the IO power is unstable<br>
A.	Check the connection of the IO power connector.<br>
B.	Inspect the IO power cable.<br>
C.	Check the grounding of the Safety Board (BD632) (ground cable and ground terminal connection status).<br>
`

[__SOURCE](4-servo-board-part/README.md)
# 4. Servo Board
[__SOURCE](4-servo-board-part/E02450.md)
# 4.1. E02450. (O Axis) No Encoder Response

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically. This error occurs when the data received from the encoder violates the specified communication protocols.

This error can be caused by failure of components transmitting/receiving encoder data, or issues with wiring or encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.

(2)	Inspect the encoder wiring.

(3)	Perform a replacement test of the servo board.

(4)	Perform a replacement test of the motor (encoder).

(5)	Inspect the communication status of the wiring after completing the measures.

{% endhint %}

(1)	Check the encoder supply voltage.<br>
The power voltage supplied to the encoder must be within the range of 5V±5% (4.75V ~ 5.25V) at the encoder-side connector. If the voltage at the encoder-side connector drops below 4.75V, the encoder may not operate normally, leading to the possibility of the above error.

Please measure the voltage of pins (3-4) on the encoder-side connector.

![](../_assets/4.서보보드/encoder_connector_pin_info_en.png)

    (Figure 4.1 Encoder Connector Pin Information)

If the measured voltage is lower than the reference voltage, adjust the VR1 variable resistor on the servo board (BD640) so that the voltage at the encoder-side connector falls within the reference voltage range.

![](../_assets/4.서보보드/BD640_가변저항.png)

    (Figure 4.2 BD640 Variable Resistor)

(2)	Inspect the encoder wiring.

The sequence for inspecting the encoder wiring is as follows.

1st: Check for poor contact in connectors related to the encoder wiring.

2nd: Check for short circuits in the encoder wiring. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester).

3rd: Perform a replacement test of the encoder wiring.

If the encoder wiring is not disconnected but there are issues such as poor contact of the shield wire, or contact between the encoder signal line and other power lines or the metal part of the robot body, it cannot be detected by a short circuit test, so please perform a wiring replacement test.

* Inspect the internal wiring of the controller.
Inspect the wiring between CNEC1,4 (BD640) connectors and CEC1.

![](../_assets/4.서보보드/hi6N제어기_en.png)

    (Figure 4.3 Hi6-N Controller Encoder Wiring Inspection)

![](../_assets/4.서보보드/Hi6_T15제어기_en.png)

    (Figure 4.4 Hi6-T15 Controller Encoder Wiring Inspection)

* Inspect the wiring between the controller and the robot.
In the case of the Hi6-N controller, inspect the wiring between CNEC1 and CER1. In the case of the Hi6-T15 controller, inspect the wiring between CMEC1 and CMER1.

![](../_assets/4.서보보드/로봇_N제어기_설치구성.png)

    (Figure 4.5 Hi6-N Controller and Robot Basic Installation Configuration Diagram)

![](../_assets/4.서보보드/로봇_T제어기_설치구성.png)

    (Figure 4.6 Hi6-T15 Controller and Robot Basic Installation Configuration Diagram)

![](../_assets/4.서보보드/N제어기_설치구성_상세.png)

    (Figure 4.7 Hi6-N Controller and Robot Basic Installation Configuration Diagram Detail)

![](../_assets/4.서보보드/T제어기_설치구성_상세.png)

    (Figure 4.8 Hi6-N Controller and Robot Basic Installation Configuration Diagram Detail)

* Inspect the internal wiring of the body.
Inspect the wiring between CER1 and the encoder-side connector.
For wiring inspection, please refer to the wiring connection diagram in the robot maintenance manual.

![](../_assets/4.서보보드/로봇기내배선.png)

    (Figure 4.9 Robot Internal Wiring)

(3)	Perform a replacement test of the servo board. 
If the error does not occur after replacing the servo board, the encoder receiving part of the servo board is defective. Please replace the servo board with a normal one.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

    (Figure 4.10 N Controller Servo Board Replacement)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

    (Figure 4.11 T Controller Servo Board Replacement)

(4)	Perform a replacement test of the motor (encoder). 
If the error does not occur after replacing the servo motor, the servo motor is defective. Please replace the servo motor with a normal one. The figure below shows the positions of the motors for each axis of the robot; for other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/로봇_모터_위치.png)

    (Figure 4.12 Robot Axis Motor Positions)

(5)	Inspect the communication status of the wiring after completing the measures.
After the measures for the problematic part are completed, please refer to the "Encoder Communication Failure Count Display Function Manual" to check the communication status.

![](../_assets/4.서보보드/encoder_comm.png)

    (Figure 4.13 Encoder Communication Failure Monitoring)

![](../_assets/4.서보보드/엔코더_통신실패_횟수_en.png)


[__SOURCE](4-servo-board-part/E02451.md)
# 4.2. E02451. (O Axis) Abnormal Number of Encoder Data Received

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the number of data items received from the encoder deviates from the specified value.

If the number of data items received from the encoder is incorrect, it may primarily occur when noise is introduced into the encoder signal line due to wiring issues or problems with the encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring

(2)	Perform a replacement test of the motor (encoder)

(3)	Perform a replacement test of the servo board

(4)	Inspect the communication status of the wiring after completing the measures

{% endhint %}

(1)	Inspect the encoder wiring.

The sequence for inspecting the encoder wiring is as follows.

1st: Check for poor contact in connectors related to the encoder wiring.

2nd: 
Check for short circuits in the encoder wiring. Check the wiring of each phase 1:1 using equipment such as a multimeter (tester).

3rd: Perform a replacement test of the encoder wiring.

If the encoder wiring is not disconnected but there are issues such as poor contact of the shield wire, or contact between the encoder signal line and other power lines or the metal part of the robot body, it cannot be detected by a short circuit test, so please perform a wiring replacement test.

* Inspect the internal wiring of the controller.

    Inspect the wiring between CNEC1,4 (BD640) connectors and CEC1.

    ![](../_assets/4.서보보드/hi6N제어기_en.png)
    
    (Figure 4.14 Hi6-N Controller Encoder Wiring Inspection)

    ![](../_assets/4.서보보드/Hi6_T15제어기_en.png)

    (Figure 4.15 Hi6-T15 Controller Encoder Wiring Inspection)

* Inspect the wiring between the controller and the robot.

    In the case of the Hi6-N controller, inspect the wiring between CNEC1 and CER1. In the case of the Hi6-T15 controller, inspect the wiring between CMEC1 and CMER1.

    ![](../_assets/4.서보보드/로봇_N제어기_설치구성.png)

    (Figure 4.16 Hi6-N Controller and Robot Basic Installation Configuration Diagram)

    ![](../_assets/4.서보보드/로봇_T제어기_설치구성.png)

    (Figure 4.17 Hi6-T Controller and Robot Basic Installation Configuration Diagram)

    ![](../_assets/4.서보보드/N제어기_설치구성_상세.png)

    (Figure 4.18 Hi6-N Controller and Robot Basic Installation Configuration Diagram Detail)

    ![](../_assets/4.서보보드/T제어기_설치구성_상세.png)

    (Figure 4.19 Hi6-T Controller and Robot Basic Installation Configuration Diagram Detail)

* Inspect the internal wiring of the body.

    Inspect the wiring between CER1 and the encoder-side connector.
    For wiring inspection, please refer to the wiring connection diagram in the robot maintenance manual.

    ![](../_assets/4.서보보드/로봇기내배선.png)

    (Figure 4.20 Robot Internal Wiring)

(2)	Perform a replacement test of the motor (encoder). 

If the error does not occur after replacing the servo motor, the servo motor is defective. Please replace the servo motor with a normal one. The figure below shows the positions of the motors for each axis of the robot; for other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/로봇_모터_위치.png)

    (Figure 4.21 Robot Axis Motor Positions)

(3)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, the servo board is defective. Please replace the servo board with a normal one.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

    (Figure 4.22 N Controller Servo Board Replacement)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

    (Figure 4.23 T Controller Servo Board Replacement)
    
(4)	Inspect the communication status of the wiring after completing the measures.

After the measures for the problematic part are completed, please refer to the "Encoder Communication Failure Count Display Function Manual" to check the communication status.

![](../_assets/4.서보보드/encoder_comm.png)

    (Figure 4.24 Encoder Communication Failure Monitoring)

![](../_assets/4.서보보드/엔코더_통신실패_횟수_en.png)


[__SOURCE](4-servo-board-part/E02452.md)
# 4.3. E02452. (O Axis) Encoder End Signal (Ser_End) Not Received

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the signal indicating the end of the data frame (Ser_End) is not received from the encoder.

Failure to receive the signal indicating the end of the data frame from the encoder can primarily occur when noise is introduced into the encoder signal line due to wiring issues or problems with the encoder shield line processing.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring

(2)	Perform a replacement test of the motor (encoder)

(3)	Perform a replacement test of the servo board

(4)	Inspect the communication status of the wiring after completing the measures

{% endhint %}

For detailed inspection methods, please refer to "E02450 (O Axis) No Encoder Response".
[__SOURCE](4-servo-board-part/E02453.md)
# 4.4. E02453. (O Axis) Encoder Data Error (CRC Error Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the CRC value of the data received from the encoder does not match the CRC value calculated by the servo board.

When a CRC error occurs in the data received from the encoder, it can primarily occur when noise is introduced into the encoder signal line due to wiring issues or problems with the encoder shield line processing.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring

(2)	Perform a replacement test of the motor (encoder)

(3)	Perform a replacement test of the servo board

(4)	Inspect the communication status of the wiring after completing the measures

{% endhint %}

For detailed inspection methods, please refer to "E02450 (O Axis) No Encoder Response".

[__SOURCE](4-servo-board-part/E02454.md)
# 4.5. E02454. (O Axis) Encoder Disconnected or Contact Failure (Motor OFF State)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when communication between the encoder and the servo board is unstable or when no signal is received at all.

Cases where communication between the encoder and servo board is unstable or no signal is received at all can primarily occur due to disconnection or poor contact of the encoder cable.

### 2. Cause and Inspection
{% hint style="info" %}

(1)	Check the encoder supply voltage <br>
(2)	Inspect the encoder wiring<br>
(3)	Perform a replacement test of the servo board<br>
(4)	Perform a replacement test of the motor (encoder)<br>
(5)	Inspect the communication status of the wiring after completing the measures<br>

{% endhint %}

For detailed inspection methods, please refer to "E02450 (O Axis) No Encoder Response".
[__SOURCE](4-servo-board-part/E02455.md)
# 4.6. E02455. (O Axis) Abnormal Encoder Data (Irregular Value Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the position value or speed value received from the encoder changes abnormally. 

Cases where the position value or speed value received from the encoder changes abnormally can primarily occur when noise is introduced into the encoder signal line due to wiring issues or problems with the encoder shield line processing.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the encoder wiring

(2)	Perform a replacement test of the motor (encoder)

(3)	Perform a replacement test of the servo board

(4)	Inspect the communication status of the wiring after completing the measures

{% endhint %}

For detailed inspection methods, please refer to "E02450 (O Axis) No Encoder Response".
[__SOURCE](4-servo-board-part/E02459.md)
# 4.7. E02459. (O Axis) Encoder Disconnected or Contact Failure (Motor ON State)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when communication between the encoder and the servo board is unstable or when no signal is received at all.

Cases where communication between the encoder and servo board is unstable or no signal is received at all can primarily occur due to disconnection or poor contact of the encoder cable.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage 

(2)	Inspect the encoder wiring

(3)	Perform a replacement test of the servo board

(4)	Perform a replacement test of the motor (encoder)

(5)	Inspect the communication status of the wiring after completing the measures

{% endhint %}

For detailed inspection methods, please refer to "E02450 (O Axis) No Encoder Response".
[__SOURCE](4-servo-board-part/E02460.md)
# 4.8. E02460. (O Axis) Encoder Internal Rotation Value Error (CE Bit Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when an error occurs in the calculation of the rotation value within the encoder and the CE (Counter Error) bit is set.

This can occur when the data received from the encoder is normal, but the encoder is in an error state (CE) as a result of monitoring its own internal status.
 
CE (Counter Error): Occurs when a position mismatch occurs due to malfunction or failure of 1-turn data when the encoder main power is turned on.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.

(2)	After clearing the serial encoder error, turn the controller power off and then on again.

(3)	If the error persists, perform a replacement test of the motor (encoder). 

{% endhint %}

(1)	Check the encoder supply voltage.<br>
The power voltage supplied to the encoder must be within the range of 5V±5% (4.75V ~ 5.25V) at the encoder-side connector. If the voltage at the encoder-side connector drops below 4.75V, the encoder may not operate normally, which may cause the above error.

Please measure the voltage of pins (3-4) on the encoder-side connector.

![](../_assets/4.서보보드/엔코더_커넥터_핀정보_en.png)

        (Figure 4.25 Encoder Connector Pin Information)

If the measured voltage is lower than the reference voltage, adjust the VR1 variable resistor on the servo board (BD640) so that the encoder-side connector voltage is within the reference voltage.

![](../_assets/4.서보보드/BD640_가변저항.png)

        (Figure 4.26 BD640 Variable Resistor)

(2)	After clearing the serial encoder error, turn the controller power off and then on again.

If the error persists when turning the main power OFF/ON after clearing the error, perform a motor (encoder) replacement test.
The error clearing is executed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Error Reset

![](../_assets/4.서보보드/enc_error_clear.png)

        (Figure 4.27 Serial Encoder Error Reset)

(3)	If the error persists, perform a replacement test of the motor (encoder). 

If the error does not occur after replacing the servo motor, the servo motor is defective. Please replace the servo motor with a normal one. The figure below shows the positions of the motors for each axis of the robot; for other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/로봇_모터_위치.png)

        (Figure 4.28 Robot Axis Motor Positions)
[__SOURCE](4-servo-board-part/E02461.md)
# 4.9. E02461. (O Axis) Encoder Overspeed Error (OS Bit Detected)

### 1. Overview
The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the encoder rotation speed exceeds the allowable range and the OS (OverSpeed) bit is set. This may be an actual overspeed situation or a false detection due to signal abnormality.

This can occur when the data received from the encoder is normal, but the encoder is in an error state (OS) as a result of monitoring its own internal status.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	Inspect the encoder wiring.<br>
(3)	After clearing the serial encoder error, turn the controller power off and then on again.<br>
(4)	If the error persists, perform a replacement test of the motor (encoder). <br>

{% endhint %}

For detailed inspection methods, please refer to "E02460 (O Axis) Encoder Internal Rotation Value Error (CE Bit Detected)".

[__SOURCE](4-servo-board-part/E02462.md)
# 4.10. E02462. (O Axis) Encoder Position Not Initialized (FS Bit Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the encoder has not reached the Full Absolute state and accurate position information has not yet been secured. This may occur immediately after encoder power is applied, due to data initialization failure, or loss of backup information.

This can occur when the data received from the encoder is normal, but the encoder is in an error state (FS) as a result of monitoring its own internal status.

FS (Full Absolute): If this bit is 0, it means the position data has not been initialized or the backup information is incomplete. If this bit is 1, it indicates that the encoder's internal data is complete and in a normal state.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	After clearing the serial encoder error, turn the controller power off and then on again.<br>
(3)	If the error persists, perform a replacement test of the motor (encoder). <br>

{% endhint %}

For detailed inspection methods, please refer to "E02460 (O Axis) Encoder Internal Rotation Value Error (CE Bit Detected)".
[__SOURCE](4-servo-board-part/E02463.md)
# 4.11. E02463. (O Axis) Encoder Multiturn Storage Error (ME Bit Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the multiturn (number of rotations) data is not stored normally due to causes such as battery backup failure, internal storage circuit error, or unexpected power interruption during power-on, and the ME bit is set.

This can occur when the data received from the encoder is normal, but the encoder is in an error state (ME) as a result of monitoring its own internal status.

### 2. Cause and Inspection
{% hint style="info" %}

(1)	Check the encoder supply voltage.<br>
(2)	After clearing the serial encoder error, turn the controller power off and then on again.<br>
(3)	If the error persists, perform a replacement test of the motor (encoder). <br>

{% endhint %}

For detailed inspection methods, please refer to "E02460 (O Axis) Encoder Internal Rotation Value Error (CE Bit Detected)".

[__SOURCE](4-servo-board-part/E02464.md)
# 4.12. E02464. (O Axis) Encoder Battery Error (BE Bit Detected)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the battery voltage connected to the encoder drops below the reference value or a connection problem occurs, causing the BE (Battery Error) bit to be set.

This can occur when the data received from the encoder is normal, but the encoder is in an error state (BE) as a result of monitoring its own internal status.

BE (Battery Error): Occurs when the external battery voltage drops below 3.1V while the encoder main power is OFF.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	After clearing the serial encoder error, turn the controller power off and then on again.

(2)	Check the encoder backup battery voltage.

(3)	Inspect the encoder battery wiring connection.

(4)	Perform a replacement test of the motor (encoder). 

{% endhint %}

(1)	After clearing the serial encoder error, turn the controller power off and then on again.

If the error persists when turning the main power OFF/ON after clearing the error, perform a motor (encoder) replacement test.
The error clearing is executed in the menu below.
        
        System -> 5. Initialization -> 4. Serial Encoder Reset - Error Reset

![](../_assets/4.서보보드/enc_error_clear.png)

                        (Figure 4.29 Encoder Error Reset)

(2)	Check the encoder battery voltage. <br>
The battery for the encoder is 3.6V. If this voltage drops to 3.0V–3.2V, "W0104 (Axis O) Encoder Battery Voltage Low" is displayed. When this warning occurs, the encoder battery must be replaced. The encoder battery must be replaced while the controller power is ON. If the battery is replaced with a normal one in this state, the robot can continue to be used without problems.

If the encoder battery voltage reaches 2.5V–3.0V after the replacement period has passed, the error "E2470 (Axis O) Encoder Error: Encoder Reset Required" occurs when the controller power is turned ON. When this error occurs, the encoder's position data has already been lost. After replacing the encoder battery and resetting the encoder, you must move the robot to the reference posture using manual operation in the axis coordinate system and re-perform encoder calibration for the corresponding axis.

![](../_assets/4.서보보드/배터리_교환위치.png)

                         (Figure 4.30 Encoder Battery Replacement Location)

The encoder reset is executed in the menu below.

        System -> 5. Initialization -> 4. Serial Encoder Reset - Encoder Reset

![](../_assets/4.서보보드/enc_reset.png)

                         (Figure 4.31 Encoder Reset)

(3)	Inspect the encoder battery wiring connection. <br>
Check the condition of the battery wiring connected from the encoder battery location to the motor.


(4)	Perform a replacement test of the motor (encoder). <br>
If the error persists when turning the main power OFF/ON after resetting the error, perform a motor (encoder) replacement test. If the error does not occur after replacement, the servo motor is defective. Please replace the servo motor with a normal one. The figure below shows the positions of the motors for each axis of the robot; for other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                        (Figure 4.32 Robot Axis Motor Positions)


[__SOURCE](4-servo-board-part/E02470.md)
# 4.13. E02470. (O Axis) Encoder Error: Reset Required

### 1. Overview

In order for the encoder to preserve the motor's position data, power must be supplied to the encoder at all times. 

Power to the encoder is supplied either by keeping the controller power ON or by the encoder backup battery. If the controller power is turned OFF while the encoder backup battery is discharged, the encoder loses its position data, resulting in an error. 

Similarly, when a motor is replaced, the same error occurs because the encoder of the new motor was already in a state where no power was being supplied.
Resetting the encoder changes the reference position data for the corresponding axis; therefore, you must move the robot to the reference posture using manual operation in the axis coordinate system and re-perform encoder calibration for the corresponding axis.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check the encoder battery voltage.<br>
(2)	Inspect the encoder battery wiring connection.<br>
(3)	Perform a replacement test of the motor.<br>
(4)	After resetting the encoder, encoder calibration must be re-performed at the robot's reference position.<br>

{% endhint %}

(1)	Check the encoder battery voltage.<br> 
The battery for the encoder is 3.6V. If this voltage drops to 3.0V–3.2V, "W0104 (Axis O) Encoder Battery Voltage Low" is displayed. When this warning occurs, the encoder battery must be replaced. The encoder battery must be replaced while the controller power is ON. If the battery is replaced with a normal one in this state, the robot can continue to be used without problems.

If the encoder battery voltage drops to 2.5V–3.0V after the replacement period has passed, the error "E2470 (Axis O) Encoder Error: Encoder Reset Required" occurs. When this error occurs, the encoder's position data has already been lost. After replacing the encoder battery and resetting the encoder, you must move the robot to the reference posture using manual operation in the axis coordinate system and re-perform encoder calibration for the corresponding axis.

![](../_assets/4.서보보드/배터리_교환위치.png)

    (Figure 4.34 Encoder Battery Replacement Location)

The encoder reset is executed in the menu below.

    System -> 5. Initialization -> 4. Serial Encoder Reset

![](../_assets/4.서보보드/enc_reset.png)

    (Figure 4.35 Serial Encoder Reset)

(2) Inspect the encoder battery wiring connection. 

Check the condition of the battery wiring connected from the encoder battery location to the motor.

(3) Perform a replacement test of the motor.

If the problem is not resolved by the above measures, there is a high possibility that the encoder itself is defective. Perform a replacement test of the motor.

    

[__SOURCE](4-servo-board-part/E02630.md)
# 4.14. E02630. (O Axis) position deviation exceeded

### 1. Overview
This error occurs when the position deviation exceeds the set value during robot operation. While the robot is operating under servo control, if the difference between the commanded movement position and the actual position is too large, the servo board detects this as an error and stops the robot.

### 2. Cause and Inspection
{% hint style="info" %}

(1)	Check if the axis where the error occurred has mechanical interference with other equipment.<br>
(2)	Verify that the robot model is configured correctly.<br>
(3)	Verify that the brake release is operating normally.<br>
    - Inspect for abnormalities in individual axis brake release.<br>
    - Inspect for abnormalities in brake power supply.<br>
(4)	Inspect the wiring condition.<br>
(5)	Check if the rated load is being exceeded.<br>
(6)	Verify the position deviation setting level.<br>
(7)	Check the versions of the servo board (BD640) and the main COM.<br>
(8)	Replace other components.<br>

{% endhint %}

(1)	Check if the axis where the error occurred has mechanical interference with other equipment.

This error can occur if there is mechanical interference or a collision with the robot. If the robot is outside the restricted area, move it to a safe area using manual operation.

(2)	Verify that the robot model is configured correctly.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.60 Checking Robot Model on TP)
    Verify that the robot model registered on the TP (Teach Pendant) screen matches the actually installed robot.

(3)	Verify that the brake release is operating normally.

There may be a problem with the brake release function of the corresponding axis or an abnormality in the brake release voltage.
 * Inspect for abnormalities in individual axis brake release.

Verify the operation of the brake release function for the corresponding axis using the Axis Lock function.
After performing an Axis Lock on all axes except the one you wish to check, repeatedly turn the motor on/off and listen for a "click" sound of the brake releasing from the motor in the mechanical unit.

The procedure for using the Axis Lock function is as follows:
    
        System -> 5. Initialization -> 9. Axis Lock Setting -> OK -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)

                    (Figure 4.61 Axis Lock Setting Screen 1)

![](../_assets/4.서보보드/axis_lock2.png)

                    (Figure 4.62 Axis Lock Setting Screen 2)

![](../_assets/4.서보보드/axis_lock3.png)

                    (Figure 4.63 Axis Lock Setting Screen 3)

   If the brake for the corresponding axis does not release, the brake output status of the servo board must be checked. Remove the brake wiring (CNB1, CNB7, CNB8 connectors) and output the brake voltage. Measure whether the brake voltage for the corresponding axis is output at 20V or higher from the CNB1, CNB7, or CNB8 connectors. If there is an axis where the voltage output is below 20V, the servo board (BD640) is defective and must be replaced.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (Figure 4.64 Pin Assignment of CNB1, CNB7, and CNB8 Connectors)

 * Inspect for abnormalities in brake power supply

The inspection sequence for the brake power wiring is as follows:

Step 1: Inspect the connectors related to the brake power wiring for any poor contact.

Step 2: Check the brake power wiring for short circuits. Perform a 1:1 check using equipment such as a multimeter (tester).

    * Inspect the internal wiring of the power electronic module. 
      The Hi6-T15 controller is not applicable as it does not have a power electronic module.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (Figure 4.65 Electronic Module and Electronic Board)

 * Inspect the servo board (BD640).

If the power electronic module is normal, measure the brake power (DC24V) on the servo board. The measured value at the test point (PAD24V0BK1) in the red area of the figure below must be DC24V or higher to be considered normal. If it is less than 20V, there is an abnormality in the power supply unit that generates the brake power. Replace the electronic module.

![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (Figure 4.66 Servo Board Brake Power)

(4)	Inspect the wiring condition.

Verify that the motor wiring (U, V, W phases) is connected correctly.
Also, check if the motor wiring is shorted to other wiring or the ground wire (FG).

(5)	Check if the rated load is being exceeded.

If the total weight, including the workpiece, exceeds the rated load, adjust the load to within the rated capacity by referring to the robot's specification manual.

(6)	Position deviation setting level error

If the position deviation setting value is smaller than the following measured maximum value, increase the setting value.

             Maximum measured position deviation after operating for a few cycles x 1.5
![](../_assets/4.서보보드/pos_dev.png)

                (Figure 4.67 Monitoring screen for maximum measured position deviation)

![](../_assets/4.서보보드/pos_dev2.png)

                (Figure 4.68 Position deviation setting change screen)

(7)	Check the versions of the servo board (BD640) and the main COM.

This error can occur if the compatibility between the servo board (BD640) and the main COM version is broken. Especially in cases where a module has been replaced, perform a version upgrade to match the version of each module with the current main COM version. The version of each module can be checked at the following path.

    Service -> 7. System Diagnosis -> 1. System Version

![](../_assets/4.서보보드/version.png)

                (Figure 4.69 Version check window for each module on TP)

(8)	Replace other components.

Check if the error occurs by replacing components in the following order: Servo Board (BD640) → Servo Drive Unit → Power Electronic Module → Motor.

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                (Figure 4.70 N Controller Motor and Drive Module)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                (Figure 4.71 T Controller Motor and Drive Module)




[__SOURCE](4-servo-board-part/E02631.md)
# 4.15. E02631. (O Axis) Speed-Based Position Deviation Excess

### 1. Overview

The position deviation occurring during jog operation or low-speed operation is larger than the set value. While the robot is operating under servo control, if the difference between the commanded movement position and the actual position is too large, the servo board detects an error during servo calculation and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the axis where the error occurred has mechanical interference with other equipment.

(2)	Verify that the brake release is operating normally.
    * Inspect for abnormalities in individual axis brake release.
    * Inspect for abnormalities in brake power supply.

(3)	Inspect the wiring condition.

(4)	Check if the rated load is being exceeded.

(5)	Verify the position deviation setting level.

(6)	Check the versions of the servo board (BD640) and the main COM. 

(7)	Replace other components.

{% endhint %}

For detailed inspection methods, please refer to "E02630 (Axis O) position deviation exceeded."
[__SOURCE](4-servo-board-part/E02632.md)
# 4.16. E02632. (O Axis) position deviation exceeded (brake voltage lowered)

### 1. Overview

The position deviation is larger than the set value. While the robot is operating under servo control, if the difference between the commanded movement position and the actual position is too large, the servo board detects an error during servo calculation and stops the robot.
This error occurs when a drop in brake voltage is detected while the position deviation is large.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the brake release is operating normally.<br>
    * Inspect for abnormalities in individual axis brake release<br>
    * Inspect for abnormalities in brake power supply

{% endhint %}

(1)	Verify that the brake release is operating normally.

There may be a problem with the brake release function of the corresponding axis or an abnormality in the brake release voltage.
 * Inspect for abnormalities in individual axis brake release

    Verify the operation of the brake release function for the corresponding axis using the Axis Lock function.
After performing an Axis Lock on all axes except the one you wish to check, repeatedly turn the motor on/off and listen for a "click" sound of the brake releasing from the motor in the mechanical unit.

   The procedure for using the Axis Lock function is as follows:
        
        System -> 5. Initialization -> 9. Axis Lock Setting -> OK -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)

                    (Figure 4.71 Axis Lock Setting Screen 1)

![](../_assets/4.서보보드/axis_lock2.png)

                    (Figure 4.72 Axis Lock Setting Screen 2)

![](../_assets/4.서보보드/axis_lock3.png)

                    (Figure 4.73 Axis Lock Setting Screen 3)

If the brake for the corresponding axis does not release, the brake output status of the servo board must be checked. Remove the brake wiring (CNB1, CNB7, CNB8 connectors) and output the brake voltage. Measure whether the brake voltage for the corresponding axis is output at 20V or higher from the CNB1, CNB7, or CNB8 connectors. If there is an axis where the voltage output is below 20V, the servo board (BD640) is defective and must be replaced.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (Figure 4.74 Pin Assignment of CNB1, CNB7, and CNB8 Connectors)

 * Inspect for abnormalities in brake power supply

The inspection sequence for the brake power wiring is as follows:

Step 1: Inspect the connectors related to the brake power wiring for any poor contact.

Step 2: Check the brake power wiring for short circuits. Perform a 1:1 check using equipment such as a multimeter (tester).

    * Inspect the internal wiring of the power electronic module. 
      The Hi6-T15 controller is not applicable as it does not have a power electronic module.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (Figure 4.75 Electronic Module and Electronic Board)

 * Inspect the servo board (BD640).

If the power electronic module is normal, measure the brake power (DC24V) on the servo board. The measured value at the test point (PAD24V0BK1) in the red area of the figure below must be DC24V or higher to be considered normal. If it is less than 20V, there is an abnormality in the power supply unit that generates the brake power. Replace the electronic module.

![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (Figure 4.76 Servo Board Brake Power)

    

[__SOURCE](4-servo-board-part/E02633.md)
# 4.17. E02633. (O Axis) position deviation exceeded (load estimation not executed)

### 1. Overview
The position deviation is larger than the set value. While the robot is operating under servo control, if the difference between the commanded movement position and the actual position is too large, the servo board detects an error during servo calculation and stops the robot.
This error occurs when the position deviation is large and load estimation has not been performed.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Perform load estimation and check if the error recurs.

(2)	Verify that the robot model is configured correctly.

{% endhint %}

(1)	Perform load estimation and check if the error recurs.

While using a measuring instrument is the most accurate way to verify the load, if that is not feasible, you can use the load estimation function among the controller features. The load estimation function can only estimate the tool installed at the end of the robot.

The load estimation procedure is as follows:
 * Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation

![](../_assets/4.서보보드/estimation1.png)

                    (Figure 4.77 Load Estimation 1)

![](../_assets/4.서보보드/estimation2.png)

                    (Figure 4.78 Load Estimation 2)

![](../_assets/4.서보보드/estimation3.png)

                    (Figure 4.79 Load Estimation 3)

 * Use the load estimation function to select the tool number to save after estimation.

![](../_assets/4.서보보드/estimation4.png)

                    (Figure 4.80 Load Estimation 4)

 * Click "Normal Operation" to perform the task.

    Press the Motor On switch, hold the deadman switch, and then click "Normal Operation."

![](../_assets/4.서보보드/estimation5.png)

                    (Figure 4.81 Load Estimation 5)

* Once the load estimation operation is complete, the estimated results will be displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)

                    (Figure 4.82 Load Estimation 6)

(2)	Verify that the robot model is configured correctly.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.83 Checking Robot Model)

    Verify that the robot model registered on the TP screen matches the actually installed robot.

    
[__SOURCE](4-servo-board-part/E02634.md)
# 4.18. E02634. (O Axis) Position Deviation Excess (Increased Friction at Low Temperature)

### 1. Overview

The position (velocity) deviation is larger than the set value. While the robot is operating under servo control, if the difference between the commanded movement position and the actual position is too large, the servo board detects an error during servo calculation and stops the robot.
This error occurs when the position deviation is large and the encoder temperature is low.
Normally, at low temperatures (encoder at 5°C or below), the friction component increases due to the viscosity of the grease, requiring additional torque compared to normal conditions. Therefore, operating the robot at high speeds may trigger this error.

### 2. Cause and Inspection
{% hint style="info" %}

(1)	Operate the robot at low speed (playback speed of 30% or less) until the encoder temperature reaches a normal level (approximately 15°C or higher), then restart at normal speed.<br>
(2)	Verify that the robot model is configured correctly.<br>

{% endhint %}

(1)	Operate the robot at low speed (playback speed of 30% or less) until the encoder temperature reaches a normal level (approximately 15°C or higher), then restart at normal speed.

![](../_assets/4.서보보드/enc_tmp2.png)

                    (Figure 4.84 Encoder Temperature Check Screen)


(2)	Verify that the robot model is configured correctly.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.85 Checking Robot Model)

 Verify that the robot model registered on the TP screen matches the actually installed robot.
[__SOURCE](4-servo-board-part/E02650.md)
# 4.19. E02650. (O Axis) Motor Overload

### 1. Overview

The motor or drive unit is operating excessively. If the motor or drive unit operates more strainfully than the set value, the servo board detects an error and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the load is installed within the robot's rated capacity.

(2)	Check for any collision factors during robot operation.

(3)	Verify that the axis brakes are operating normally.

(4)	Inspect the connection status of motor cables and connectors.

(5)	Replace the servo board to check for abnormalities.

(6)	Inspect whether the drive unit is operating normally.

{% endhint %}

(1)	Check if the load is installed within the robot's rated capacity.

Verify that the load installed is within the robot's maximum specifications. If the specifications are exceeded, an error may occur. (In this context, "load" includes not only the tool installed at the end of the robot but also cables and all other parts attached to the robot mechanism.)

While using a measuring instrument is the most accurate way to verify the load, if that is not feasible, you can use the load estimation function among the controller features. The load estimation function can only estimate the tool installed at the end of the robot.

The load estimation procedure is as follows:

* Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation

![](../_assets/4.서보보드/estimation1.png)

                    (Figure 4.86 Load Estimation 1)

![](../_assets/4.서보보드/estimation2.png)

                    (Figure 4.87 Load Estimation 2)

![](../_assets/4.서보보드/estimation3.png)

                    (Figure 4.88 Load Estimation 3)

 * Use the load estimation function to select the tool number to save after estimation.

![](../_assets/4.서보보드/estimation4.png)

                    (Figure 4.89 Load Estimation 4)

* Click "Normal Operation" to perform the task.

    Press the Motor On switch, hold the deadman switch, and then click "Normal Operation."

![](../_assets/4.서보보드/estimation5.png)

                    (Figure 4.90 Load Estimation 5)

* Once the load estimation operation is complete, the estimated results will be displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)

                    (Figure 4.91 Load Estimation 6)

(2)	Check for any collision factors during robot operation.

Check if there are any parts in the robot's work area that interfere or collide with the robot. If interference occurs between the robot and other mechanical structures, an error may be generated. In this case, modify the work program to prevent interference from occurring.

(3) Verify that the brake release is operating normally.

There may be a problem with the brake release function of the corresponding axis or an abnormality in the brake release voltage.
 * Inspect for abnormalities in individual axis brake release.

    Verify the operation of the brake release function for the corresponding axis using the Axis Lock function.
After performing an Axis Lock on all axes except the one you wish to check, repeatedly turn the motor on/off and listen for a "click" sound of the brake releasing from the motor in the mechanical unit.

    The procedure for using the Axis Lock function is as follows:
        System -> 5. Initialization -> 9. Axis Lock Setting -> OK -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)

                    (Figure 4.92 Axis Lock Setting Screen 1)

![](../_assets/4.서보보드/axis_lock2.png)

                    (Figure 4.93 Axis Lock Setting Screen 2)

![](../_assets/4.서보보드/axis_lock3.png)

                    (Figure 4.94 Axis Lock Setting Screen 3)

 If the brake for the corresponding axis does not release, the brake output status of the servo board must be checked. Remove the brake wiring (CNB1, CNB7, CNB8 connectors) and output the brake voltage. Measure whether the brake voltage for the corresponding axis is output at 20V or higher from the CNB1, CNB7, or CNB8 connectors. If there is an axis where the voltage output is below 20V, the servo board (BD640) is defective and must be replaced.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (Figure 4.95 Pin Assignment of CNB1, CNB7, and CNB8 Connectors)

 * Inspect for abnormalities in brake power supply

The inspection sequence for the brake power wiring is as follows:

Step 1: Inspect the connectors related to the brake power wiring for any poor contact.

Step 2: Check the brake power wiring for short circuits. Perform a 1:1 check using equipment such as a multimeter (tester).

    * Inspect the internal wiring of the power electronic module. 
      The Hi6-T15 controller is not applicable as it does not have a power electronic module.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (Figure 4.96 Electronic Module and Electronic Board)

 * Inspect the servo board (BD640).

If the power electronic module is normal, measure the brake power (DC24V) on the servo board. The measured value at the test point (PAD24V0BK1) in the red area of the figure below must be DC24V or higher to be considered normal. If it is less than 20V, there is an abnormality in the power supply unit that generates the brake power. Replace the electronic module.

    ![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (Figure 4.97 Servo Board Brake Power)

(4)	Inspect the connection status of motor cables and connectors.
 
 * Inspect the internal wiring of the controller.
 * Inspect the wiring between the controller and the robot.
 * Inspect the internal wiring of the robot.

(5) Replace the servo board to check for abnormalities.

An error may occur if there is an abnormality in the servo board. Replace the board to verify.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (Figure 4.98 Replacing Servo Board for N Controller)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (Figure 4.99 Replacing Servo Board for T Controller)

(6)	Verify that the drive unit is operating normally.

Check whether the drive unit (motor, reducer) of the corresponding axis is operating normally.

![](../_assets/4.서보보드/축구동부_en.png)

                    (Figure 4.100 Verifying Normal Operation of the Drive Unit)
[__SOURCE](4-servo-board-part/E02651.md)
# 4.20. E02651. (O Axis) Motor Overload (Brake Voltage Drop)

### 1. Overview

The motor or drive unit is operating excessively. If the motor or drive unit operates more strainfully than the set value, the servo board detects an error and stops the robot.
This error occurs when a drop in brake voltage is detected while in an overload state.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the brake release is operating normally.

* Inspect for abnormalities in individual axis brake release
* Inspect for abnormalities in brake power supply

{% endhint %}

(1)	Verify that the brake release is operating normally.

There may be a problem with the brake release function of the corresponding axis or an abnormality in the brake release voltage.
 * Inspect for abnormalities in individual axis brake release.

    Verify the operation of the brake release function for the corresponding axis using the Axis Lock function.
After performing an Axis Lock on all axes except the one you wish to check, repeatedly turn the motor on/off and listen for a "click" sound of the brake releasing from the motor in the mechanical unit.

    The procedure for using the Axis Lock function is as follows:

        System -> 5. Initialization -> 9. Axis Lock Setting -> OK -> Individual Axis Lock

![](../_assets/4.서보보드/axis_lock1.png)

                    (Figure 4.101 Axis Lock Setting Screen 1)

![](../_assets/4.서보보드/axis_lock2.png)

                    (Figure 4.102 Axis Lock Setting Screen 2)

![](../_assets/4.서보보드/axis_lock3.png)

                    (Figure 4.103 Axis Lock Setting Screen 3)

 If the brake for the corresponding axis does not release, the brake output status of the servo board must be checked. Remove the brake wiring (CNB1, CNB7, CNB8 connectors) and output the brake voltage. Measure whether the brake voltage for the corresponding axis is output at 20V or higher from the CNB1, CNB7, or CNB8 connectors. If there is an axis where the voltage output is below 20V, the servo board (BD640) is defective and must be replaced.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (Figure 4.104 Pin Assignment of CNB1, CNB7, and CNB8 Connectors)

 * Inspect for abnormalities in brake power supply

The inspection sequence for the brake power wiring is as follows:

Step 1: Inspect the connectors related to the brake power wiring for any poor contact.

Step 2: Check the brake power wiring for short circuits. Perform a 1:1 check using equipment such as a multimeter (tester).

    * Inspect the internal wiring of the power electronic module. 
      The Hi6-T15 controller is not applicable as it does not have a power electronic module.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (Figure 4.105 Electronic Module and Electronic Board)

 * Inspect the servo board (BD640).

If the power electronic module is normal, measure the brake power (DC24V) on the servo board. The measured value at the test point (PAD24V0BK1) in the red area of the figure below must be DC24V or higher to be considered normal. If it is less than 20V, there is an abnormality in the power supply unit that generates the brake power. Replace the electronic module.

![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (Figure 4.106 Servo Board Brake Power)

[__SOURCE](4-servo-board-part/E02652.md)
# 4.21. E02652. (O Axis) Motor Overload (Load Estimation Not Performed)

### 1. Overview

The motor or drive unit is operating excessively. If the motor or drive unit operates more strainfully than the set value, the servo board detects an error and stops the robot.
This error occurs when an overload state is detected and load estimation has not been performed.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Perform load estimation and check if the error recurs.

{% endhint %}

(1)	Perform load estimation and check if the error recurs.

While using a measuring instrument is the most accurate way to verify the load, if that is not feasible, you can use the load estimation function among the controller features. The load estimation function can only estimate the tool installed at the end of the robot.

The load estimation procedure is as follows:
 * Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation

![](../_assets/4.서보보드/estimation1.png)

                    (Figure 4.107 Load Estimation 1)

![](../_assets/4.서보보드/estimation2.png)

                    (Figure 4.108 Load Estimation 2)

![](../_assets/4.서보보드/estimation3.png)

                    (Figure 4.109 Load Estimation 3)

 * Use the load estimation function to select the tool number to save after estimation.

![](../_assets/4.서보보드/estimation4.png)

                    (Figure 4.110 Load Estimation 4)

* Click "Normal Operation" to perform the task.

    Press the Motor On switch, hold the deadman switch, and then click "Normal Operation."

![](../_assets/4.서보보드/estimation5.png)

                    (Figure 4.111 Load Estimation 5)

* Once the load estimation operation is complete, the estimated results will be displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)

                    (Figure 4.112 Load Estimation 6)

[__SOURCE](4-servo-board-part/E02653.md)
# 4.22. E02653. (O Axis) motor overloaded (low-temperature friction increased)

### 1. Overview

The motor or drive unit is operating excessively. If the motor or drive unit operates more strainfully than the set value, the servo board detects an error and stops the robot.
This error occurs when an overload state is detected and the encoder temperature is low.
Normally, at low temperatures (encoder at 5°C or below), the friction component increases due to the viscosity of the grease, requiring additional torque compared to normal conditions. Therefore, operating the robot at high speeds may trigger this error.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Operate the robot at low speed (playback speed of 30% or less) until the encoder temperature reaches a normal level (approximately 15°C or higher), then restart at normal speed. 

{% endhint %}

(1)	Operate the robot at low speed (playback speed of 30% or less) until the encoder temperature reaches a normal level (approximately 15°C or higher), then restart at normal speed.

![](../_assets/4.서보보드/enc_tmp2.png)

                    (Figure 4.113 Encoder Temperature Check Screen)


[__SOURCE](4-servo-board-part/E02670.md)
# 4.23. E02670. (O Axis) command value abnormal

### 1. Overview

An error may occur due to a communication abnormality between the mainboard and the servo board or because of rapid motion changes. If a communication problem occurs between the boards, normal commands cannot be transmitted from the mainboard to the servo board. In this case, the robot may exhibit abnormal behavior due to incorrect commands, so the system triggers an error and stops the robot. Additionally, in the case of rapid motion, the drive unit may fail to follow the position commands, which also triggers an error and stops the robot.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Check if the mainboard and the servo board are installed correctly.

    * Inspect whether the boards are installed properly.
    * Inspect the boards for any abnormalities or defects.

(2)	Check if there is a work program that causes the robot to move abruptly.

{% endhint %}


(1)	Check if the mainboard and the servo board are installed correctly.

If the mainboard and servo board are not correctly installed in the rack, or if there is a problem with the boards themselves, communication issues may arise, leading to errors.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**To protect existing work programs, please ensure all files on the mainboard are backed up to a USB memory device before removing the boards from the rack.**

</div>

---

The procedure for backing up mainboard files to a USB memory device is as follows:

![](../_assets/4.서보보드/USB연결.png)

                    (Figure 4.114 Connecting USB to TP)
                
When the USB is recognized by the TP, the following icon will appear at the top of the screen.

![](../_assets/4.서보보드/usb.png)

                    (Figure 4.115 TP USB Recognition)

To back up files, navigate to the following path:

            Service -> 5. File Management

![](../_assets/4.서보보드/filemanage.png)

                    (Figure 4.116 Backup Step 1)

![](../_assets/4.서보보드/filemanage2.png)

                    (Figure 4.117 Backup Step 2)

Copy the "Project" folder to the USB.

    * Inspect whether the boards are installed properly.

        Check the connection status of the EtherCAT cable, which serves as the interface between the boards. Please remove and then reinstall it.

![](../_assets/4.서보보드/보드_인터페이스_en.png)

                    (Figure 4.118 Connecting EtherCAT Cable for N Controller)

![](../_assets/4.서보보드/T제어기-보드인터페이스_en.png)

                    (Figure 4.119 Connecting EtherCAT Cable for T Controller)


    * Inspect the boards for any abnormalities.
        Please replace the board to determine if there is a defect.

        

(2)	Check if there is a work program that causes the robot to move abruptly.
Verify whether the error occurs during segments where the motion changes rapidly.
If the error occurs during abrupt motion, the work program must be modified.

The reasons for errors occurring during abrupt motions are as follows: When executing a work program, there are cases where the robot's posture inevitably changes significantly while moving through a short interval. In such instances, the axial speed of the robot increases suddenly. If the servo board cannot follow this command, an error is triggered. To resolve this, you should modify the teaching points at the location where the posture changes abruptly or adjust the robot's orientation.

[__SOURCE](4-servo-board-part/E02680.md)
# 4.24. E02680. (O Axis) Maximum Speed Exceeded

### 1. Overview

The speed of the robot axis has exceeded the maximum limit. Since the robot is in a state where it cannot be controlled normally, the system processes this as an error and stops the robot.

When sending commands from the mainboard to the servo board, restricted commands are sent so as not to exceed the maximum speed. However, if the robot fails to follow these commands and a speed overshoot occurs, a maximum speed exceeded error may be triggered.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the tool data is entered correctly.

(2)	Verify that the robot model is configured correctly.

(3)	Check the versions of the servo board (BD640) and the main com.

(4)	Check if the robot's posture is near a singularity.

(5)	For additional axes, check the acceleration/deceleration parameter settings and the load factor during operation.

(6)	Adjust the work program.

{% endhint %}

(1)	Verify that the tool data is entered correctly. 

If the tool weight or inertia differs significantly from the values registered in the controller, robot control performance may deteriorate, leading to a maximum speed exceeded error. The tool weight and inertia can be registered for each tool number in the menu below:

                System -> 3. Robot Parameters -> Tool Data

![](../_assets/4.서보보드/tool.png)

                    (Figure 4.120 Checking Tool Data)

To automatically set the tool weight or inertia, you can use the load estimation function in the following menu:

* Enter the load estimation function.

        System -> 6. Auto Calibration -> 4. Load Estimation

![](../_assets/4.서보보드/estimation1.png)

                    (Figure 4.121 Load Estimation 1)

![](../_assets/4.서보보드/estimation2.png)

                    (Figure 4.122 Load Estimation 2)

![](../_assets/4.서보보드/estimation3.png)

                    (Figure 4.123 Load Estimation 3)

 * Use the load estimation function to select the tool number to save after estimation.

![](../_assets/4.서보보드/estimation4.png)

                    (Figure 4.124 Load Estimation 4)

 * Click "Normal Operation" to perform the task.

    Press the Motor On switch, hold the deadman switch, and then click "Normal Operation."

![](../_assets/4.서보보드/estimation5.png)

                    (Figure 4.125 Load Estimation 5)

* Once the load estimation operation is complete, the estimated results will be displayed on the screen.

![](../_assets/4.서보보드/estimation6.png)

                    (Figure 4.126 Load Estimation 6)

(2)	Verify that the robot model is configured correctly.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.127 Checking Robot Model)

    Verify that the robot model registered on the TP screen matches the actually installed robot.

(3)	Check the versions of the servo board (BD640) and the main com. 

This error may occur if the compatibility between the servo board (BD640) and the main com version is compromised. Especially if a module has been replaced, perform a version update to match the version of each module with the current main com version.

The version of each module can be checked at the following path:

                Service -> 7. System Diagnosis -> 1. System Version

![](../_assets/4.서보보드/version.png)

                    (Figure 4.128 Checking Module Version)


(4)	Check if the robot's posture is near a singularity. 

An error may occur if L-interpolation or C-interpolation is executed instead of PtP-interpolation in a posture near a singularity. Singularities occur when the B-axis is close to 0 degrees or when the center of the wrist is close to the rotation axis of the S-axis. If the robot must pass near a singularity, change the corresponding step to PtP-interpolation.

![](../_assets/4.서보보드/로봇특이자세.png)

                    (Figure 4.129 Identifying Singularity Postures)

(5)	For additional axes, check the acceleration/deceleration parameter settings and the load factor during operation. 

The motor torque may be insufficient if the maximum speed in the additional axis acceleration/deceleration parameters is too high or if the acceleration time is too short. While monitoring the load factor during robot operation, you should lower the I/Ip maximum speed or increase the acceleration time.

                System -> 3. Robot Parameters -> 34. Accel/Decel Parameters

![](../_assets/4.서보보드/acc.png)

                    (Figure 4.130 Checking Additional Axis Accel/Decel)

(6)	Adjust the work program. 

Modify the step conditions of the corresponding step or the immediately preceding step in the work program. Change the program conditions by first trying to change to "Acc=0," second by lowering the step speed, and third by adding an additional step to the movement path.

[__SOURCE](4-servo-board-part/E02780.md)
# 4.25. E02780. (O Axis) Servo Lock Cannot Be Maintained – Current Generation Error

### 1. Overview

Current for driving the motor or drive unit is not being supplied. The current generated to operate the robot or drive unit is failing to be delivered normally. In such cases, the controller detects an error, prevents the brake from releasing, and cuts off the current supplied to the motor or drive unit. This can be attributed to connection abnormalities between the motor and controller, wiring defects, or issues in the current generation circuit. Additionally, an error may occur if the parameters required for motor control (Gain and maximum current) do not match the actual motor due to an incorrect robot model registration.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the robot model is configured correctly.

(2)	Inspect the motor power lines and encoder communication lines.

* Check the wiring connecting the robot and the controller.
* Check the internal wiring of the robot.
* Check the internal wiring of the controller.

(3) Inspect the cables between the servo board and the amplifier board inside the controller.

(4) Replace other components.

(5) Inspect the BD640 power system lines (Issues such as noise, wiring shorts, etc.).

{% endhint %}

(1)	Verify that the robot model is configured correctly.

Check whether the robot model registered on the TP screen matches the actually installed robot.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.130 Checking Robot Model)

(2)	Inspect the motor power and encoder communication lines.

Turn off the controller power and disconnect the U, V, and W phases of the corresponding axis drive unit to check for any short circuits or open circuits. Perform a 1:1 check of the wiring for each phase using equipment such as a multimeter (tester). Also, verify whether there is any disconnection in the encoder communication lines.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**Exercise extreme caution when inspecting while the power is on, as there is a risk of electric shock.**

</div>

---

* Check the wiring connecting the robot and the controller.
        Remove the wiring connecting the controller to the robot or drive unit. Check if there are any short circuits between the phases (U, V, W) or between a phase and the ground. If a short circuit is found, the corresponding wiring must be replaced.



![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (Figure 4.131 Wiring between N Controller and Robot)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (Figure 4.132 Wiring between T Controller and Robot)

 * Inspect the internal wiring of the robot.
        It is necessary to inspect the wiring connected to the motor inside the robot for any short circuits or incorrect wiring.

![](../_assets/4.서보보드/로봇기내배선.png)

                    (Figure 4.133 Internal Robot Wiring)


 * Inspect the internal wiring of the controller.
        It is necessary to inspect the wiring installed with the amplifiers inside the controller.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (Figure 4.134 Inspecting Internal Wiring of N Controller)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (Figure 4.135 Inspecting Internal Wiring of T Controller)


(2)	Inspect the Board-to-Board connectors between the servo board and the amplifier board inside the controller.

Check whether the connectors (Board-to-Board) that link and secure the servo board to the amplifier board are installed correctly. If the connection is poor, this error may occur.

![](../_assets/4.서보보드/서보보드_앰프보드_b2b_en.png)

                    (Figure 4.136 Connection between Servo Board and Amplifier Board in N Controller)

![](../_assets/4.서보보드/T제어기_서보보드_앰프보드_en.png)

                    (Figure 4.137 Connection between Servo Board and Amplifier Board in T Controller)

(3)	Replace other components.

Check for errors by replacing components in the following order: Servo Board (BD640) → Amplifier Board → Wire Harness → Motor → PSM (Power Supply Module).

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                    (Figure 4.138 Drive Components for N Controller)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                    (Figure 4.139 Drive Components for T Controller)

(5) Inspect the BD640 power system lines.

If this error occurs simultaneously with other errors such as E64003 (Servo board (BD640) status abnormality detected), E02764 (Safety board (BD632) error), E02500 (Regenerative discharge resistor overheat), E02504 (AC input voltage exceeded), E02505 (AMP PN overvoltage or discharge abnormality), E02506 (AMP PN undervoltage), E62850 (MCON1 input wiring noise), or E62851 (MCON2 input wiring noise), you must inspect the power systems of the BD640 and BD632 (checking for noise, wire harness wiring status, etc.).

[Image of a wiring diagram showing the 24V DC power distribution system and ground connections for an industrial robot controller]

A short circuit in the factory wiring can cause abnormalities in the 24V power supply and ground status of the boards, leading to multiple errors related to I/O signals. It is necessary to inspect the power systems (noise, wire harness wiring status, etc.) of the BD640 and BD632.
[__SOURCE](4-servo-board-part/E02781.md)
# 4.26. E02781. (O Axis) Servo Lock Cannot Be Maintained – Parameter Error

### 1. Overview

Current for driving the motor or drive unit is not being supplied. The current generated to operate the robot or drive unit is failing to be delivered normally. In such cases, the controller detects the error, prevents the brake from releasing, and cuts off the current supplied to the motor or drive unit. This can be attributed to connection abnormalities between the motor and the controller, wiring defects, or issues in the current generation circuit. Additionally, an error may occur if the parameters required for motor control (Gain and maximum current) do not match the actual motor due to an incorrect robot model registration.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the robot model is configured correctly.

(2)	Inspect the motor power lines and encoder communication lines.

* Check the wiring connecting the robot and the controller.
* Check the internal wiring of the robot.
* Check the internal wiring of the controller.

(3) Inspect the cables between the servo board and the amplifier board inside the controller.

(4) Replace other components.

{% endhint %}

(1)	Verify that the robot model is configured correctly.

Check whether the robot model registered on the TP screen matches the actually installed robot.

![](../_assets/4.서보보드/robot_model.png)

                    (Figure 4.130 Checking Robot Model)

(2)	Inspect the motor power and encoder communication lines.

Turn off the controller power and disconnect the U, V, and W phases of the corresponding axis drive unit to check for any short circuits or open circuits. Perform a 1:1 check of the wiring for each phase using equipment such as a multimeter (tester). Also, verify whether there is any disconnection in the encoder communication lines.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ Warning

**Exercise extreme caution when inspecting while the power is on, as there is a risk of electric shock.**

</div>

---

* Check the wiring connecting the robot and the controller.
        Remove the wiring connecting the controller to the robot or drive unit. Check if there are any short circuits between the phases (U, V, W) or between a phase and the ground. If a short circuit is found, the corresponding wiring must be replaced.


![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (Figure 4.131 Wiring between N Controller and Robot)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (Figure 4.132 Wiring between T Controller and Robot)

* Inspect the internal wiring of the robot.
        It is necessary to inspect the wiring connected to the motor inside the robot for any short circuits or incorrect wiring.

![](../_assets/4.서보보드/로봇기내배선.png)

                    (Figure 4.133 Internal Robot Wiring)


* Inspect the internal wiring of the controller.
        It is necessary to inspect the wiring installed with the amplifiers inside the controller.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (Figure 4.134 Inspecting Internal Wiring of N Controller)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (Figure 4.135 Inspecting Internal Wiring of T Controller)


(2)	Inspect the Board-to-Board connectors between the servo board and the amplifier board inside the controller.

Check whether the connectors (Board-to-Board) that link and secure the servo board to the amplifier board are installed correctly. If the connection is poor, this error may occur.

![](../_assets/4.서보보드/서보보드_앰프보드_b2b_en.png)

                    (Figure 4.136 Connection between Servo Board and Amplifier Board in N Controller)

![](../_assets/4.서보보드/T제어기_서보보드_앰프보드_en.png)

                    (Figure 4.137 Connection between Servo Board and Amplifier Board in T Controller)

(3)	Replace other components.

Check for errors by replacing components in the following order: Servo Board (BD640) → Amplifier Board → Wire Harness → Motor → PSM (Power Supply Module).

[Image of a flowchart showing the component replacement sequence for troubleshooting a robot servo system: Servo Board to Amplifier Board to Wire Harness to Motor to Power Supply Module]

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                    (Figure 4.138 Drive Components for N Controller)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                    (Figure 4.139 Drive Components for T Controller)

[__SOURCE](4-servo-board-part/E02472.md)
# 4.27. E02472. (O Axis) Encoder Overheat Detected (OH Bit Set)

### 1. Overview

The servo board performs serial communication with the encoder to control the servo motor and receives encoder data periodically; this error occurs when the OH bit is detected from the encoder.

The OH bit is set when the internal temperature of the encoder exceeds the allowable range. The threshold reference temperature is approximately 90°C to 100°C; however, since specifications vary by encoder model, please check the manufacturer's manual.


### 2. Cause and Inspection

{% hint style="info" %}

(1)	Perform a replacement test of the motor (encoder)

(2)	Check the operating conditions (speed, load, etc.)

(3)	Inspect the ambient temperature around the encoder

(4)	Replace the servo board (BD640)

{% endhint %}

((1)	Perform a replacement test of the motor (encoder).

If the error does not occur after replacing the servo motor, the servo motor is defective. Please replace the servo motor with a normal one. The figure below shows the positions of the motors for each axis of the robot; for other robots, please refer to the corresponding mechanical maintenance manual for replacement.

![](../_assets/4.서보보드/로봇_모터_위치.png)

    (Figure 4.36 Motor (Encoder) Replacement Position)

(2)	Check the operating conditions (speed, load, etc.).

Check the saturated encoder temperature while running the Job program. The encoder temperature can be checked as follows:

    Engineering Mode -> Window Adjustment -> System Characteristics -> System Characteristics List - Motor/Encoder

![](../_assets/4.서보보드/enc_tmp.png)

    (Figure 4.37 Checking Encoder Temperature)

(3)	Inspect the ambient temperature around the encoder.

The internal temperature of the encoder may increase due to the external temperature, causing an error.

(4)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, it can be determined as a failure in the encoder data receiving unit of the servo board.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

    (Figure 4.38 Replacing N Controller Servo Board)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

    (Figure 4.39 Replacing T Controller Servo Board)

[__SOURCE](4-servo-board-part/E02554.md)
# 4.28. E02554. Initial Pre-Charge Relay Operation Failure

### 1. Overview

The servo board (BD640) operates the initial charge relay during the motor power-on process and generates an error by monitoring the operating status of the initial charge relay. Since the initial charge relay functions to suppress inrush current, if a relay operation abnormality occurs, an error is generated for safety and the motor power application is cut off.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the monitoring system.

(2)	Inspect the electronic boards.

(3)	Inspect the servo board (BD640).

{% endhint %}

(1)	Inspect the monitoring system.

Check the cabling between the electronic module (PSM or PDM), where the initial charge resistor and relay are installed, and the servo board (BD640), which collects monitoring signals. The cable name is CNPRC, and it enters the electronic module through the bottom left side of the servo board. Inspect the connector connection status of this cable. In the case of the Hi6-T controller, this is not applicable as there is no such cable wiring.

![](../_assets/4.서보보드/CNPRC케이블.png)

    (Figure 4.40 CNPRC Cable Connection)

(2)	Inspect the electronic boards

In the case of the Hi6-N controller, there may be problems with the servo board, electronic board, or cable wiring, so please inspect or replace them. In the case of the Hi6-T controller, this is not applicable as there is no such cable wiring.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

    (그림 4.41 전장모듈 내부 전장보드)

(3)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, it can be determined as a failure in the encoder data receiving unit of the servo board.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (Figure 4.42 Replacing N Controller Servo Board)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (Figure 4.43 Replacing T Controller Servo Board)
    

[__SOURCE](4-servo-board-part/E02560.md)
# 4.29. E02560. Brake Power Supply Error

### 1. Overview

While the servo board is monitoring the brake power (24V), an error is generated if the voltage falls outside the set normal range. If the brake power is not supplied normally, the fixation of the robot axes may become unstable; therefore, the servo controller detects this, generates an error, and stops the robot safely.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Verify that the brake power (24V) is being supplied normally

(2)	Check for any disconnection or poor contact in the brake power cable

(3)	Replace the servo board (BD640)

{% endhint %}

(1)	Verify that the brake power (24V) is being supplied normally

The inspection sequence for the brake power wiring is as follows:

Step 1: Inspect the connectors related to the brake power wiring for any poor contact.

Step 2: Check the brake power wiring for short circuits. Perform a 1:1 check using equipment such as a multimeter (tester).

    * Inspect the internal wiring of the power electronic module.
        The Hi6-T15 controller is not applicable as it does not have a power electronic module.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (Figure 4.44 Power Electronic Module)

(2)	Check for any disconnection or poor contact in the brake power cable.

Inspect the internal wiring of the controller. For the Hi6-N controller, inspect the wiring between the CNPB1 (BD640) connector and the CNPB1 (electronic board) connector. For the Hi6-T15 controller, inspect the wiring between the CNPB1 (BD602T) connector and the brake SMPS output.

![](../_assets/4.서보보드/N제어기_브레이크_전원케이블.png)

                    (Figure 4.45 N Controller Brake Power Inspection)

![](../_assets/4.서보보드/T제어기_브레이크전원.png)

                    (Figure 4.45 T Controller Brake Power Inspection)

(3)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, it can be determined as a failure in the servo board's monitoring circuit.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (Figure 4.46 Replacing N Controller Servo Board)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (Figure 4.47 Replacing T Controller Servo Board)

[__SOURCE](4-servo-board-part/E02570.md)
# 4.30. E02570. (O Axis) Brake Output Error

### 1. Overview

The servo board (BD640) monitors the brake operation command and the signal from the brake feedback circuit; an error is generated if the two signals do not match. If the output of the brake circuit is not performed normally, brake operation may fail; therefore, the servo board detects this and stops the robot. 

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the brake wiring.

(2)	Inspect the servo board (BD640).

{% endhint %}

(1)	Inspect the brake wiring.

The inspection sequence for the brake wiring is as follows:

Step 1: Inspect the connectors related to the brake wiring for any poor contact.

Step 2: Check the brake wiring for short circuits. Perform a 1:1 check for each axis's wiring using equipment such as a multimeter (tester).

Step 3: Perform a replacement test of the brake wiring.

If there are phenomena such as poor contact, or contact between the brake power line and other power lines or metal parts of the robot body even though the brake wiring is not disconnected, it cannot be detected through a short-circuit test; therefore, please perform a wiring replacement test.

    * Inspect the internal wiring of the controller.
        For the Hi6-N controller, inspect the wiring between the CNB1 (BD640) connector and CMC1, CMC2.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (Figure 4.54 N Controller Brake Output Wiring)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (Figure 4.55 T Controller Brake Output Wiring)
    
    * Inspect the wiring between the controller and the robot.
        For the Hi6-N controller, inspect the wiring between CMC1 and CMR1, and between CMC2 and CMR2. For the Hi6-T15 controller, inspect the wiring between CMEC1 and CMER1.

![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (Figure 4.56 N Controller Brake Output Wiring)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (Figure 4.57 T Controller Brake Output Wiring)

(2)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, it can be determined as a failure in the servo board's monitoring circuit.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (Figure 4.58 Replacing N Controller Servo Board)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (Figure 4.59 Replacing T Controller Servo Board)

[__SOURCE](4-servo-board-part/E02564.md)
# 4.31. E02564. (O Axis) Brake Output Overcurrent Detected

### 1. Overview

The servo board (BD640) monitors the overcurrent status of the brake output circuit; if a Fault signal is detected from the protection circuit (IC) connected to the output circuit, it is determined as an overcurrent situation and generates an error. If such an abnormal condition occurs, the reliability of the brake control cannot be guaranteed; therefore, the servo board immediately detects this and stops the robot safely.

### 2. Cause and Inspection

{% hint style="info" %}

(1)	Inspect the brake wiring.

(2)	Inspect the servo board (BD640).

{% endhint %}

(1)	Inspect the brake wiring.

The inspection sequence for the brake wiring is as follows:

Step 1: Inspect the connectors related to the brake wiring for any poor contact.

Step 2: Check the brake wiring for short circuits. Perform a 1:1 check for each axis's wiring using equipment such as a multimeter (tester).

Step 3: Perform a replacement test of the brake wiring.

If there are phenomena such as poor contact, or contact between the brake power line and other power lines or metal parts of the robot body even though the brake wiring is not disconnected, it cannot be detected through a short-circuit test; therefore, please perform a wiring replacement test.

    * Inspect the internal wiring of the controller.
        For the Hi6-N controller, inspect the wiring between the CNB1 (BD640) connector and CMC1, CMC2.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (Figure 4.48 N Controller Brake Output Wiring)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (Figure 4.49 T Controller Brake Output Wiring)
    
* Inspect the wiring between the controller and the robot.
        For the Hi6-N controller, inspect the wiring between CMC1 and CMR1, and between CMC2 and CMR2. For the Hi6-T15 controller, inspect the wiring between CMEC1 and CMER1.

![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (Figure 4.50 N Controller Brake Output Wiring)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (Figure 4.51 T Controller Brake Output Wiring)

(2)	Perform a replacement test of the servo board. 

If the error does not occur after replacing the servo board, it can be determined as a failure in the servo board's monitoring circuit.

![](../_assets/4.assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (Figure 4.52 Replacing N Controller Servo Board)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (Figure 4.53 Replacing T Controller Servo Board)
[__SOURCE](5-communication/README.md)
# 5. Communication
[__SOURCE](5-communication/E29003.md)
# 5.1. E29003 Board Communication Error (EtherCAT Disconnected)

### 1. Summary

A board communication error (EtherCAT connection lost) has occurred.
Communication between the main control module (H6COM-T) and the servo board (BD640) and safety board (BD632) has been disconnected.

### 2. Causation

{% hint style="info" %}

(1)	Check the inter-board communication cable connection and the cable condition.<br>
(2)	Inspect the servo board (BD640).<br>
(3)	Inspect the safety board (BD632).<br>

{% endhint %}


### (1)	Check the inter-board communication cable connection status.

### [Check the Ethernet cable connection status between each module (Main Control Module (H6COM-T) and the servo board (BD640) and safety board (BD632))]

![](../_assets/5-Communication/E29003/보드_인터페이스_en.png)<br>

1)	Inspection Targets<br>
A.	Ethernet cable between the main control module (H6COM-T) and the servo board (BD640)<br>
B.	Ethernet cable between the servo board (BD640) and safety board (BD632)<br>
2)	Inspection Items<br>
A.	Check that the connectors at both ends of the cable are securely fastened.<br>
B.	Visually inspect the cable for breaks, crimping damage, bends, or damage.<br>
C.	Check the connector pins (terminals) for corrosion, contamination, or bending.<br>
3)	Inspection Method<br>
A.	With the power turned OFF, disconnect and reconnect the cable.<br>
B.	When inserting, ensure it is fully seated until a “click” sound is heard.<br>
C.	If necessary, replace the cable with a spare cable and try again.<br>
D.	Recheck the connection order and verify that it is connected to the correct LAN port.<br>
4)	Additional Checks<br>
A.	Check the Link/Act LED status on the servo board (BD640) and safety board (BD632).<br>
- Normal: Green (left) blinking, Yellow (right) ON <br>
- Abnormal: Green (left) & Yellow (right) lights remain OFF or ON.<br>
![](../_assets/5-Communication/E29003/그림2.png)<br>
B.	If disconnections occur repeatedly, consider the possibility of an internal cable break → Cable replacement may be necessary.<br>
C.	Also check for possible damage to the Ethernet connector (PCB terminal area).<br>

 
### (2) Inspect the servo board (BD640).
#### [Servo board (BD640) inspection procedure]
![](../_assets/5-Communication/E29003/그림3.png)<br> 

1) Check the power status<br>
   Confirm that LED1 and LED2 blink green. <br>
   Confirm that the 7-segment display indicates P001 or P002.<br>

2) Check the normal boot status<br>
   After the Main Control Module (H6COM-T) has completely booted (approximately 50 seconds after power-on), <br>The 7-segment display must indicate P002.<br>

If a communication connection problem still exists even though there are no abnormalities in the inspection items 1) and 2), replace the board.

 
### (3) Inspect the safety board (BD632)

#### [Safety board (BD632) inspection procedure]
![](../_assets/5-Communication/E29003/그림11_en.png)<br> 
 
1)	Power status inspection procedure<br>
A.	Verify that the two LEDs in the figure above are lit green.<br>
B.	If the power LED is red or OFF, check whether the indicated fuse is in normal condition.<br>
C.	If the fuse is blown, replace the fuse.<br>

2)	Check for power instability during motor ON<br>
A.	Verify that the power LED stays green when the motor is turned ON. <br>
B.	If the LED turns red or goes OFF at the moment of motor ON, the power supply is unstable.<br>

3)	If the power supply is unstable<br>
A.	Verify the power connector is securely connected.<br>
B.	Inspect the power cable.<br>
C.	Check the grounding of the safety board (BD632) (ground cable and grounding terminal connection).<br>

4)	Verify the safety board is in a normal boot state<br>
A.	After the main control module (H6COM-T) has fully booted (about 50 seconds after power-on),<br> the 7-segment display shall indicate two “S” characters.<br>

5)	If communication issues persist despite normal results in inspection items 1)–4), replace the safety board (BD632).<br>

[__SOURCE](5-communication/E29016.md)
# 5.2. E29016 Board Communication (EtherCAT) Master Disconnection Detected

### 1. Summary

The connection with the first device connected to the EtherCAT master has been lost.

### 2. Causation

{% hint style="info" %}

(1)	Check the inter-board communication cable connection and the cable condition.
(2)	Inspect the servo board (BD640).

{% endhint %}

### (1) Check the inter-board communication cable connection status.

#### [Check the Ethernet cable connection status between each module (Main Control Module (H6COM-T) and the servo board (BD640))]
![](../_assets/5-Communication/E29016/보드_인터페이스_en.png)<br> 

1)	Inspection Targets<br>
A.	Ethernet cable between the main control module (H6COM-T) and the servo board (BD640)<br>
2)	Inspection Items<br>
A.	Check that the connectors at both ends of the cable are securely fastened.<br>
B.	Visually inspect the cable for breaks, crimping damage, bends, or damage.<br>
C.	Check the connector pins (terminals) for corrosion, contamination, or bending.<br>
3)	Inspection Method<br>
A.	With the power turned OFF, disconnect and reconnect the cable.<br>
B.	When inserting, ensure it is fully seated until a “click” sound is heard.<br>
C.	If necessary, replace the cable with a spare cable and try again.<br>
D.	Recheck the connection order and verify that it is connected to the correct LAN port.<br>
4)	Additional Checks<br>
A.	Check the Link/Act LED status on the servo board (BD640)<br>
- Normal: Green (left) blinking, Yellow (right) ON  <br>
- Abnormal: Green (left) & Yellow (right) lights remain OFF or ON<br>
![](../_assets/5-Communication/E29016/그림2.png)<br>
B.	If disconnections occur repeatedly, consider the possibility of an internal cable break → Cable replacement may be necessary.<br>
C.	Also check for possible damage to the Ethernet connector (PCB terminal area).<br>

 
### (2) Inspect the servo board (BD640).
#### [Servo board (BD640) inspection procedure]
![](../_assets/5-Communication/E29016/그림3.png)<br> 

1) Check the power status<br>
   Confirm that LED1 and LED2 blink green.  <br>
   Confirm that the 7-segment display indicates P001 or P002.<br>

2) Check the normal boot status<br>
   After the Main Control Module (H6COM-T) has completely booted (approximately 50 seconds after power-on), <br>
   The 7-segment display must indicate P002.<br>

If a communication connection problem still exists even though there are no abnormalities in the inspection items 1) and 2), replace the board.

[__SOURCE](appendices/README.md)
# Appendices

  



[__SOURCE](appendices/rules-occupational-safety.md)
# Rules on Occupational Safety and Health Standards and Safety Inspection Notification
This industrial robot shall be installed in consideration of the inspection requirements specified in the Rules on Occupational Safety and Health Standards and the Safety Inspection Notification, where applicable.

"[Rules on Occupational Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/korean/README)"

[__SOURCE](quality-assurance.md)
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/korean/README)"
