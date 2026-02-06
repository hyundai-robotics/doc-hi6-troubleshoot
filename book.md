
[__SOURCE](README.md)
# Maintenance Manual – Troubleshooting
The controller is designed with a primary focus on high precision and high-speed performance. In the event of a malfunction, the system is structured to allow easy identification of the cause and rapid recovery. Please ensure that you fully understand this manual and use it effectively for smooth and efficient troubleshooting.

## Troubleshooting Procedure
This section describes the troubleshooting methods for each error code that may occur in the Hi6-N and Hi6-T controllers.


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

f the error does not recur after replacing the servo motor, the original motor is defective. Please replace the servo motor with a known functional unit. The figure below illustrates the location of each axis motor for the HS165 robot. For other robot models, please refer to the corresponding mechanical maintenance manual for replacement instructions.

![](../_assets/2.서보AMP/E02520/E02520_IPM폴트_HS165로봇.PNG)

Figure 1.3 Motor Locations for Each Axis of the HS165 Robot

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

Figure 1.1 Internal Wiring Inspection Points for Each Axis of the HS165


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
Figure 1 Example of hardware limit switch installation positions (HS165/HS200 Robot)

![](../_assets/3-Safety-io/E00002/그림2.png)<br>
Figure 2 Example of hardware limit switch operating range (HS165/HS200 S Axis)

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
**Figure 2** Example of Hardware Limit Switch Installation Positions (HS165 / HS200)

![](../_assets/3-Safety-io/E02200/그림3.png)<br>
**Figure 3** Example of Hardware Limit Switch Operating Range  
(HS165 / HS200, S-axis)

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
# 4. 서보보드
[__SOURCE](4-servo-board-part/E02450.md)
# 4.1. E02450. (O축) 엔코더 응답 없음

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신하는데, 엔코더로부터 수신된 데이터가 정해진 통신규정에 어긋나는 경우 발생하는 에러입니다.

엔코더 데이터를 송수신하는 부품들의 고장이거나 배선 또는 엔코더 쉴드 라인의 처리 문제로 상기의 에러가 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 공급전압을 확인하십시오 

(2)	엔코더 배선을 점검하십시오

(3)	서보보드를 교체 시험하십시오

(4)	모터(엔코더)를 교체 시험하십시오

(5)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

(1)	엔코더 공급전압을 확인하십시오.
엔코더에 공급하는 전원전압은 엔코더측 커넥터 공급 전압이 5V±5% (4.75V ~ 5.25V)범위 내에 있어야 합니다. 엔코더측 커넥터 전압이 4.75V이하로 떨어질 경우, 엔코더가 정상 동작하지 않아, 상기 에러 발생 가능성이 있습니다.

엔코더측 커넥터 pin(3-4)의 전압을 측정해 주십시오.

![](../_assets/4.서보보드/encoder_connector_pin_info_en.png)

                    (그림 4.1 엔코더 커넥터 핀 정보)

측정된 전압이 기준전압보다 낮을 경우 서보보드(BD640)의 VR1 볼륨저항을 돌려 엔코더측 커넥터 전압이 기준전압 이내가 되도록 조정하십시오.

![](../_assets/4.서보보드/BD640_가변저항.png)

                    (그림 4.2 BD640 가변저항)

(2)	엔코더 배선을 점검하십시오.

엔코더의 배선점검 순서는 다음과 같습니다.

1차: 엔코더 배선에 관련된 커넥터들의 접촉 불량여부를 점검하십시오.

2차: 엔코더 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 상의 배선을 1:1로 체크하십시오.

3차: 엔코더 배선을 교체시험 하십시오.

엔코더 배선이 단선되지 않고 쉴드선의 접촉불량, 엔코더 신호선과 타 전력선 또는 로봇 본체 금속부위와의 접촉 등의 현상이 있을 경우에는 단락유무 검사로는 검사할 수 없으므로 배선교체 시험을 하여주십시오.

* 제어기 내부 배선을 점검하십시오.
CNEC1,4(BD640)커넥터와 CEC1 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/hi6N제어기_en.png)

                    (그림 4.3 Hi6-N 제어기 엔코더 배선 점검)

![](../_assets/4.서보보드/Hi6_T15제어기_en.png)

                    (그림 4.4 Hi6-T15 제어기 엔코더 배선 점검)

* 제어기와 로봇간의 배선을 점검하십시오.
Hi6-N제어기의 경우, CNEC1와 CER1간의 배선을 Hi6-T15제어기의 경우, CMEC1과 CMER1 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/로봇_N제어기_설치구성.png)

                    (그림 4.5 Hi6-N 제어기와 로봇간 기본 설치 구성도)

![](../_assets/4.서보보드/로봇_T제어기_설치구성.png)

                    (그림 4.6 Hi6-T15 제어기와 로봇간 기본 설치 구성도)

![](../_assets/4.서보보드/N제어기_설치구성_상세.png)

                    (그림 4.7 Hi6-N 제어기와 로봇간 기본 설치 구성도 상세)

![](../_assets/4.서보보드/T제어기_설치구성_상세.png)

                    (그림 4.8 Hi6-N 제어기와 로봇간 기본 설치 구성도 상세)

* 본체 내부의 배선을 점검하십시오.
CER1과 엔코더측 커넥터간의 배선을 점검하십시오.
배선점검은 로봇 보수설명서의 배선 접속도를 참고하시기 바랍니다.

![](../_assets/4.서보보드/로봇기내배선.png)

                    (그림 4.9 로봇기내배선)

(3)	서보보드를 교체 시험하십시오. 
서보 보드를 교체한 후 에러가 발생하지 않으면 서보보드의 엔코더 수신부 불량입니다. 서보 보드를 정상품으로 교체하여 주십시오.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.10 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.11 T제어기 서보보드 교체)

(4)	모터(엔코더)를 교체 시험하십시오. 
서보 모터를 교체한 후 에러가 발생하지 않으면 서보모터의 불량입니다. 서보 모터를 정상품으로 교체하여 주십시오. 아래 그림은 HS165 로봇의 각 축 모터의 위치를 나타내고 있으며, 다른 로봇은 해당 기구 보수설명서를 참고하여 교체하시기 바랍니다.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                    (그림 4.12 HS165 로봇의 각 축 모터 위치)

(5)	조치 완료후 배선의 통신상태를 점검하십시오.
문제부분의 조치가 완료된후 『엔코더 통신실패 횟수 표시 기능 메뉴얼』을 참고하여 통신상태를 점검 하십시오.

![](../_assets/4.서보보드/엔코더통신실패.png)

                    (그림 4.13 엔코더 통신실패 모니터링)

![](../_assets/4.서보보드/엔코더_통신실패_횟수_en.png)


[__SOURCE](4-servo-board-part/E02451.md)
# 4.2. E02451. (O축) 엔코더 데이터 수신 개수 이상

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더로부터 수신된 데이터의 개수가 규정치에 어긋나는 경우 발생합니다.

엔코더로부터 수신된 데이터의 개수가 맞지 않을 경우는 주로 배선 또는 엔코더 쉴드 라인의 처리 문제로 엔코더 신호선에 노이즈가 유입되는 경우 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 배선을 점검하십시오

(2)	모터(엔코더)를 교체 시험하십시오

(3)	서보보드를 교체 시험하십시오

(4)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

(1)	엔코더 배선을 점검하십시오.

엔코더의 배선점검 순서는 다음과 같습니다.

1차: 엔코더 배선에 관련된 커넥터들의 접촉 불량여부를 점검하십시오.

2차: 
엔코더 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 상의 배선을 1:1로 체크하십시오.

3차: 엔코더 배선을 교체시험 하십시오.

엔코더 배선이 단선되지 않고 쉴드선의 접촉불량, 엔코더 신호선과 타 전력선 또는 로봇 본체 금속부위와의 접촉 등의 현상이 있을 경우에는 단락유무 검사로는 검사할 수 없으므로 배선교체 시험을 하여주십시오.

* 제어기 내부 배선을 점검하십시오.

    CNEC1,4(BD640)커넥터와 CEC1간의 배선을 점검하십시오.

    ![](../_assets/4.서보보드/hi6N제어기_en.png)
    
                    (그림 4.14 Hi6-N 제어기 엔코더 배선 점검)

    ![](../_assets/4.서보보드/Hi6_T15제어기_en.png)

                    (그림 4.15 Hi6-T15 제어기 엔코더 배선 점검)

* 제어기와 로봇간의 배선을 점검하십시오.

    Hi6-N제어기의 경우, CNEC1와 CER1간의 배선을 Hi6-T15제어기의 경우, CMEC1과 CMER1 간의 배선을 점검하십시오.

    ![](../_assets/4.서보보드/로봇_N제어기_설치구성.png)

                    (그림 4.16 Hi6-N 제어기와 로봇간 기본 설치 구성도)

    ![](../_assets/4.서보보드/로봇_T제어기_설치구성.png)

                    (그림 4.17 Hi6-T 제어기와 로봇간 기본 설치 구성도)

    ![](../_assets/4.서보보드/N제어기_설치구성_상세.png)

                    (그림 4.18 Hi6-N 제어기와 로봇간 기본 설치 구성도 상세)

    ![](../_assets/4.서보보드/T제어기_설치구성_상세.png)

                    (그림 4.19 Hi6-T 제어기와 로봇간 기본 설치 구성도 상세)

* 본체 내부의 배선을 점검하십시오.

    CER1과 엔코더측 커넥터간의 배선을 점검하십시오.
    배선점검은 로봇 보수설명서의 배선 접속도를 참고하시기 바랍니다.

    ![](../_assets/4.서보보드/로봇기내배선.png)

                    (그림 4.20 로봇 기내 배선)

(2)	모터(엔코더)를 교체 시험하십시오. 

서보 모터를 교체한 후 에러가 발생하지 않으면 서보모터의 불량입니다. 서보 모터를 정상품으로 교체하여 주십시오. 아래 그림은 HS165 로봇의 각 축 모터의 위치를 나타내고 있으며, 다른 로봇은 해당 기구 보수설명서를 참고하여 교체하시기 바랍니다.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                    (그림 4.21 HS165 로봇의 각 축 모터 위치)

(3)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보보드의 불량입니다. 서보 보드를 정상품으로 교체하여 주십시오.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.22 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.23 T제어기 서보보드 교체)
    
(4)	조치 완료후 배선의 통신상태를 점검하십시오.

문제부분의 조치가 완료된후 『엔코더 통신실패 횟수 표시 기능 메뉴얼』을 참고하여 통신상태를 점검 하십시오.

![](../_assets/4.서보보드/엔코더통신실패.png)

                    (그림 4.24 엔코더 통신실패 모니터링)

![](../_assets/4.서보보드/엔코더_통신실패_횟수_en.png)


[__SOURCE](4-servo-board-part/E02452.md)
# 4.3. E02452. (O축) 엔코더 데이터 종료 신호(Ser_End) 수신 실패

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더로부터 데이터 프레임의 종료를 알리는 신호(Ser_End)가 수신되지 않는 경우 발생합니다.

엔코더로부터 데이터 프레임의 종료를 알리는 신호가 수신되지 않을 경우는 주로 배선 또는 엔코더 쉴드 라인의 처리 문제로 엔코더 신호선에 노이즈가 유입되는 경우 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 배선을 점검하십시오

(2)	모터(엔코더)를 교체 시험하십시오

(3)	서보보드를 교체 시험하십시오

(4)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

세부적인 점검방법은 "E02450 (O축) 엔코더 응답 없음"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02453.md)
# 4.4. E02453. (O축) 엔코더 데이터 오류 (CRC 오류 검출됨)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더로부터 수신된 데이터의 CRC값과 서보 보드에서 계산한 CRC 값이 일치하지 않는 경우 발생합니다.

