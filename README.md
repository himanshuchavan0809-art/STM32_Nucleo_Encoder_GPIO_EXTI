# STM32_Nucleo_Encoder_GPIO_EXTI
Code for STM32F446RET6 to get encoder counts using GPIO Interrupts

This project demonstrates how to read a quadrature encoder using GPIO external interrupts (EXTI) on the STM32F446RET6.

Instead of using hardware timer encoder mode, this approach:

1. Detects signal changes via interrupts on GPIO pins
2. Determines direction using software logic
3. Updates encoder count manually

This method is useful when timers are unavailable or when you need custom decoding logic.

Features

1. Uses GPIO EXTI interrupts (no timer encoder mode)
2. Software-based quadrature decoding
3. Direction detection (CW / CCW)
4. Lightweight and flexible
5. Works on any interrupt-capable GPIO pins 
