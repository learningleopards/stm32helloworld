- 👋 **Group Name:** Learning Leopards
- 👀 **Group Members:** Deveepria A/P Sankaran, Nur Irdina binti Mohd Shahrir, Thulasy A/P Chandran
- 🌱 **Task description:-** UART, or universal asynchronous receiver-transmitter, is one of the most common device-todevice communication protocols.
The UART interface transmits data asynchronously and does not use a clock signal to
synchronize the transmitter and receiver devices. USART (Universal Synchronous/Asynchronous Receiver/Transmitter) is an extension of UART
that allows for synchronous transmission via a dedicated clock wire. USART, rather than plain
UART, is now fairly common on modern microcontrollers. STM32 microcontrollers include a variable number of USARTs that can operate in both synchronous and asynchronous modes. The USART2 of the target MCU is connected to the ST-LINK interface on all Nucleo-64 boards. We configured the UART first add stm32f4xx_hal_uart.c and stm32f4xx_hal_uart.h files into the project then uncomment the HAL_UART_MODULE_ENABLED in stm32f4xx_hal_conf.h file this will include
the UART source files into the project. On the Nucleo-F446RE, the UART lines used to communicate with the host computer are connected to the programming chip next to the USB connector. To view data sent from the UART, a serial terminal program PuTTY. In order to use the UART or USART, the GPIO PA2 and PA3 is involved since port pins must be configured for the alternate function. The code prints Hello World! on the terminal. It waits for 1 second, then repeats forever. The output on the PuTTY terminal as below.
![image](https://user-images.githubusercontent.com/92903308/211154410-f7a135f4-aed7-4a74-815b-35996fa53933.png)



- 📫 **References:** Lecture Note, Chapter 10: Serial Interfacing https://wiki.st.com/stm32mcu/wiki/STM32StepByStep:Step3_Introduction_to_the_UART https://www.youtube.com/watch?v=Kdn2-XSqVGY
