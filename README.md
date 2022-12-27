# Switched capacitor multilevel inverter (17Level)

<img src="https://github.com/ShahinSabour/multilevel_inverter_17Level/blob/main/images/17%20level%20inverter.png">

## Abstract

This structure offers multiple features of the conventional multilevel structures. Moreover, regarding the provided output voltage levels, the proposed structure exploits a new quasi-resonant basic module which helps to diminish circuit cost and complexity using fewer power components. In the proposed structure, the balancing of capacitors voltages is achieved by series and parallel connection with the voltage source and without the need to employ a complicated control system. In order to obtain higher voltage levels at the inverter ac side, a developed H-bridge is used in which the basic module is extended horizontally in separate cells on either side. Through a quasiresonant inductor deployment in the basic module, current spikes of capacitors are filtered which overwhelms decreasing of capacitor value and also lengthening the capacitor lifetime besides decreasing electromagnetic interference.

Read the complete paper here:
https://onlinelibrary.wiley.com/doi/10.1002/2050-7038.12478

## The proposed inveter in Matlab/Simulink

Each cell is depicted in the below figure. This structure consists of two power switches,
one capacitor, and one diode. When S1 (cell 1) is on, the capacitor is charged. On the
other hand, when S2 is off, and S1 is on, the capacitor is discharged on the load.
Moreover, for increasing output voltage, capacitors are connected in series and parallel. In charging time, capacitors
are parallel, and the equivalent of these capacitors is in series with a quasi-resonant inductance. Here, the cells
play a vital role in lessening current spikes of capacitors.
Also, the simulated structure consists of a extended H-bridge connected to cells
on both sides. Each cells and exnted H-bridge provide positive voltage levels. To achieve higher voltages and also to produce zero and negative levels, a extended H-bridge is utilized, which consists of the switches T1, T2, T3, T4, T5, and T6.
<img src="https://github.com/ShahinSabour/multilevel_inverter_17Level/blob/main/images/Circuit_.png">

## Modulation Starategy

Different modulation strategies are employed in multilevel converters to yield the output voltage waveforms. These
methods can be classified into two main categories; High-frequency modulation (HFM) and fundamental frequency
modulation (FFM). In this structure, an FFM method is used for switching and producing an output voltage. In the proposed extended structure, there are
two cells. 50v is the output voltage of cell one and 150v is the output voltage of cell two which are shown in below figures.

<img src="https://github.com/ShahinSabour/multilevel_inverter_17Level/blob/main/images/Pulses%20diagram%202.png">
Inside the subsystems, we have the below logic:
<img src="https://github.com/ShahinSabour/multilevel_inverter_17Level/blob/main/images/Pulses%20logic.png">