엔코더로부터 수신된 데이터의 CRC에러가 발생할 경우는 주로 배선 또는 엔코더 쉴드 라인의 처리 문제로 엔코더 신호선에 노이즈가 유입되는 경우 발생할 수 있습니다.


### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 배선을 점검하십시오

(2)	모터(엔코더)를 교체 시험하십시오

(3)	서보보드를 교체 시험하십시오

(4)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

세부적인 점검방법은 "E02450 (O축) 엔코더 응답 없음"을 참조하십시오.

[__SOURCE](4-servo-board-part/E02454.md)
# 4.5. E02454. (O축) 엔코더 단선 혹은 접촉불량(모터 OFF 상태)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더와 서보 보드 간의 통신이 불안정하거나 신호가 아예 수신되지 않을 때 발생합니다.

엔코더로부터 서보 보드 간의 통신이 불안정하거나 신호가 아에 수신되지 않는 경우는 주로 엔코더 케이블의 단선 또는 접촉 불량인 경우 발생할 수 있습니다.

### 2. 원인 및 점검
{% hint style="info" %}
(1)	엔코더 공급전압을 확인하십시오 
(2)	엔코더 배선을 점검하십시오
(3)	서보보드를 교체 시험하십시오
(4)	모터(엔코더)를 교체 시험하십시오
(5)	조치 완료후 배선의 통신상태를 점검하십시오
{% endhint %}

세부적인 점검방법은 "E02450 (O축) 엔코더 응답 없음"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02455.md)
# 4.6. E02455. (O축) 엔코더 데이터 이상 (비정상 값 변화 감지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더에서 수신된 위치값 또는 속도값이 비정상적으로 변경될 때 발생합니다. 

엔코더로부터 수신된 위치값 또는 속도값이 비정상적으로 변경되는 경우는 주로 배선 또는 엔코더 쉴드 라인의 처리 문제로 엔코더 신호선에 노이즈가 유입되는 경우 발생할 수 있습니다.


### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 배선을 점검하십시오

(2)	모터(엔코더)를 교체 시험하십시오

(3)	서보보드를 교체 시험하십시오

(4)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

세부적인 점검방법은 "E02450 (O축) 엔코더 응답 없음"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02459.md)
# 4.7. E02459. (O축) 엔코더 단선 혹은 접촉불량(모터 ON 상태)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더와 서보 보드 간의 통신이 불안정하거나 신호가 아예 수신되지 않을 때 발생합니다.

엔코더로부터 서보 보드 간의 통신이 불안정하거나 신호가 아에 수신되지 않는 경우는 주로 엔코더 케이블의 단선 또는 접촉 불량인 경우 발생할 수 있습니다.


### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 공급전압을 확인하십시오 

(2)	엔코더 배선을 점검하십시오

(3)	서보보드를 교체 시험하십시오

(4)	모터(엔코더)를 교체 시험하십시오

(5)	조치 완료후 배선의 통신상태를 점검하십시오

{% endhint %}

세부적인 점검방법은 "E02450 (O축) 엔코더 응답 없음"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02460.md)
# 4.8. E02450. (O축) 엔코더 내부 회전값 오류 (CE 비트 감지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더 내부에서 회전값 계산에 오류가 발생하여 CE(Counter Error) 비트가 세트 되었을 때 발생합니다.

엔코더로부터 수신된 데이터는 정상이나 엔코더가 스스로 내부상태를 감시한 결과 에러상태(CE)인 경우에 발생할 수 있습니다.
 
CE(Counter Error) : 엔코더 주전원 On시, 1회전 Data가 오동작 또는 고장등에 의해 위치 어긋남이 발생하는 경우 발생

### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 공급전압을 확인하십시오.

(2)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.

(3)	계속 에러발생시 모터(엔코더)를 교체 시험하십시오. 

{% endhint %}

(1)	엔코더 공급전압을 확인하십시오.
엔코더에 공급하는 전원전압은 엔코더측 커넥터 공급 전압이 5V±5% (4.75V ~ 5.25V)범위 내에 있어야 합니다. 엔코더측 커넥터 전압이 4.75V이하로 떨어질 경우, 엔코더가 정상 동작하지 않아, 상기 에러 발생 가능성이 있습니다.

엔코더측 커넥터 pin(3-4)의 전압을 측정해 주십시오.

![](../_assets/4.서보보드/엔코더_커넥터_핀정보_en.png)

                        (그림 4.25 엔코더 커넥터 핀 정보)

측정된 전압이 기준전압보다 낮을 경우 서보보드(BD640)의 VR1 볼륨저항을 돌려 엔코더측 커넥터 전압이 기준전압 이내가 되도록 조정하십시오.

![](../_assets/4.서보보드/BD640_가변저항.png)

                        (그림 4.26 BD640 가변저항)

(2)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.

에러해제 후, 주전원 OFF/ON시 계속 에러가 발생하면 모터(엔코더)교체 시험하십시오.
에러해제는 아래의 메뉴에서 실행합니다.

        시스템 -> 5. 초기화 -> 4. 시리얼 엔코더 리셋 - 에러해제

![](../_assets/4.서보보드/엔코더_에러해제.png)

                        (그림 4.27 시리얼 엔코더 에러해제)

(3)	계속 에러 발생 시 모터(엔코더)를 교체 시험하십시오. 

서보 모터를 교체한 후 에러가 발생하지 않으면 서보모터의 불량입니다. 서보 모터를 정상품으로 교체하여 주십시오. 아래 그림은 HS165 로봇의 각 축 모터의 위치를 나타내고 있으며, 다른 로봇은 해당 기구 보수설명서를 참고하여 교체하시기 바랍니다.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                        (그림 4.28 HS165 로봇의 각 축 모터 위치)
[__SOURCE](4-servo-board-part/E02461.md)
# 4.9. E02461. (O축) 엔코더 과속 오류 (OS 비트 감지)

### 1. 개요
서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더 회전 속도가 허용 범위를 초과하여 OS(OverSpeed) 비트가 세트되었을 때 발생합니다. 이는 실제 과속 상황이거나, 신호 이상으로 잘못 감지되었을 수 있습니다.

엔코더로부터 수신된 데이터는 정상이나 엔코더가 스스로 내부상태를 감시한 결과 에러상태(OS)인 경우에 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1)	엔코더 공급전압을 확인하십시오.
(2)	엔코더 배선을 점검하십시오
(3)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.
(4)	계속 에러발생시 모터(엔코더)를 교체 시험하십시오. 
{% endhint %}

세부적인 점검방법은 "E02460 (O축) 엔코더 내부 회전값 오류(CE 비트 감지)"을 참조하십시오.

[__SOURCE](4-servo-board-part/E02462.md)
# 4.10. E02462. (O축) 엔코더 위치 정보 초기화되지 않음 (FS 비트 검지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더 내부에서 Full Absolute 상태에 도달하지 않아 정확한 위치 정보가 아직 확보되지 않을 때 발생합니다. 이는 엔코더 전원 인가 직후, 데이터 초기화 실패, 또는 백업 정보 손실로 인해 발생할 수 있습니다.

엔코더로부터 수신된 데이터는 정상이나 엔코더가 스스로 내부상태를 감시한 결과 에러상태(FS)인 경우에 발생할 수 있습니다.

FS(Full Absolute) : 해당 비트가 0이면 위치 데이터가 초기화 되지 않았거나, 백업 정보가 불완전한 상태. 해당 비트가 1이면 엔코더 내부 데이터가 완전하고 정상 상태임을 나타냅니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1)	엔코더 공급전압을 확인하십시오.
(2)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.
(3)	계속 에러발생시 모터(엔코더)를 교체 시험하십시오. 
{% endhint %}

세부적인 점검방법은 "E02460 (O축) 엔코더 내부 회전값 오류(CE 비트 감지)"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02463.md)
# 4.11. E02463. (O축) 엔코더 멀티턴 저장 오류 (ME 비트 감지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더 내부에서 배터리 백업 불량, 내부 저장 회로 오류, 전원 인가 중 예기치 않은 차단 등의 원인으로 멀티턴(회전수)가 정상적으로 저장되지 않아 ME 비트가 세트되었을때 발생합니다.

엔코더로부터 수신된 데이터는 정상이나 엔코더가 스스로 내부상태를 감시한 결과 에러상태(ME)인 경우에 발생할 수 있습니다.

### 2. 원인 및 점검
{% hint style="info" %}
(1)	엔코더 공급전압을 확인하십시오.
(2)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.
(3)	계속 에러발생시 모터(엔코더)를 교체 시험하십시오. 
{% endhint %}

세부적인 점검방법은 "E02460 (O축) 엔코더 내부 회전값 오류(CE 비트 감지)"을 참조하십시오.

[__SOURCE](4-servo-board-part/E02464.md)
# 4.12. E02464. (O축) 엔코더 배터리 이상 (BE 감지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더에 연결된 배터리 전압이 기준치 이하로 떨어지거나 연결에 문제가 발생하여 BE(Battery Error)가 세트되었을 경우 발생합니다.

엔코더로부터 수신된 데이터는 정상이나 엔코더가 스스로 내부상태를 감시한 결과 에러상태(BE)인 경우에 발생할 수 있습니다.

BE(Battery Error) : 엔코더 주전원 Off시 외부배터리전압이 3.1V이하로 되었던 경우에 발생.


### 2. 원인 및 점검

{% hint style="info" %}

(1)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.

(2)	엔코더 백업용 배터리 전압 확인하십시오.

(3)	엔코더 배터리 결선상태를 점검하십시오.

(4)	모터(엔코더)를 교체 시험하십시오. 

{% endhint %}

(1)	시리얼 엔코더 에러해제 후, 제어기 전원을 껏다카 다시 켜십시오.

에러해제 후, 주전원 OFF/ON시 계속 에러가 발생하면 모터(엔코더)교체 시험하십시오.
에러해제는 아래의 메뉴에서 실행합니다.
        
        시스템 -> 5.초기화 -> 4. 시리얼 엔코더 리셋 - 에러해제

![](../_assets/4.서보보드/엔코더_에러해제.png)

                        (그림 4.29 엔코더 에러 해제)

(2)	엔코더 배터리 전압을 확인하십시오. 
엔코더용 배터리는 3.6V 입니다. 이 전압이 3.0V~3.2V 로 저하되면 “W0104 ○축 엔코더Battery 전압저하입니다” 로 표시 됩니다. 이 경고가 발생할 때 엔코더용 배터리를 교환해야 합니다. 엔코더 배터리 교환은 반드시 제어기 전원이 ON되어 있는 상태에서 배터리를 교체해야 합니다. 이 상태에서 정상적인 엔코더 배터리로 교체하면 문제 없이 로봇을 계속 사용할 수 있습니다.

엔코더 배터리 교체시기를 지나서 엔코더용 배터리 전압이 2.5V~3.0V 가 되면 제어기 전원 ON시“E2470 ○축 엔코더 이상 : 엔코더 리셋 필요” 에러가 발생합니다. 이 에러가 발생하면 이미 엔코더의 위치데이터를 잃어버린 상태입니다. 엔코더 배터리를 교체하고 엔코더를 리셋 시킨 후에 축좌표계 수동 조작으로 로봇을 기준자세로 이동하여 해당 축의 엔코더 보정을 재실시 해야 합니다.

![](../_assets/4.서보보드/배터리_교환위치.png)

                         (그림 4.30 엔코더 배터리 교환 위치)

엔코더 리셋은 아래의 메뉴에서 실행합니다.

        시스템 -> 5. 초기화 -> 4. 시리얼 엔코더 리셋 - 엔코더 리셋

