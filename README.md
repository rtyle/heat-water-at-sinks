# heat-water-at-sinks
SmartThings SmartApp to run a hot water recirulation pump when needed.

The pump must be able to be turned on and off as a switch.
This can often be done by plugging the pump into a smart outlet.

In order to avoid running the pump when it is dry, the SmartApp can be configured with a number of valves that will cause the pump to be turned off if any are closed.

Otherwise, the pump will be run when needed as configured by a number of triggers.
Each trigger includes a threshold temperature specification, a temperature sensor and a number of switches.
The pump will be turned on if, for any of the triggers, the sensor measures temperature below the threshold and any of its switches are on.

This works well with something like the [Watts 500800 Instant Hot Water Recirculating System](https://www.amazon.com/dp/B000E78XHG) that has been enhanced with temperature measurement capabilities on each valve.
By characterizing the threshold temperature when the valve opens, the **heat-water-at-sinks** SmartApp can be configured to make sure that the pump is not run when it would not be effective (when the valve is closed). Smart switches are also added to indicate need. For example. if your nearby sink and/or shower light switches are smart, they can be used to suggest such.
