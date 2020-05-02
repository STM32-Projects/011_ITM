# Instrumentation Trace Macrocell(ITM)

To illustrate the use of ITM mechanism for stm32f446re(Nucleo)

The main uses of ITM include:

1. Support printf style debugging.
2. Trace OS and application events.
3. Emit diagnostic system information.

This is implemented by making use of the 3rd pin(SWO Trace Pin) in SWD(Serial Wire Debug) interface for printf style debugging.