![](../_assets/4.서보보드/엔코더_리셋.png)

                         (그림 4.31 엔코더 리셋)

(3)	엔코더 배터리 결선 상태를 점검하십시오. 
엔코더 배터리 위치부터 모터까지 연결되는 배터리 결선 상태를 확인하십시오.


(4)	모터(엔코더)를 교체 시험하십시오. 
에러리셋후 주전원 OFF/ON시 계속 에러가 발생하면 모터(엔코더)교체 시험하십시오. 교체한 후 에러가 발생하지 않으면 서보모터의 불량입니다. 서보 모터를 정상품으로 교체하여 주십시오. 아래 그림은 HS165 로봇의 각 축 모터의 위치를 나타내고 있으며, 다른 로봇은 해당 기구 보수설명서를 참고하여 교체하시기 바랍니다.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                        (그림 4.32 HS165 로봇의 각 축 모터 위치)


[__SOURCE](4-servo-board-part/E02470.md)
# 4.13. E02470. (O축) 엔코더 이상: 엔코더 리셋 필요

### 1. 개요

엔코더가 모터의 위치데이터를 보존하기 위해서는 상시 엔코더에 전원이 공급되어야 합니다. 

엔코더의 전원은 제어기 전원을 ON시켜 두거나 엔코더용 백업 배터리에 의해서 전원이 공급됩니다. 만일 엔코더용 백업 배터리가 방전되어 있는 상태에서 제어기 전원을 OFF 시키면 엔코더가 위치데이터를 잃어버리기 때문에 에러가 발생합니다. 

마찬가지로 모터를 교체할 때에도 신규 모터의 엔코더는 이미 전원이 공급되지 않는 상태였기 때문에 동일한 에러가 발생합니다.
엔코더를 리셋시키면 해당 축의 기준위치 데이터가 변경되므로 반드시 축좌표계 수동 조작으로 로봇을 기준자세로 이동하여 해당 축의 엔코더 보정을 재실시해야 합니다. 

### 2. 원인 및 점검

{% hint style="info" %}
(1)	엔코더 배터리 전압을 확인하십시오.
(2)	엔코더 배터리 결선 상태를 점검하십시오.
(3)	모터를 교체 시험하십시오.
(4)	엔코더 리셋 이후에는 로봇 기준위치에서 엔코더 보정을 재실시해야 합니다.
{% endhint %}

(1)	엔코더 배터리 전압을 확인하십시오. 
엔코더용 배터리는 3.6V 입니다. 이 전압이 3.0V~3.2V 로 저하되면 “W0104 ○축 엔코더Battery 전압저하입니다” 로 표시 됩니다. 이 경고가 발생할 때 엔코더용 배터리를 교환해야 합니다. 엔코더 배터리 교환은 반드시 제어기 전원이 ON되어 있는 상태에서 배터리를 교체해야 합니다. 이 상태에서 정상적인 엔코더 배터리로 교체하면 문제 없이 로봇을 계속 사용할 수 있습니다.

엔코더 배터리 교체시기를 지나서 엔코더용 배터리 전압이 2.5V~3.0V 가 되면 “E2470 ○축 엔코더 이상 : 엔코더 리셋 필요” 에러가 발생합니다. 이 에러가 발생하면 이미 엔코더의 위치데이터를 잃어버린 상태입니다. 엔코더 배터리를 교체하고 엔코더를 리셋 시킨 후에 축좌표계 수동 조작으로 로봇을 기준자세로 이동하여 해당 축의 엔코더 보정을 재실시 해야 합니다.

![](../_assets/4.서보보드/배터리_교환위치.png)

                    (그림 4.34 엔코더 배터리 교환 위치)

엔코더 리셋은 아래의 메뉴에서 실행합니다.

            시스템 -> 5. 초기화 -> 4. 시리얼 엔코더 리셋

![](../_assets/4.서보보드/엔코더_리셋.png)

                    (그림 4.35 시리얼 엔코더 리셋)

(2)	엔코더 배터리 결선 상태를 점검하십시오. 

엔코더 배터리 위치부터 모터까지 연결되는 배터리 결선 상태를 확인하십시오.

(3)	모터를 교체 시험하십시오.

상기 조치로도 문제가 해결되지 않는다면 엔코더 자체 고장일 가능성이 높습니다. 모터를 교체 시험하십시오.

    

[__SOURCE](4-servo-board-part/E02630.md)
# 4.14. E02630. (O축) 위치편차 초과

### 1. 개요
로봇 구동 중 위치편차가 설정값을 초과할 경우 발생합니다. 서보제어에 의해 로봇 동작하는 중, 이동명령위치와 실제위치와의 차이가 너무 클 경우 서보보드는 이를 에러를 감지하고 로봇을 정지시킵니다.

### 2. 원인 및 점검
{% hint style="info" %}

