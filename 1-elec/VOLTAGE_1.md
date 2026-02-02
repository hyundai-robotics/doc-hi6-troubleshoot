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
