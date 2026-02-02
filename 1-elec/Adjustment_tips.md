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