(1)	에러가 발생한 축이 다른 설비와 기계적 간섭이 있는지 확인하십시오.
(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.
(3)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.
    개별 축 브레이크 해제 이상 점검
    브레이크용 전원이상 점검.
(4)	배선상태를 점검하십시오.
(5)	정격부하를 사용하지는 확인하십시오.
(6)	위치편차 설정 레벨을 확인하십시오.
(7)	서보 보드(BD640)와 main com의 버전을 확인하십시오. 
(8)	기타의 부품을 교체하십시오.
{% endhint %}

(1)	에러가 발생한 축이 다른 설비와 기계적 간섭이 있는지 확인하십시오.

로봇의 기구적 간섭 혹은 충돌이 있을 경우 이 에러가 발생할 수 있습니다. 제한영역을 벗어나 있을 경우에는 수동조작하여 안전영역으로 로봇을 이동시켜야 합니다.

(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.60 TP 로봇 모델 확인)
    TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.

(3)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.

해당 축 브레이크의 해제기능에 문제가 있거나 브레이크 해제전압의 이상일 수 있습니다.
 * 개별 축 브레이크 해제 이상 점검

    축 잠금 기능을 사용하여 해당 축 브레이크 해제 기능 작동을 확인하십시오.
확인 하려는 축을 제외하고 축 잠금을 한 뒤 모터 온/오프를 반복하여 기구부의 모터에서 브레이크 해제 소리(“딸깍”)가 들리는지 확인하십시오.

    축 잠금 기능을 사용하는 방법은 아래와 같습니다.
    
        시스템 -> 5. 초기화 -> 9. 축 잠금 설정 -> 확인 -> 개별 축 축잠금

![](../_assets/4.서보보드/축잠금1.png)

                    (그림 4.61 축 잠금 설정화면1)

![](../_assets/4.서보보드/축잠금2.png)

                    (그림 4.62 축 잠금 설정화면2)

![](../_assets/4.서보보드/축잠금3.png)

                    (그림 4.63 축 잠금 설정화면3)

    해당 축의 브레이크가 해제되지 않는다면 서보보드의 브레이크 출력상태를 확인해야 합니다. 브레이크 배선(CNB1, CNB7, CNB8 커넥터)를 제거하고 브레이크 전압을 출력하십시오. CNB1, CNB7 또는 CNB8 커넥터에서 해당 축의 브레이크 전압이 20V 이상으로 출력되는지 측정하십시오. 20V 이하의 전압으로 출력되는 축이 있다면 서보보드(BD640)의 고장이므로 고체하십시오.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (그림 4.64 CNB1,CNB7,CNB8 커넥터의 핀배치)

 * 브레이크용 전원이상 점검

    브레이크 전원 배선점검 순서는 다음과 같습니다.

    1차: 브레이크 전원 배선에 관련된 커넥터들의 접촉 불량여부를 점거하십시오.

    2차: 브레이크 전원 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 1:1로 체크하십시오.

    파워전장모듈 내부 배선을 점검하십시오. Hi6-T15 제어기는 파워전장모듈이 없으므로 해당 사항이 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.65 전장모듈 및 전장보드)

 * 서보보드(BD640)를 점검 하십시오.

    파워전장모듈이 정상이라면 서보보드에서 브레이크 전원(DC24V)을 측정하십시오. 아래 그림의 빨간색 구역에 테스트 포인트(PAD24V0BK1)의 측정 값이 DC24V 이상 되어야 정상입니다. 만약 20V 미만이라면 브레이크 전원을 생성하는 전원 장치의 이상입니다. 전장모듈을 교체하십시오.

    ![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (그림 4.66 서보보드 브레이크 전원)

(4)	배선상태를 점검하십시오.

모터배선(U, V, W상)이 올바르게 연결되어 있는지 확인하십시오.
또한 모터 배선이 다른 배선 또는 접지선(FG)과 단락되어 있는지 확인하십시오.

(5)	정격부하를 사용하는지 확인하십시오.

작업 물을 포함하여 전체무게가 정격부하를 초과하고 있다면 해당 로봇의 사양서를 참조하여 정격 이내로 부하를 조정하십시오.

(6)	위치편차 설정 레벨 오류

위치편차 설정치가 다음의 측정최대치 보다 작으면 설정치를 상향조정 하십시오.

             싸이클 이상 동작시킨 후의 위치편차 측정최대치x1.5
![](../_assets/4.서보보드/위치편차_모니터링_화면.png)

                (그림 4.67 위치편차 측정최대치 모니터링 화면)

![](../_assets/4.서보보드/위치편차_설정_변경.png)

                (그림 4.68 위치편차 설정 변경 화면)

(7)	서보 보드(BD640)와 main com의 버전을 확인하십시오.

서보 보드(BD640)와 main com버전의 호환성이 깨져 발생할 수 있습니다. 특히 모듈을 교체한 상황이라면 버전업을 진행하여 각 모듈의 버전을 현재 메인 com 버전에 맞춰주십시오. 각 모듈의 버전은 아래의 경로에서 확인할 수 있습니다.

                서비스 -> 7.시스템 진단 -> 1.시스템 버전

![](../_assets/4.서보보드/TP버전확인.png)

                (그림 4.69 TP의 각 모듈 버전 확인 창)

(8)	기타의 부품을 교체하십시오.

서보보드(BD640) → 서보구동장치 → 파워전장모듈 → 모터 순으로 교체하여 에러발생 여부를 확인하십시오.

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                (그림 4.70 N제어기 모터 및 구동 모듈)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                (그림 4.70 T제어기 모터 및 구동 모듈)




[__SOURCE](4-servo-board-part/E02631.md)
# 4.15. E02631. (O축) 속도별 위치편차 초과

### 1. 개요

조그 동작 또는 저속 동작 시 발생하는 위치편차가 설정치 보다 큽니다. 서보제어에 의한 로봇 동작 중 이동명령위치와 실제위치와의 차이가 너무 큰 경우, 서보보드는 서보연산 중 에러를 감지하고 로봇을 정지시킵니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	에러가 발생한 축이 다른 설비와 기계적 간섭이 있는지 확인하십시오.

(2)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.
	개별 축 브레이크 해제 이상 점검
	브레이크용 전원이상 점검.

(3)	배선상태를 점검하십시오.

(4)	정격부하를 사용하지는 확인하십시오.

(5)	위치편차 설정 레벨을 확인하십시오.

(6)	서보 보드(BD640)와 main com의 버전을 확인하십시오. 

(7)	기타의 부품을 교체하십시오.

{% endhint %}

세부적인 점검방법은 "E02630 (O축) 위치편차 초과"을 참조하십시오.
[__SOURCE](4-servo-board-part/E02632.md)
# 4.16. E02632. (O축) 위치편차초과 - 브레이크전압 저하

### 1. 개요

위치편차가 설정치 보다 큽니다. 서보제어에 의한 로봇 동작 중 이동명령위치와 실제위치와의 차이가 너무 큰 경우, 서보보드는 서보연산 중 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 위치편차가 크면서 브레이크전압 저하가 검지되었을 때 발생합니다.

### 2. 원인 및 점검

{% hint style="info" %}
(1)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.
    * 개별 축 브레이크 해제 이상 점검
    * 브레이크용 전원이상 점검
{% endhint %}

(1)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.

해당 축 브레이크의 해제기능에 문제가 있거나 브레이크 해제전압의 이상일 수 있습니다.
 * 개별 축 브레이크 해제 이상 점검

    축 잠금 기능을 사용하여 해당 축 브레이크 해제 기능 작동을 확인하십시오.
확인 하려는 축을 제외하고 축 잠금을 한 뒤 모터 온/오프를 반복하여 기구부의 모터에서 브레이크 해제 소리(“딸깍”)가 들리는지 확인하십시오.

    축 잠금 기능을 사용하는 방법은 아래와 같습니다.
        시스템 -> 5. 초기화 -> 9. 축 잠금 설정 -> 확인 -> 개별 축 축잠금

![](../_assets/4.서보보드/축잠금1.png)

                    (그림 4.71 축 잠금 설정화면1)

![](../_assets/4.서보보드/축잠금2.png)

                    (그림 4.72 축 잠금 설정화면2)

![](../_assets/4.서보보드/축잠금3.png)

                    (그림 4.73 축 잠금 설정화면3)

    해당 축의 브레이크가 해제되지 않는다면 서보보드의 브레이크 출력상태를 확인해야 합니다. 브레이크 배선(CNB1, CNB7, CNB8 커넥터)를 제거하고 브레이크 전압을 출력하십시오. CNB1, CNB7 또는 CNB8 커넥터에서 해당 축의 브레이크 전압이 20V 이상으로 출력되는지 측정하십시오. 20V 이하의 전압으로 출력되는 축이 있다면 서보보드(BD640)의 고장이므로 고체하십시오.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (그림 4.74 CNB1,CNB7,CNB8 커넥터의 핀배치)

 * 브레이크용 전원이상 점검

    브레이크 전원 배선점검 순서는 다음과 같습니다.

    1차: 브레이크 전원 배선에 관련된 커넥터들의 접촉 불량여부를 점거하십시오.

    2차: 브레이크 전원 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 1:1로 체크하십시오.

    파워전장모듈 내부 배선을 점검하십시오. Hi6-T15 제어기는 파워전장모듈이 없으므로 해당 사항이 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.75 전장모듈 및 전장보드)

 * 서보보드(BD640)를 점검 하십시오.

    파워전장모듈이 정상이라면 서보보드에서 브레이크 전원(DC24V)을 측정하십시오. 아래 그림의 빨간색 구역에 테스트 포인트(PAD24V0BK1)의 측정 값이 DC24V 이상 되어야 정상입니다. 만약 20V 미만이라면 브레이크 전원을 생성하는 전원 장치의 이상입니다. 전장모듈을 교체하십시오.

    ![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (그림 4.76 서보보드 브레이크 전원)

    

[__SOURCE](4-servo-board-part/E02633.md)
# 4.17. E02633. (O축) 위치편차 초과 - 부하추정 미실시

### 1. 개요
위치편차가 설정치 보다 큽니다. 서보제어에 의한 로봇 동작 중 이동명령위치와 실제위치와의 차이가 너무 큰 경우, 서보보드는 서보연산 중 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 위치편차가 크면서 부하추정이 미 실시 되었을 때 발생합니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	부하추정을 실시하고, 에러가 다시 발생 되는지 확인하십시오.

(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

{% endhint %}

(1)	부하추정을 실시하고, 에러가 다시 발생 되는지 확인하십시오.

부하를 확인하는 방법에는 계측기를 사용하는 방법이 가장 정확하지만 여의치 않을 경우에는 제어기 기능 중 부하추정 기능을 사용하여 확인할 수 있습니다. 부하추정 기능은 로봇 끝단에 설치되어 있는 툴에 대한 부분만 추정 가능합니다.

부하 추정 방법은 다음과 같습니다.
 * 부하추정 기능으로 들어갑니다.

        시스템 -> 6. 자동 캘리브레이션 -> 4. 부하추정 기능

![](../_assets/4.서보보드/부하추정1.png)

                    (그림 4.77 부하 추정 기능1)

![](../_assets/4.서보보드/부하추정2.png)

                    (그림 4.78 부하 추정 기능2)

![](../_assets/4.서보보드/부하추정3.png)

                    (그림 4.79 부하 추정 기능3)

 * 부하추정 기능을 사용하여 부하 추정 후 저장할 툴 번호를 선택합니다.

![](../_assets/4.서보보드/부하추정4.png)

                    (그림 4.80 부하 추정 기능4)

 * 정상 운전을 클릭하여 수행합니다.

    모터 On 스위치를 누르고 데드맨을 잡은 후 정상운전을 클릭합니다.

![](../_assets/4.서보보드/부하추정5.png)

                    (그림 4.81 부하 추정 기능5)

* 부하 추정 운전이 완료되면 추정 결과가 화면에 보여집니다.

![](../_assets/4.서보보드/부하추정6.png)

                    (그림 4.82 부하 추정 기능6)

(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.83 로봇 모델 확인)

    TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.

    
[__SOURCE](4-servo-board-part/E02634.md)
# 4.18. E02634. (O축) 위치편차 초과 - 저온 마찰 증가

### 1. 개요

위치(속도)편차가 설정치 보다 큽니다. 서보제어에 의한 로봇 동작 중 이동명령위치와 실제위치와의 차이가 너무 큰 경우, 서보보드는 서보연산 중 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 위치편차가 크면서 엔코더 온도가 저온일 때 발생합니다.
통상 저온시(엔코더 5℃이하)는, 구리스 점성에 의한 마찰성분이 증가해서 정상시보다 부가적인 토크가 필요하므로 로봇을 고속으로 동작시키면 본 에러가 발생 할 수 있습니다.

### 2. 원인 및 점검
{% hint style="info" %}
(1)	엔코더 온도가 정상치(약 15℃ 이상)가 될 때까지 저속구동(재생속도 30% 이하) 시킨 후, 정상속도로 재 가동하십시오. 
(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.
{% endhint %}

(1)	엔코더 온도가 정상치(약 15℃ 이상)가 될 때까지 저속구동(재생속도 30% 이하) 시킨 후, 정상속도로 재 가동하십시오

![](../_assets/4.서보보드/엔코더온도및재생속도.png)

                    (그림 4.84 엔코더 온도 확인 화면)


(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.85 로봇 모델 확인)

    TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.
[__SOURCE](4-servo-board-part/E02650.md)
# 4.19. E02650. (O축) 모터 과부하

### 1. 개요

모터 또는 구동장치가 무리하게 동작되고 있습니다. 모터 또는 구동장치가 설정치 보다 무리하게 동작하게 되면, 서보보드는 에러를 감지하고 로봇을 정지시킵니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	부하가 로봇의 정격 이하로 설치되어 있는지 확인하십시오.

(2)	로봇 동작 중 충돌요소가 있는지 점검하십시오.

(3)	축 브레이크가 정상적으로 작동하는지 확인하십시오.

(4)	모터 케이블 및 커넥터 연결 상태를 점검하십시오.

(5)	서보보드를 교체하여 이상여부를 점검하십시오.

(6)	구동부가 정상적으로 작동하는지 점검하십시오.

{% endhint %}

(1)	부하가 로봇의 정격 이하로 설치되어 있는지 확인하십시오.

로봇 최대 사양 이하의 부하가 설치되어 있는지 확인하십시오. 사양을 초과할 경우 에러가 발생할 수 있습니다. (여기서 부하란, 로봇 끝단에 설치되는 툴뿐만 아니라 로봇 기구에 부착되는 케이블 및 다른 모든 부분이 포함됩니다.)

부하를 확인하는 방법에는 계측기를 사용하는 방법이 가장 정확하지만 여의치 않을 경우에는 제어기 기능 중 부하추정 기능을 사용하여 확인할 수 있습니다. 부하추정 기능은 로봇 끝단에 설치되어 있는 툴에 대한 부분만 추정 가능합니다.

부하 추정 방법은 다음과 같습니다.

* 부하추정 기능으로 들어갑니다.

        시스템 -> 6. 자동 캘리브레이션 -> 4. 부하추정 기능

![](../_assets/4.서보보드/부하추정1.png)

                    (그림 4.86 부하 추정 기능1)

![](../_assets/4.서보보드/부하추정2.png)

                    (그림 4.87 부하 추정 기능2)

![](../_assets/4.서보보드/부하추정3.png)

                    (그림 4.88 부하 추정 기능3)

 * 부하추정 기능을 사용하여 부하 추정 후 저장할 툴 번호를 선택합니다.

![](../_assets/4.서보보드/부하추정4.png)

                    (그림 4.89 부하 추정 기능4)

 * 정상 운전을 클릭하여 수행합니다.

    모터 On 스위치를 누르고 데드맨을 잡은 후 정상운전을 클릭합니다.

![](../_assets/4.서보보드/부하추정5.png)

                    (그림 4.90 부하 추정 기능5)

* 부하 추정 운전이 완료되면 추정 결과가 화면에 보여집니다.

![](../_assets/4.서보보드/부하추정6.png)

                    (그림 4.91 부하 추정 기능6)

(2)	로봇 동작 중 충돌요소가 있는지 점검하십시오.

로봇 작업 영역에 로봇과 간섭 또는 충돌하는 부분이 있는지 확인하십시오. 로봇이 다른 기구물과 간섭이 발생할 경우 에러가 발생할 수 있습니다. 이 경우, 작업 프로그램을 수정하여 간섭이 발생하지 않도록 합니다.

(3) 브레이크 해제가 정상적으로 작동되는지 확인하십시오.

해당 축 브레이크의 해제기능에 문제가 있거나 브레이크 해제전압의 이상일 수 있습니다.
 * 개별 축 브레이크 해제 이상 점검

    축 잠금 기능을 사용하여 해당 축 브레이크 해제 기능 작동을 확인하십시오.
확인 하려는 축을 제외하고 축 잠금을 한 뒤 모터 온/오프를 반복하여 기구부의 모터에서 브레이크 해제 소리(“딸깍”)가 들리는지 확인하십시오.

    축 잠금 기능을 사용하는 방법은 아래와 같습니다.
        시스템 -> 5. 초기화 -> 9. 축 잠금 설정 -> 확인 -> 개별 축 축잠금

![](../_assets/4.서보보드/축잠금1.png)

                    (그림 4.92 축 잠금 설정화면1)

![](../_assets/4.서보보드/축잠금2.png)

                    (그림 4.93 축 잠금 설정화면2)

![](../_assets/4.서보보드/축잠금3.png)

                    (그림 4.94 축 잠금 설정화면3)

    해당 축의 브레이크가 해제되지 않는다면 서보보드의 브레이크 출력상태를 확인해야 합니다. 브레이크 배선(CNB1, CNB7, CNB8 커넥터)를 제거하고 브레이크 전압을 출력하십시오. CNB1, CNB7 또는 CNB8 커넥터에서 해당 축의 브레이크 전압이 20V 이상으로 출력되는지 측정하십시오. 20V 이하의 전압으로 출력되는 축이 있다면 서보보드(BD640)의 고장이므로 고체하십시오.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (그림 4.95 CNB1,CNB7,CNB8 커넥터의 핀배치)

 * 브레이크용 전원이상 점검

    브레이크 전원 배선점검 순서는 다음과 같습니다.

    1차: 브레이크 전원 배선에 관련된 커넥터들의 접촉 불량여부를 점거하십시오.

    2차: 브레이크 전원 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 1:1로 체크하십시오.

    파워전장모듈 내부 배선을 점검하십시오. Hi6-T15 제어기는 파워전장모듈이 없으므로 해당 사항이 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.96 전장모듈 및 전장보드)

 * 서보보드(BD640)를 점검 하십시오.

    파워전장모듈이 정상이라면 서보보드에서 브레이크 전원(DC24V)을 측정하십시오. 아래 그림의 빨간색 구역에 테스트 포인트(PAD24V0BK1)의 측정 값이 DC24V 이상 되어야 정상입니다. 만약 20V 미만이라면 브레이크 전원을 생성하는 전원 장치의 이상입니다. 전장모듈을 교체하십시오.

    ![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (그림 4.97 서보보드 브레이크 전원)

(4)	모터 케이블 및 커넥터 연결 상태를 점검하십시오.
 
 * 제어기 내부 배선을 점검 하십시오.
 * 제어기와 로봇 간의 배선을 점검하십시오.
 * 로봇 기내 배선을 점검하십시오.

(5) 서보보드를 교체하여 이상여부를 확인하십시오.

서보보드에 이상이 있을 경우 에러가 발생할 수 있습니다. 보드를 교체하여 확인하십시오.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.98 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.99 T제어기 서보보드 교체)

(6)	구동부가 정상적으로 작동하는지 확인하십시오.

해당축의 구동부(모터, 감속기)가 정상적으로 작동하는지 확인하십시오.

![](../_assets/4.서보보드/축구동부_en.png)

                    (그림 4.100 구동부 정상동작 확인)
[__SOURCE](4-servo-board-part/E02651.md)
# 4.20. E02651. (O축) 모터 과부하 - 브레이크전압 저하

### 1. 개요

모터 또는 구동장치가 무리하게 동작되고 있습니다. 모터 또는 구동장치가 설정치 보다 무리하게 동작하게 되면, 서보보드는 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 과부하 상태이면서 브레이크전압 저하가 검지되었을 때 발생합니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.

    * 개별 축 브레이크 해제 이상 점검
    * 브레이크용 전원 이상 점검

{% endhint %}

(1)	브레이크 해제가 정상적으로 작동되는지 확인하십시오.

해당 축 브레이크의 해제기능에 문제가 있거나 브레이크 해제전압의 이상일 수 있습니다.
 * 개별 축 브레이크 해제 이상 점검

    축 잠금 기능을 사용하여 해당 축 브레이크 해제 기능 작동을 확인하십시오.
확인 하려는 축을 제외하고 축 잠금을 한 뒤 모터 온/오프를 반복하여 기구부의 모터에서 브레이크 해제 소리(“딸깍”)가 들리는지 확인하십시오.

    축 잠금 기능을 사용하는 방법은 아래와 같습니다.

        시스템 -> 5. 초기화 -> 9. 축 잠금 설정 -> 확인 -> 개별 축 축잠금

![](../_assets/4.서보보드/축잠금1.png)

                    (그림 4.101 축 잠금 설정화면1)

![](../_assets/4.서보보드/축잠금2.png)

                    (그림 4.102 축 잠금 설정화면2)

![](../_assets/4.서보보드/축잠금3.png)

                    (그림 4.103 축 잠금 설정화면3)

    해당 축의 브레이크가 해제되지 않는다면 서보보드의 브레이크 출력상태를 확인해야 합니다. 브레이크 배선(CNB1, CNB7, CNB8 커넥터)를 제거하고 브레이크 전압을 출력하십시오. CNB1, CNB7 또는 CNB8 커넥터에서 해당 축의 브레이크 전압이 20V 이상으로 출력되는지 측정하십시오. 20V 이하의 전압으로 출력되는 축이 있다면 서보보드(BD640)의 고장이므로 고체하십시오.

![](../_assets/4.서보보드/CNB_커넥터_배치.png)

                    (그림 4.104 CNB1,CNB7,CNB8 커넥터의 핀배치)

 * 브레이크용 전원이상 점검

    브레이크 전원 배선점검 순서는 다음과 같습니다.

    1차: 브레이크 전원 배선에 관련된 커넥터들의 접촉 불량여부를 점거하십시오.

    2차: 브레이크 전원 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 1:1로 체크하십시오.

    파워전장모듈 내부 배선을 점검하십시오. Hi6-T15 제어기는 파워전장모듈이 없으므로 해당 사항이 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.105 전장모듈 및 전장보드)

 * 서보보드(BD640)를 점검 하십시오.

    파워전장모듈이 정상이라면 서보보드에서 브레이크 전원(DC24V)을 측정하십시오. 아래 그림의 빨간색 구역에 테스트 포인트(PAD24V0BK1)의 측정 값이 DC24V 이상 되어야 정상입니다. 만약 20V 미만이라면 브레이크 전원을 생성하는 전원 장치의 이상입니다. 전장모듈을 교체하십시오.

    ![](../_assets/4.서보보드/서보보드_브레이크전원_측정.png)

                    (그림 4.106 서보보드 브레이크 전원)

[__SOURCE](4-servo-board-part/E02652.md)
# 4.21. E02652. (O축) 모터 과부하 - 부하추정 미실시

### 1. 개요

모터 또는 구동장치가 무리하게 동작되고 있습니다. 모터 또는 구동장치가 설정치 보다 무리하게 동작하게 되면, 서보보드는 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 과부하 상태이면서 부하추정이 미 실시 되었을 때 발생합니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	부하추정을 실시하고, 에러가 다시 발생 되는지 확인하십시오.

{% endhint %}

(1)	부하추정을 실시하고, 에러가 다시 발생 되는지 확인하십시오.

부하를 확인하는 방법에는 계측기를 사용하는 방법이 가장 정확하지만 여의치 않을 경우에는 제어기 기능 중 부하추정 기능을 사용하여 확인할 수 있습니다. 부하추정 기능은 로봇 끝단에 설치되어 있는 툴에 대한 부분만 추정 가능합니다.

부하 추정 방법은 다음과 같습니다.
 * 부하추정 기능으로 들어갑니다.

        시스템 -> 6. 자동 캘리브레이션 -> 4. 부하추정 기능

![](../_assets/4.서보보드/부하추정1.png)

                    (그림 4.107 부하 추정 기능1)

![](../_assets/4.서보보드/부하추정2.png)

                    (그림 4.108 부하 추정 기능2)

![](../_assets/4.서보보드/부하추정3.png)

                    (그림 4.109 부하 추정 기능3)

 * 부하추정 기능을 사용하여 부하 추정 후 저장할 툴 번호를 선택합니다.

![](../_assets/4.서보보드/부하추정4.png)

                    (그림 4.110 부하 추정 기능4)

 * 정상 운전을 클릭하여 수행합니다.

    모터 On 스위치를 누르고 데드맨을 잡은 후 정상운전을 클릭합니다.

![](../_assets/4.서보보드/부하추정5.png)

                    (그림 4.111 부하 추정 기능5)

* 부하 추정 운전이 완료되면 추정 결과가 화면에 보여집니다.

![](../_assets/4.서보보드/부하추정6.png)

                    (그림 4.112 부하 추정 기능6)

[__SOURCE](4-servo-board-part/E02653.md)
# 4.22. E02653. (O축) 모터 과부하 - 저온 마찰 증가

### 1. 개요

모터 또는 구동장치가 무리하게 동작되고 있습니다. 모터 또는 구동장치가 설정치 보다 무리하게 동작하게 되면, 서보보드는 에러를 감지하고 로봇을 정지시킵니다.
이 에러는 과부하 상태이면서 엔코더 온도가 저온일 때 발생합니다.
통상 저온시(엔코더 5℃이하)는, 구리스 점성에 의한 마찰성분이 증가해서 정상시보다 부가적인 토크가 필요하므로 로봇을 고속으로 동작시키면 본 에러가 발생 할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	엔코더 온도가 정상치(약 15℃ 이상)가 될 때까지 저속구동(재생속도 30% 이하) 시킨 후, 정상속도로 재 가동하십시오 

{% endhint %}

(1)	엔코더 온도가 정상치(약 15℃ 이상)가 될 때까지 저속구동(재생속도 30% 이하) 시킨 후, 정상속도로 재 가동하십시오

![](../_assets/4.서보보드/엔코더온도및재생속도.png)

                    (그림 4.113 엔코더 온도 확인 화면)


[__SOURCE](4-servo-board-part/E02670.md)
# 4.23. E02670. (O축) 지령치 이상

### 1. 개요

메인보드와 서보보드간 통신이상이나 급격한 모션변화에 의해서 에러가 발생할 수 있습니다. 보드간 통신 문제가 발생하면 정상적인 지령이 메인보드에서 서보보드로 전달되지 못하며, 이때 잘못된 지령으로 로봇이 이상 동작을 할 수 있으므로 에러를 발생시키고 로봇을 정지시킵니다. 또한 급격한 모션의 경우 구동장치가 위치 지령을 추종하지 못하는 경우가 발생되므로 에러를 발생시키고 로봇을 정지시킵니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	메인보드와 서보보드가 올바로 설치되어 있는지 점검하십시오.

    * 보드가 올바르게 설치되어 있는지 점검하십시오.
    * 보드 이상여부를 점검하십시오.

(2)	로봇이 급격하게 동작하는 작업 프로그램이 있는지 점검하십시오.

{% endhint %}


(1)	메인보드와 서보보드가 올바르게 설치되어 있는지 점검하십시오.

메인보드와 서보보드가 랙에 올바로 설치되어 있지 않거나 보드에 문제가 있으면 통신에 문제가 되어 에러가 발생할 수 있습니다.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ 경고(Warning)

**이전 작업 프로그램을 보호하기 위해서 보드를 랙에서 제거하기 전에 반드시 메인보드의 모든 파일을 USB 메모리를 이용하여 백업하시기 바랍니다.**

</div>

---

USB 메모리에 메인보드 파일을 백업하는 방법은 다음과 같습니다.

![](../_assets/4.서보보드/USB연결.png)

                    (그림 4.114 TP USB 연결)
                
USB가 TP에서 인식되면 화면 위에 다음과 같은 아이콘으로 표시됩니다.

![](../_assets/4.서보보드/USB인식.png)

                    (그림 4.115 TP USB 인식)

파일을 백업하기 위해서 아래의 경로로 진입합니다.

            서비스 -> 5. 파일관리

![](../_assets/4.서보보드/백업1.png)

                    (그림 4.116 백업 단계1)

![](../_assets/4.서보보드/백업2.png)

                    (그림 4.117 백업 단계2)

Project 폴더를 USB에 복사합니다.

    * 보드가 올바르게 설치되어 있는지 점검하십시오.

        보드 간 인터페이스인 EtherCAT 케이블 연결 상태를 점검하십시오. 제거 후 다시 설치하시기 바랍니다.

![](../_assets/4.서보보드/보드_인터페이스_en.png)

                    (그림 4.118 N제어기 EtherCAT 케이블 연결)

![](../_assets/4.서보보드/T제어기-보드인터페이스_en.png)

                    (그림 4.119 T제어기 EtherCAT 케이블 연결)


    * 보드 이상여부를 점검하십시오.
        보드 이상 여부를 판단하기 위해서 보드 교체를 하시기 바랍니다.

        

(2)	로봇이 급격하게 동작하는 작업 프로그램이 있는지 점검하십시오.
로봇 동작 중 급격하게 모션이 변하는 구간에서 에러가 발생하는지 확인하십시오.
만약, 급격한 모션 중에 에러가 발생한다면 작업 프로그램의 수정이 필요합니다.

급격한 모션에서 에러가 발생하는 원인은 다음과 같습니다. 작업 프로그램을 수행할 때 짧은 구간을 이동하면서 불가피하게 로봇의 자세가 많이 틀어지는 경우가 있습니다. 이 때, 로봇의 축 속도가 갑자기 높아지게 되고 이를 서보보드에서 추종하지 못할 경우 에러가 발생하게 됩니다. 해결하는 방법은 자세가 급격히 변하는 지점의 티칭 포인트를 수정하거나 로봇 자세를 바꾸어 주면 됩니다. 


[__SOURCE](4-servo-board-part/E02680.md)
# 4.24. E02680. (O축) 최고속 초과

### 1. 개요

로봇 축의 속도가 최고속을 초과하여 동작하였습니다. 로봇이 정상적으로 제어되지 않는 상태이므로 에러로 처리하여 로봇을 정지시킵니다.

메인보드에서 서보보드로 지령을 보낼 때에는 최고속을 초과하지 않도록 제한된 지령을 보냅니다. 이렇게 만들어진 지령을 로봇이 쫓아가지 못하다가 속도에 overshoot가 발생할 때 최고속 초과 에러가 발생할 수 있습니다.


### 2. 원인 및 점검

{% hint style="info" %}

(1)	툴 데이터가 정확히 입력되어 있는지 확인하십시오.

(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

(3)	서보 보드(BD640)와 main com의 버전을 확인하십시오.

(4)	로봇 자세가 특이점 근방인지 확인하십시오.

(5)	부가축은 가감속 파라미터 설정값과 동작중 부하율을 확인하십시오.

(6)	작업 프로그램을 조정하십시오.

{% endhint %}

(1)	툴 데이터가 정확히 입력되어 있는지 확인하십시오. 

툴 중량이나 이너셔가 제어기에 등록되어 있는 값과 크게 다르면 로봇 제어 성능이 악화되면서 최고속 초과에러가 발생할 수 있습니다. 툴중량과 이너셔는 아래 메뉴에서 툴 번호에 따라 등록할 수 있습니다.

                시스템 -> 3. 로봇파라미터 -> 툴 데이터

![](../_assets/4.서보보드/툴데이터.png)

                    (그림 4.120 툴 데이터 확인)

툴 중량이나 이너셔를 자동으로 설정하기 위해서는 아래의 메뉴에서 부하추정 기능을 사용할 수 있습니다. 

* 부하추정 기능으로 들어갑니다.

        시스템 -> 6. 자동 캘리브레이션 -> 4. 부하추정 기능

![](../_assets/4.서보보드/부하추정1.png)

                    (그림 4.121 부하 추정 기능1)

![](../_assets/4.서보보드/부하추정2.png)

                    (그림 4.122 부하 추정 기능2)

![](../_assets/4.서보보드/부하추정3.png)

                    (그림 4.123 부하 추정 기능3)

 * 부하추정 기능을 사용하여 부하 추정 후 저장할 툴 번호를 선택합니다.

![](../_assets/4.서보보드/부하추정4.png)

                    (그림 4.124 부하 추정 기능4)

 * 정상 운전을 클릭하여 수행합니다.

    모터 On 스위치를 누르고 데드맨을 잡은 후 정상운전을 클릭합니다.

![](../_assets/4.서보보드/부하추정5.png)

                    (그림 4.125 부하 추정 기능5)

* 부하 추정 운전이 완료되면 추정 결과가 화면에 보여집니다.

![](../_assets/4.서보보드/부하추정6.png)

                    (그림 4.126 부하 추정 기능6)

(2)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.127 로봇 모델 확인)

    TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.

(3)	서보 보드(BD640)와 main com의 버전을 확인하십시오. 

서보 보드(BD640)와 main com버전의 호환성이 깨져 발생할 수 있습니다. 특히 모듈을 교체한 상황이라면 버전업을 진행하여 각 모듈의 버전을 현재 메인 com 버전에 맞춰주십시오.

각 모듈의 버전은 아래 경로에서 확인할 수 있습니다.

                서비스 -> 7. 시스템 진단 -> 1. 시스템 버전


![](../_assets/4.서보보드/TP버전확인.png)

                    (그림 4.127 모듈 버전 확인)


(4)	로봇 자세가 특이점 근방인지 확인하십시오. 

특이점 근방의 자세에서 PtP 보간이 아닌 L 보간이나 C 보간을 실행하면 에러가 발생할 수 있습니다. 특이점은 B축이 0deg에 가까운 경우와 손목부 중심이 S축 회전 중심축과 가까울 때 발생합니다. 특이점 근방을 지나야 할 때에는 해당 스텝을 PtP 보간으로 변경하여 주십시오.

![](../_assets/4.서보보드/로봇특이자세.png)

                    (그림 4.128 특이점 자세 확인)

(5)	부가축은 가감속 파라미터 설정값과 동작중 부하율을 확인하십시오. 

부가축 가감속 파라미터의 최고속이 너무 높거나 가속시간이 너무 짧아서 모터토크가 부족할 수 있습니다. 로봇 동작중 부하율을 관찰하면서 I/Ip 최고속을 낮추거나 가속시간을 크게 조정해야 합니다.

                시스템 -> 3. 로봇 파라미터 -> 34. 가감속 파라미터

![](../_assets/4.서보보드/부가축가감속.png)

                    (그림 4.129 부가축 가감속 확인)

(6)	작업 프로그램을 조정하십시오. 

작업 프로그램의 해당 스텝 혹은 직전 스텝의 스텝 조건을 변경하십시오. 첫 번째로 “Acc=0”으로 변경해 보고, 두 번째는 스텝의 속도를 낮춰 보고, 세 번째는 이동 경로에 스텝을 하나 추가해 보는 방식으로 프로그램의 조건을 변경하십시오.


[__SOURCE](4-servo-board-part/E02780.md)
# 4.25. E02780. (O축) 서보락 유지 불가 - 전류 생성 이상

### 1. 개요

모터 또는 구동장치에 구동을 위한 전류가 공급되지 못하고 있습니다. 로봇 또는 구동장치를 동작시키기 위해 만들어진 전류가 정상적으로 공급되지 못하고 있습니다. 이와 같은 경우 제어기에서는 에러를 감지하며 브레이크 해제를 막고 모터 또는 구동장치에 공급되는 전류를 차단합니다. 모터와 제어기 간의 연결 이상, 배선 불량, 또는 전류 생성 회로의 문제로 판단할 수 있습니다. 또한 로봇 기종 등록 오류로 인해 모터 제어에 필요한 파라미터(Gain 및 최대 전류)가 실제 모터와 일치하지 않아 에러가 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

(2)	모터 파워 라인 및 엔코더 통신 라인을 점검하십시오.

    * 로봇과 제어기를 연결하는 배선을 확인하십시오.
    * 로봇 기내 배선을 확인하십시오.
    * 제어기 내부 배선을 확인하십시오.

(3) 제어기 내부 서보보드와 앰프보드간의 케이블을 점검하십시오.

(4) 기타의 부품을 교체하십시오.

(5) BD640 전원 계통 라인 점검(노이즈, 배선 short 등의 이슈)

{% endhint %}

(1)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.130 로봇 모델 확인)

