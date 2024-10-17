# ARM Mini Projects

This repository contains repos of my embedded systems ARM mini-projects. In this repo, you find demo videos of them running with brief explanations in arabic. For non-arabic speakers, don't worry you can find a description for all projects below.

## Projects Description

### Project 1: External Interrupts
This project uses external interrupts to control an array of LEDs connected to Port A. The microcontroller (STM32) is set up with two push buttons, each mapped to an external interrupt line. Pressing one button turns all the LEDs on, while the second button toggles the LEDs sequentially with a delay. To make this, I configured RCC, NVIC, and sysclock (system clock).

### Project 2: LED Matrix Text Display
This project uses a matrix of LEDs to display a scrolling text message. The program initializes the system clock and GPIO ports, then displays the text entered by the user. Its logic works as shift register. What makes this project unique is its versatility as it does not display predefined text but rather it can shift frames of any input character. 

### Project 3: UART-Controlled RGB LEDs
The system initializes USART1, allowing users to send commands to control three LEDs: red, green, and blue. Users can toggle the LEDs on and off using the UART terminal by sending characters ('r', 'g', 'b', 'o'). The project showcases the initialization and configuration of system clocks, GPIO pins, UART transmission, and interrupts. It also features callback functions to handle USART interrupts.

### Project 4: DMA vs CPU Speed Comparison
The efficiency of the Direct Memory Access (DMA) controller is compared to CPU-based data transfer in this project. While the CPU handles the copying of array1 to array2, the DMA is responsible for transferring data between array3 and array4. GPIO pins are used to signal the completion of each process, with the DMA signaling through an interrupt callback function. Spoiler: the DMA was much faster XD