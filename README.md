# FHTW_BIC_MCSD_Assign3 Description:

ADC/DAC Task
The purpose of this task is to learn to interface analog signals with the digital domain.

Task Description
Let the user control the brightness of the blue LED (LED_ABRG, A3) on the Click Shield by use of the potentiometer (RV1, A6). To that end, use a timer to trigger ADC conversions of the potentiometer pin. In the ADC ISR read out the value and drive the DAC connected to the blue LED accordingly. The main loop should be empty (apart from optional power-saving and debugging instructions) and everything should be driven by interrupts and trigger events. Choose a suitable period for the timer to make the update rate fast enough for humans but not too fast to overburden the CPU with excessive interrupt handling.

Also, make sure to use the whole range of the pot to control the comparably small range of DAC values that lead to visible changes of the LED. To that end, determine the DAC values to create the minimal and maximal brightness and scale the input values from the ADC accordingly.

Hints
The only IRQ that needs to be enabled is that of the ADC.

Don’t forget to start all necessary peripherals before entering the main loop.

# Points:

7/10