(2)	모터 파워 및 엔코더 통신 라인을 점검하십시오.

제어기 전원을 Off하고 해당축 구동장치의 U, V, W를 분리하여 각 상의 단락 및 단선 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 상의 배선을 1:1로 체크하십시오. 엔코더 통신 선의 단선 여부를 확인하십시오.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ 경고(Warning)

**전원이 투입된 상태에서 점검시 감전의 위험이 있으므로 주의하십시오**

</div>

---

    * 로봇과 제어기를 연결하는 배선을 확인하십시오
        제어기와 로봇 또는 구동장치를 연결하는 배선을 제거하여 각 상(U상, V상, W상)이 서로 또는 접지와 단락된 곳이 있는지 확인하시고, 단락된 곳이 있으면 해당하는 배선을 교체하셔야 합니다.


![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (그림 4.131 N제어기 로봇 간 배선)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (그림 4.132 T제어기 로봇 간 배선)

    * 로봇 내부의 기내배선을 점검하십시오.
        로봇 내부에 모터와 연결되어 있는 배선에 단락 또는 잘못 배선된 곳이 있는지 점검이 필요합니다.

![](../_assets/4.서보보드/로봇기내배선.png)

                    (그림 4.133 로봇 기내 배선)


    * 제어기 내부 배선을 점검하십시오.
        제어기 내부에 앰프와 설치되어 있는 배선 점검이 필요합니다.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (그림 4.134 N제어기 내부 배선 점검)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (그림 4.135 T제어기 내부 배선 점검)


(2)	제어기 내부 서보 보드와 앰프보드 간의 커넥터(Board to Board)을 점검하십시오.

서보보드와 앰프보드 간의 연결 및 체결되는 커넥터(보드 to 보드)의 설치가 올바른지 점검하십시오. 체결 상태가 불량일 경우 해당 에러가 발생할 수 있습니다.

![](../_assets/4.서보보드/서보보드_앰프보드_b2b_en.png)

                    (그림 4.136 N제어기 서보 보드와 앰프보드의 연결)

![](../_assets/4.서보보드/T제어기_서보보드_앰프보드_en.png)

                    (그림 4.137 T제어기 서보 보드와 앰프보드의 연결)

(3)	기타의 부품을 교체하십시오.

서보보드(BD640) → 앰프 보드 → 와이어 하네스 → 모터 → PSM의 순으로 교체하여 에러발생 여부를 확인하십시오.

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                    (그림 4.138 N제어기 구동 부품)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                    (그림 4.138 T제어기 구동 부품)

(5) BD640 전원 계통 라인을 점검하십시오.

해당에러와 함께 E64003 서보 보드(BD640) 상태 이상 검지, E02764 세이프티 보드(BD632)에러, E02500 회생방전 저항 과열, E02504 AC 입력 전압 초과, E02505 AMP PN 과전압 또는 방전 이상, E02506 AMP PN 저전압, E62850 MCON1 입력 배선 노이즈, E62851 MCON2 입력 배선 노이즈 등의 에러가 같이 발생한다면 BD640 및 BD632의 전원 계통(노이즈, 와이어하네스 배선 상태 등)을 점검하여야 합니다.

공정 내 배선 Short 발생으로 보드 24V 전원 및 그라운드 상태 이상으로 IO 신호들에 대한 에러가 다발로 발생할 수 있습니다. BD640 및 BD632의 전원 계통 (노이즈, 와이어하네스 배선 상태 등)의 점검이 필요합니다. 
[__SOURCE](4-servo-board-part/E02781.md)
# 4.26. E02781. (O축) 서보락 유지 불가 - 파라미터 이상

### 1. 개요

모터 또는 구동장치에 구동을 위한 전류가 공급되지 못하고 있습니다. 로봇 또는 구동장치를 동작시키기 위해 만들어진 전류가 정상적으로 공급되지 못하고 있습니다. 이와 같은 경우 제어기에서는 에러를 감지하며 브레이크 해제를 막고 모터 또는 구동장치에 공급되는 전류를 차단합니다. 모터와 제어기 간의 연결 이상, 배선 불량, 또는 전류 생성 회로의 문제로 판단할 수 있습니다. 또한 로봇 기종 등록 오류로 인해 모터 제어에 필요한 파라미터(Gain 및 최대 전류)가 실제 모터와 일치하지 않아 에러가 발생할 수 있습니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

(2)	모터 파워 라인 및 엔코더 통신 라인을 점검하십시오.

    * 로봇과 제어기를 연결하는 배선을 확인하십시오.
    * 로봇 기내 배선을 확인하십시오.
    * 제어기 내부 배선을 확인하십시오.

(3) 제어기 내부 서보보드와 앰프보드간의 케이블을 점검하십시오.

(4) 기타의 부품을 교체하십시오.

{% endhint %}

(1)	로봇 기종이 맞게 설정되어 있는지 확인하십시오.

TP화면상의 등록된 로봇기종과 실제 설치된 로봇이 일치하는지 확인하십시오.

![](../_assets/4.서보보드/로봇모델확인.png)

                    (그림 4.130 로봇 모델 확인)

(2)	모터 파워 및 엔코더 통신 라인을 점검하십시오.

제어기 전원을 Off하고 해당축 구동장치의 U, V, W를 분리하여 각 상의 단락 및 단선 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 상의 배선을 1:1로 체크하십시오. 엔코더 통신 선의 단선 여부를 확인하십시오.

---

<div style="border: 2px solid #f5c542; background-color: #fff8e1; padding: 1em; border-radius: 8px;">

### ⚠️ 경고(Warning)

**전원이 투입된 상태에서 점검시 감전의 위험이 있으므로 주의하십시오**

</div>

---

    * 로봇과 제어기를 연결하는 배선을 확인하십시오
        제어기와 로봇 또는 구동장치를 연결하는 배선을 제거하여 각 상(U상, V상, W상)이 서로 또는 접지와 단락된 곳이 있는지 확인하시고, 단락된 곳이 있으면 해당하는 배선을 교체하셔야 합니다.


![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (그림 4.131 N제어기 로봇 간 배선)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (그림 4.132 T제어기 로봇 간 배선)

    * 로봇 내부의 기내배선을 점검하십시오.
        로봇 내부에 모터와 연결되어 있는 배선에 단락 또는 잘못 배선된 곳이 있는지 점검이 필요합니다.

![](../_assets/4.서보보드/로봇기내배선.png)

                    (그림 4.133 로봇 기내 배선)


    * 제어기 내부 배선을 점검하십시오.
        제어기 내부에 앰프와 설치되어 있는 배선 점검이 필요합니다.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (그림 4.134 N제어기 내부 배선 점검)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (그림 4.135 T제어기 내부 배선 점검)


(2)	제어기 내부 서보 보드와 앰프보드 간의 커넥터(Board to Board)을 점검하십시오.

서보보드와 앰프보드 간의 연결 및 체결되는 커넥터(보드 to 보드)의 설치가 올바른지 점검하십시오. 체결 상태가 불량일 경우 해당 에러가 발생할 수 있습니다.

![](../_assets/4.서보보드/서보보드_앰프보드_b2b_en.png)

                    (그림 4.136 N제어기 서보 보드와 앰프보드의 연결)

![](../_assets/4.서보보드/T제어기_서보보드_앰프보드_en.png)

                    (그림 4.137 T제어기 서보 보드와 앰프보드의 연결)

(3)	기타의 부품을 교체하십시오.

서보보드(BD640) → 앰프 보드 → 와이어 하네스 → 모터 → PSM의 순으로 교체하여 에러발생 여부를 확인하십시오.

![](../_assets/4.서보보드/N제어기_모터및구동장치_en.png)

                    (그림 4.138 N제어기 구동 부품)

![](../_assets/4.서보보드/T제어기_모터및구동장치_en.png)

                    (그림 4.138 T제어기 구동 부품)

[__SOURCE](4-servo-board-part/E02472.md)
# 4.27. E02472. (O축) 엔코더 과열 검지 (OH 비트 감지)

### 1. 개요

서보보드에서는 서보 모터의 제어를 수행하기 위해 엔코더와 시리얼통신을 하여 주기적으로 엔코더 데이터를 수신합니다, 해당 에러는 엔코더로부터 OH 비트를 감지하였을 때 발생합니다.

OH비트는 엔코더 내부 온도가 허용 범위를 초과하였을 때 세트 됩니다. 임계값이 되는 기준 온도는 약 90도 에서 100도 이며 이는 엔코더 모델 별로 사양이 상이하기 때문에 제조사 매뉴얼을 확인하십시오. 


### 2. 원인 및 점검

{% hint style="info" %}

(1)	모터(엔코더)를 교체 시험하십시오

(2)	운전 조건(속도, 부하 등)을 확인하십시오

(3)	엔코더 주변 환경 온도를 점검하십시오

(4)	서보 보드(BD640)를 교체하십시오.

{% endhint %}

(1)	모터(엔코더)를 교체 시험하십시오.

서보 모터를 교체한 후 에러가 발생하지 않으면 서보모터의 불량입니다. 서보 모터를 정상품으로 교체하여 주십시오. 아래 그림은 HS165 로봇의 각 축 모터의 위치를 나타내고 있으며, 다른 로봇은 해당 기구 보수설명서를 참고하여 교체하시기 바랍니다.

![](../_assets/4.서보보드/로봇_모터_위치.png)

                    (그림 4.36 모터(엔코더) 교체 위치)

(2)	운전 조건(속도, 부하 등)을 확인하십시오.

Job 프로그램을 동작시키면서 포화되는 엔코더 온도를 확인하십시오. 엔코더 온도는 아래와 같이 확인할 수 있습니다.

            엔지니어링 모드 -> 창조정 -> 시스템 특성 -> 시스템 특성 리스트 - 모터/엔코더

![](../_assets/4.서보보드/엔코더온도.png)

                    (그림 4.37 엔코더 온도 확인)

(3)	엔코더 주변 환경 온도를 점검하십시오.

외부 온도로 인하여 엔코더 내부 온도가 증가하여 에러가 발생할 수 있습니다.

(4)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보 보드의 엔코더 데이터 수신부의 고장으로 판단할 수 있습니다.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.38 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.39 T제어기 서보보드 교체)

[__SOURCE](4-servo-board-part/E02554.md)
# 4.28. E02554. 초기 충전 릴레이 동작 이상

### 1. 개요

서보 보드(BD640)에서는 모터 전원 인가 과정에서 초기 충전 릴레이를 동작시키고 초기 충전 릴레이의 동작상태를 감시하여 에러를 발생시킵니다. 초기 충전 릴레이는 돌입 전류를 억제하는 기능을 하므로, 릴레이 동작 이상 시 안전을 위하여 에러가 발생하고 모터 전원 인가를 차단합니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	모니터링 계통을 점검하십시오.

(2)	전장 보드를 점검 하십시오.

(3)	서보보드(BD640)을 점검 하십시오.

{% endhint %}

(1)	모니터링 계통을 점검하십시오.

초기 충전 저항과 릴레이가 설치되어 있는 전장모듈(PSM or PDM)과 모니터링 신호를 수집하는 서보보드(BD640) 간의 케이블링을 확인합니다. 케이블 이름은 CNPRC 이고 서보보드 하단 왼쪽면을 통하여 전장 모듈로 들어 갑니다. 이 케이블의 커넥터 접속상태를 점검하십시오. Hi6-T 제어기의 경우, 해당 케이블배선이 없으므로 해당 사항 없습니다.

![](../_assets/4.서보보드/CNPRC케이블.png)

                     (그림 4.40 CNPRC 케이블 연결)

(2)	전장보드를 점검하십시오

Hi6-N 제어기의 경우, 서보보드와 전장보드, 케이블 배선에 문제가 있을 수 있으므로 점검 또는 교체하십시오. Hi6-T 제어기의 경우, 해당 케이블배선이 없으므로 해당 사항 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.41 전장모듈 내부 전장보드)

