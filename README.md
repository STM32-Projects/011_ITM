# Instrumentation Trace Macrocell(ITM)

To illustrate the use of ITM mechanism for stm32f446re(Nucleo)

The main uses of ITM include:

1. Support printf style debugging.
2. Trace OS and application events.
3. Emit diagnostic system information.

This is implemented by making use of the 3rd pin(SWO Trace Pin) in SWD(Serial Wire Debug) interface for printf style debugging.

The following changes are reuired to implement printf style debugging with ITM

1. Enable SWV in project configurations(Debugger Tab)
2. Update syscalls.c with ITM_SendChar() function to write toITM specific reggisters	

If you want to see the outputs from ITM unit, you need to enable SWV ITM Data Console as follows:

Window -> Show View -> SWV -> SWV ITM Data Console