(3)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보 보드의 엔코더 데이터 수신부의 고장으로 판단할 수 있습니다.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.42 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.43 T제어기 서보보드 교체)
    

[__SOURCE](4-servo-board-part/E02560.md)
# 4.29. E02560. 브레이크 전원 이상

### 1. 개요

브레이크용 전원(24V)를 서보보드에서 감시하는 중, 설정된 정상 전압 범위를 벗어나는 경우 에러를 발생시킵니다.브레이크 전원이 정상적으로 공급되지 않으면, 로봇 축 고정이 불안정해질 수 있으므로 서보 제어기는 이를 감지하여 에러를 발생시키고 로봇을 안전하게 정지시킵니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	브레이크 전원(24V)가 정상적으로 공급되고 있는지 확인하십시오

(2)	브레이크 전원 케이블의 단선 또는 접촉 불량 상태를 확인하십시오

(3)	서보 보드(BD640)을 교체 하십시오.

{% endhint %}

(1)	브레이크 전원(24V)가 정상적으로 공급되고 있는지 확인하십시오

브레이크 전원 배선점검 순서는 다음과 같습니다.

1차: 브레이크 전원 배선에 관련된 커넥터들의 접촉 불량여부를 점거하십시오.

2차: 브레이크 전원 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 1:1로 체크하십시오.

    * 파워전장모듈 내부 배선을 점검하십시오.
        Hi6-T15 제어기는 파워전장모듈이 없으므로 해당 사항이 없습니다.

![](../_assets/4.서보보드/전장모듈내부_전장보드.png)

                    (그림 4.44 파워 전장 모듈)

(2)	브레이크 전원 케이블의 단선 또는 접촉 불량 상태를 확인하십시오.

제어기 내부 배선을 점검 하십시오. Hi6-N 제어기의 경우, CNPB1(BD640) 커넥터와 CNPB1(전장보드) 커넥터 간의 배선을 점검하십시오. Hi6-T15제어기의 경우, CNPB1(BD602T) 커넥터와 브레이크 SMPS 출력 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/N제어기_브레이크_전원케이블.png)

                    (그림 4.45 N제어기 브레이크 전원 점검)

![](../_assets/4.서보보드/T제어기_브레이크전원.png)

                    (그림 4.45 T제어기 브레이크 전원 점검)

(3)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보 보드의 엔코더 데이터 수신부의 고장으로 판단할 수 있습니다.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.46 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                 (그림 4.47 T제어기 서보보드 교체)

[__SOURCE](4-servo-board-part/E02570.md)
# 4.30. E02570. (O축) 브레이크 출력 이상

### 1. 개요

서보 보드(BD640)에서는 브레이크 작동 명령과 브레이크 피드백 회로의 신호를 감시하는 중, 두 신호가 불일치 할 경우 에러를 발생시킵니다. 브레이크 회로의 출력이 정상적으로 이루어지지 않으면 브레이크 작동에 실패할 수 있으므로 서보 보드에서는 이를 감지하여 로봇을 정지시킵니다. 

### 2. 원인 및 점검

{% hint style="info" %}

(1)	브레이크 배선을 점검하십시오.

(2)	서보보드(BD640)를 점검 하십시오.

{% endhint %}

(1)	브레이크 배선을 점검하십시오.

브레이크 배선점검 순서는 다음과 같습니다.

1차: 브레이크 배선에 관련된 커넥터들의 접촉 불량여부를 점검하십시오.

2차: 브레이크 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 축의 배선을 1:1로 체크하십시오.

3차: 브레이크 배선을 교체시험 하십시오.

브레이크 배선이 단선되지 않고 접촉불량, 브레이크 파워선과 타 전력선 또는 로봇 본체 금속부위와의 접촉 등의 현상이 있을 경우에는 단락유무 검사로는 검사할 수 없으므로 배선 교체시험을 하여 주십시요.

    * 제어기 내부 배선을 점검하십시오.
        Hi6-N 제어기의 경우, CNB1(BD640) 커넥터와 CMC1, CMC2 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (그림 4.54 N제어기 브레이크 출력 배선)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (그림 4.55 T제어기 브레이크 출력 배선)
    
    * 제어기와 로봇간의 배선을 점검하십시오.
        Hi6-N제어기의 경우, CMC1과 CMR1 그리고 CMC2와 CMR2 간의 배선을 Hi6-T15제어기의 경우, CMEC1과 CMER1 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (그림 4.56 N제어기 브레이크 출력 배선)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (그림 4.57 T제어기 브레이크 출력 배선)

(2)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보 보드의 엔코더 데이터 수신부의 고장으로 판단할 수 있습니다.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.58 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.59 T제어기 서보보드 교체)

[__SOURCE](4-servo-board-part/E02564.md)
# 4.31. E02564. (O축) 브레이크 출력 과전류 검지

### 1. 개요

서보 보드(BD640)에서는 브레이크 출력 회로의 과전류 상태를 감시하고 있으며, 출력 회로에 연결된 보호 회로(IC)로부터 Fault 신호가 감지되면 과전류 상황으로 판단하여 에러를 발생시킵니다. 이러한 이상 상태가 발생하면 브레이크 제어의 신뢰성을 보장할 수 없기 때문에, 서보 보드는 즉시 이를 감지하고 로봇을 안전하게 정지시킵니다.

### 2. 원인 및 점검

{% hint style="info" %}

(1)	브레이크 배선을 점검하십시오.

(2)	서보보드(BD640)를 점검 하십시오.

{% endhint %}

(1)	브레이크 배선을 점검하십시오.

브레이크 배선점검 순서는 다음과 같습니다.

1차: 브레이크 배선에 관련된 커넥터들의 접촉 불량여부를 점검하십시오.

2차: 브레이크 배선의 단락 유무를 점검하십시오. 멀티미터(테스터기)와 같은 장비를 이용하여 각 축의 배선을 1:1로 체크하십시오.

3차: 브레이크 배선을 교체시험 하십시오.

브레이크 배선이 단선되지 않고 접촉불량, 브레이크 파워선과 타 전력선 또는 로봇 본체 금속부위와의 접촉 등의 현상이 있을 경우에는 단락유무 검사로는 검사할 수 없으므로 배선 교체시험을 하여 주십시요.

    * 제어기 내부 배선을 점검하십시오.
        Hi6-N 제어기의 경우, CNB1(BD640) 커넥터와 CMC1, CMC2 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/N제어기_브레이크_출력_배선_en.png)

                    (그림 4.48 N제어기 브레이크 출력 배선)

![](../_assets/4.서보보드/T제어기_브레이크_출력_배선.png)

                    (그림 4.49 T제어기 브레이크 출력 배선)
    
    * 제어기와 로봇간의 배선을 점검하십시오.
        Hi6-N제어기의 경우, CMC1과 CMR1 그리고 CMC2와 CMR2 간의 배선을 Hi6-T15제어기의 경우, CMEC1과 CMER1 간의 배선을 점검하십시오.

![](../_assets/4.서보보드/N제어기_로봇_제어기_브레이크_배선.png)

                    (그림 4.50 N제어기 브레이크 출력 배선)

![](../_assets/4.서보보드/T제어기_로봇_제어기_브레이크배선.png)

                    (그림 4.51 T제어기 브레이크 출력 배선)

(2)	서보보드를 교체 시험하십시오. 

서보 보드를 교체한 후 에러가 발생하지 않으면 서보 보드의 엔코더 데이터 수신부의 고장으로 판단할 수 있습니다.

![](../_assets/4.서보보드/N제어기_서보보드_교체_en.png)

                    (그림 4.52 N제어기 서보보드 교체)

![](../_assets/4.서보보드/T제어기_서보보드_교체_en.png)

                    (그림 4.53 T제어기 서보보드 교체)
[__SOURCE](5-communication/README.md)
# 5. 통신
[__SOURCE](5-communication/E29003.md)
# 5.1. E29003 전장 보드 통신 오류 (EtherCAT 연결 끊김)

### 1. 개요

전장 보드 통신 오류 (EtherCAT 연결 끊김)가 발생하였습니다. 메인제어모듈(H6COM-T)과 서보보드(BD640), 안전보드(BD632)간의 통신이 끊어졌습니다.

### 2. 원인

{% hint style="info" %}

(1)	보드 간 통신 케이블 결선 상태 확인.<br>
(2)	서보보드(BD640)를 점검하십시오.<br>
(3)	안전보드(BD632)를 점검하십시오.<br>

{% endhint %}


### (1)	보드 간 통신 케이블 결선 상태 확인.

### [각 모듈간(메인제어모듈(H6COM-T), 서보보드(BD640), 안전보드(BD632)) Ethernet 케이블 결선 상태 확인]

![](../_assets/5-Communication/E29003/그림1.png)<br>

1)	점검 대상<br>
A.	메인제어모듈 (H6COM-T) ↔ 서보보드 (BD640) 간 Ethernet 케이블<br>
B.	서보보드 (BD640) ↔ 안전보드 (BD632) 간 Ethernet 케이블<br>
2)	점검 항목<br>
A.	케이블 양쪽 커넥터가 확실히 체결되어 있는지 확인<br>
B.	케이블에 단선, 압착 손상, 꺾임, 파손이 없는지 육안 점검<br>
C.	커넥터 핀(단자)에 녹, 오염, 휘어짐이 없는지 확인<br>
3)	점검 방법<br>
A.	전원을 OFF한 상태에서 케이블 분리 및 재삽입 수행<br>
B.	삽입 시 '딸깍' 소리가 나도록 완전히 체결<br>
C.	필요한 경우 예비 케이블로 교체 후 재시도<br>
D.	연결 순서 및 올바른 LAN Port와 연결되어 있는지 재확인<br>
4)	추가 확인<br>
A.	서보보드(BD640), 안전보드(BD632) 장치 자체에 Link/Act LED 상태 확인<br>
- 정상: 녹색(좌) 점멸, 황색(우) 점등 <br>
- 비정상: 녹색(좌) & 황색(우) 꺼짐 또는 점등 상태 유지<br>
![](../_assets/5-Communication/E29003/그림2.png)<br>
B.	반복적으로 끊김이 발생할 경우, 케이블 내부 단선 가능성 고려 → 케이블 교체 필요<br>
C.	이더넷 커넥터(PCB 단자부) 손상 가능성도 점검<br>

 
### (2) 서보보드(BD640)를 점검하십시오.
#### [서보 보드(BD640)를 점검하는 방법]
![](../_assets/5-Communication/E29003/그림3.png)<br> 

1) 전원 상태 확인<br>
   LED1과 LED2가 초록색으로 점멸하는지 확인하십시오. <br>
   7-Segment에 P001 혹은 P002로 표기되는지 확인하십시오.<br>

2) 정상 부팅 상태 확인<br>
   메인제어모듈 (H6COM-T)이 완전히 부팅되고 난 후(전원투입후 약 50초 정도 소요) <br>7-Segment에 P002로 표기되어야함.<br>

1-2) 가 모두 정상임에도 이더캣 통신 연결에 문제가 있는 경우 보드를 교체 하십시오.

 
### (3) 안전보드(BD632)를 점검하십시오.

#### [안전보드(BD632)를 점검하는 방법]
![](../_assets/5-Communication/E29003/그림4.png)<br> 
 
1)	전원 상태를 확인하는 방법<br>
A.	위 그림의 두개의 LED가 녹색 점등 상태 인지를 확인<br>
B.	전원 LED가 적색 또는 소등인 경우 표시된 퓨즈가 정상 상태인지를 확인한다.<br>
C.	퓨즈가 끊겼다면 퓨즈를 교체한다.<br>

2)	모터온시 전원이 불안정한 상태인지 확인<br>
A.	모터온시에 전원 LED가 녹색 점등 상태 인지를 확인한다. <br>
B.	모터온 순간 적색으로 변하거나 소등되다면 모터온시 전원이 불안정한 상태 임<br>

3)	전원 상태가 불안정한 경우<br>
A.	전원 커넥터 체결 상태 확인<br>
B.	전원 케이블 점검<br>
C.	안전보드(BD632) 접지 상태 점검 (접지 케이블, 접지 단자 체결 상태)<br>

4)	안전보드가 정상 부팅 상태인지를 확인<br>
A.	메인제어모듈 (H6COM-T)이 완전히 부팅되고 난 후(전원투입후 약 50초 정도 소요)<br> 7-Segment의 표시가 ‘S’자로 2개가 표시 되어야 함.<br>

5)	1)~4)의 점검사항이 모두 이상이 없는 경우에도 통신에 문제가 있다면 안전보드(BD632)를 교체하십시오.<br>

[__SOURCE](5-communication/E29016.md)
# 5.2. E29016 전장보드 통신(EtherCAT) 마스터 연결 끊김 발생

### 1. 개요

전장보드 통신(EtherCAT) 마스터와 연결되는 첫번째 장치와의 연결이 끊어 졌습니다.

### 2. 원인

{% hint style="info" %}

(1)	보드 간 통신 케이블 결선 상태 확인.
(2)	서보보드(BD640)를 점검하십시오.

{% endhint %}

### (1) 보드 간 통신 케이블 결선 상태 확인.

#### [각 모듈간(메인제어모듈(H6COM-T), 서보보드(BD640)) Ethernet 케이블 결선 상태 확인]
![](../_assets/5-Communication/E29016/그림1.png)<br> 

1)	점검 대상
A.	메인제어모듈 (H6COM-T) ↔ 서보보드 (BD640) 간 Ethernet 케이블
2)	점검 항목
A.	케이블 양쪽 커넥터가 확실히 체결되어 있는지 확인
B.	케이블에 단선, 압착 손상, 꺾임, 파손이 없는지 육안 점검
C.	커넥터 핀(단자)에 녹, 오염, 휘어짐이 없는지 확인
3)	점검 방법
A.	전원을 OFF한 상태에서 케이블 분리 및 재삽입 수행
B.	삽입 시 '딸깍' 소리가 나도록 완전히 체결
C.	필요한 경우 예비 케이블로 교체 후 재시도
D.	연결 순서 및 올바른 LAN Port와 연결되어 있는지 재확인
4)	추가 확인
A.	서보보드(BD640) 장치 자체에 Link/Act LED 상태 확인
- 정상: 녹색(좌) 점멸, 황색(우) 점등 <br>
- 비정상: 녹색(좌) & 황색(우) 꺼짐 또는 점등 상태 유지<br>
![](../_assets/5-Communication/E29016/그림2.png)<br>
B.	반복적으로 끊김이 발생할 경우, 케이블 내부 단선 가능성 고려 → 케이블 교체 필요<br>
C.	이더넷 커넥터(PCB 단자부) 손상 가능성도 점검<br>

 
### (2) 서보보드(BD640)를 점검하십시오.
#### [서보 보드(BD640)를 점검하는 방법]
![](../_assets/5-Communication/E29016/그림3.png)<br> 

1) 전원 상태 확인<br>
   LED1과 LED2가 초록색으로 점멸하는지 확인하십시오. <br>
   7-Segment에 P001 혹은 P002로 표기되는지 확인하십시오.<br>

2) 정상 부팅 상태 확인<br>
   메인제어모듈 (H6COM-T)이 완전히 부팅되고 난 후(전원투입후 약 50초 정도 소요) <br>
   7-Segment에 P002로 표기되어야함.<br>

1-2) 가 모두 정상임에도 이더캣 통신 연결에 문제가 있는 경우 보드를 교체 하십시오.

[__SOURCE](appendices/README.md)
# Appendices

  



[__SOURCE](appendices/rules-occupational-safety.md)
# Rules on Occupational Safety and Health Standards and Safety Inspection Notification
This industrial robot shall be installed in consideration of the inspection requirements specified in the Rules on Occupational Safety and Health Standards and the Safety Inspection Notification, where applicable.

"[Rules on Occupational Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/korean/README)"

[__SOURCE](quality-assurance.md)
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/korean/README)"
