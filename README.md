# ES Diploma
## Module 2: Data Structures, Algorithms and Computer Architecture
### Part 1: Data Structures
Intro to data structure
Linked Lists
- Linked Lists vs. Array
- Implementations of Linked Lists
- Insert Node
- Traverse through List
- Delete Node
Reverse List
Doubly Linked Lists
Stack
- PUSH elements
- POP elements
Queue
### Part 2: Algorithms
#### Sorting
Introduction to Sorting
- Selection Sorting Algorithm
- Bubble Sorting Algorithm
- Other Techniques Overview
			Searching
				Introduction to searching
				Linear Search
				Binary Search
				Other Techniques Overview
		Part 3: Computer System Organizations
			Intro to Computer System
			Processors
				CPU Organizaiton
					ALU
					CU
						PC
						IR
					Data Path
				Instruction Execution Cycle (Fetch, Decode, Execute)
				RISC vs. CISC
				Pipe-lining Concept
				Muti-processor Concepts
			Primary Memory
				Primary Memory Types
					RAM
						SRAM
						DRAM
					NVM
						ROM
						PROM
						EPROM
						EEPROM
						Data Flash
					Cache Memory
				Memory Addesses
				Big/Little Endian  
			Buses
				Address Bus
				Data Bus
				Control Bus
				Von Neumann vs. Harvard Architecture
	Module 1: Intro to Embedded & C Programming
		Part 1: Introduction to Embedded Systems
			ES Definition
			ES Characteristics
			General System vs. Embedded System
			Embedded System Applications
			Embedded System Design
				Trade off between HW and SW
				SW (pros and cons)
				HW (pros and cons)
				Embedded System Design Steps
			ES HW
				Processing Engines
				MCU vs. MPU
				MCU Components
					CPU
					Memory Units
					Buses
					IO
					Timers
					Watchdog Timers
					Interrupt Circuitry
					Clock
					Other Components
						Communication
							USART
							SPI
							I2C
							CAN
							LIN
						Sensing
							ADC
							Analog Comparator 
						Storage
				MCU Clocks
					Types
					Sources
					More complex (ARM, PLL)
				MCU Power Management
					Power Management Features (Why in Embedded?)
					Low Power Modes
			ES Constraints
				Deadlines (Maximum Execution Time)
					Operating System Constraints
				Communication Constraints
				Memory Consumption
				MCU Resources
			Selection of Microcontroller
				MCU Vendors
				MCU IDEs
			Embedded System Market
				HW Market
				SW Market
				Embedded Market in Egypt
		Part 2: Solid C Programming
			1- Choosing and Installing IDE
				What's IDE?
				Currently Available IDEs
				Eclipse Download and Install
			3. C Data Types, Operators and Expressions
				Data Types
					Basic Data types
					Constatns
						Escape character
					Declarations
					Casting
				Operators
					Arithmetic Operators (+,-,*,/,%)
					(++, --) operators
					Relational Operators
					Logical Operators ( AND , OR , NOT ) 
					Bitwise Operators ( & , | , ^ , << , >> , ~ )
					Conditional Operator (Ternary) ()?:
					sizeof( ) operator
					Operator Precedence Rules
			4. Control Flow
				Conditional
					If, else if, else
					Switch
				Loops
					While
					Do While
					For
					Break; Continue;
					Goto Labels
						Spaghetti Vs. Structured Code
			5. Functions
				Basics of functions
				Function Declaration (Prototype) and Definition
				Call by Value vs. Call by reference
				Static local variables, register keyword
				Recursion
			6.Arrays
				Array definition and Multi-dimension Arrays
				Arrays and functions (passing, returning)
				Strings (characters array)
			7. Pointers
				Pointer and Addresses
				Dereferencing 
				Pass by value vs. Pass by reference (address)
				Pointers and arrays
				Pointer Arithmetic
				Why using pointers over arrays in loops?
				Pointer to functions
				Complex pointers
			8. Structure and User-defined Data Types
				need for complex data types
				struct keyword
				Arrays of structs
				Pointers to structs (*will be discussed in dynamic memory allocation*)
				struct usage with functions (why?)
				Typedef (user-defined types)
				Struct bit fileds
				Union
			9. Dynamic Memory Allocation
				Dynamic vs. static memory allocation
				malloc, calloc, realloc and free
				Advantages, disadvantages
			10- Modularity and Program Structure
				C Preprocessors 
					include
					macro like functions
					conditional inclusion
				.h and .c files
				overview the executing process
				conventions to write library
					.h file 
						prototypes
						extern variables
					.c files
						global variables
						function definitions
			11- Important Notes (Bonus Topics) 
				Declaration Vs. Definition for Variables and Functions
				What does the compiler actually do? (Compilation Process)
				Storage Classes
					auto, register, static, extern
				Pointer Reading
				Applications in which unions are helpful (IPV4)
				Command Line Arguments
	Module 3: Microcontroller Drivers Interfacing
		Part 1: Interfacing Basic Drivers
			AVR Architecture
			Getting Started
				Basic Connection (Crystal and Biasing)
				Generating Hex File 
				Programmer
			GPIO
				Input (Switch)
				Output
			Debugging using Serial printf (Caveman Debugging)
			LCD
				Pin Configuration
				LCD Modes
				Implement Driver Functions
					Write Char
					Print String
					Cursor Display Mode
					Set Cursor Position
					Clear Screen
				Custom Character
			Keypad
				Keypad Matrix
				Scan Button Press
			ADC & DAC
				ADC
					ADC Terms
						Sampling 
						Resolution 
						Channels
					ADC Conversion Technique (Successive Approximation)
					Sensor Interfacing
						Temp Sensor (LM35)
						Light Sensor (LDR)
					Analog Comparator
				DAC
					Digital to Analog Conversion
					Implementing Code for (DAC0808)
			Timers & Counters
				Timer Functional Diagram
				Compare Match Mode
				Normal Timer Mode
				16-Bit Timer Vs. 8-Bit Timer
				Using Pre-Scalars for Generating Large Time Delays
				Timers to Counters 
			PWM Programming
				What's a PWM wave?
				PWM Applications 
				PWM Mode in Timers
				Controlling Servo Motor
			Input Capture and Wave Generation
				Wave Generation
					Generating Waves
						Square Waves
						Pulse Pattern
					Normal and CTC modes
				Input Capture Mode
					Measuring Frequency of Wave
					Measuring Pulse Width
			Interrupt
				Polling vs. Interrupts
				Interrupt Service Routine (ISR)
				Interrupt Vector Table
				External Interrupt
				Interrupt Priority 
				Nesting Interrupts
				Context Switching
				Interrupt Latency
			Serial Communication
				Serial vs. Parallel
				Terminologies 
					Data Transfer Rate (Baud Rate)
					Synch vs. ASynch
					Full-duplex vs. Half-duplex
				USART Module Driver Implementation
					Data Frame
					Sending Data
					Receiving Data
				SPI
					SPI Essentials
					SPI Modes
					SPI Master/Slave Communication
					Implementing SPI Code
						Master Code
						Slave Code
				I2C
					I2C Essentials
						I2C Operating Mode
						I2C Protocol
						I2C Addressing Modes
					I2C Master/Slave Communication
					I2C Implementing Code
						Slave Code
						Master Code
			Power Management Modes
				Why Power Management?
				AVR Sleep
				On-time Calculations for Battery-based Systems
			Debugging AVR
				Hardware Debugger
				AVR Simulator
				PROTEUS Simulator
		Part 2: Make Arduino-like Driver Abstractions
			Intro to Arduino Core Style
			digitalRead, digitalWrite
			analogRead, analogWrite
			Serial.begin, Serial.write, Serial.print, Serial.println, Serial.read, Serial.available
	Module 4: RTOS and Automotive Programming and Communication Standards
		Part 1: RTOS
			Part1 : RTOS concepts
				Introduction for RTOS
				RTOS vs. Normal OS
				RTOS basic Components and How it works
				Foreground / Background Program Execution
				Multitasking
				Task Management
					Task States
					Context Switching
				Scheduler
					Scheduler Types
						Preemptive
						Non preemptive
					Policies / Algorithm / Strategies 
						Priority Based
						Round Robin
						Least Execution Time 
				Re-entrant / Non Re-entrant Function
				Resource (Share Resource)
					Mutex
					Semaphores
						Binary Semaphore
						Counting Semaphore
						Issues
							Priority Inversion
							Dead block
			Part 2: RTOS Implementation Using FreeRTOS AVR
				FreeRTOS Intro
				Tasks
					Creating Tasks
					Deleting Tasks
				Using Queues
				Using Semaphores
				Using Interrupts
				Porting to AVR
		Part 2: Automotive
			1. Programming Standards
				A. MISRA C
				B. AutoSAR SW Architecture
			2. Communication Protocols
				CAN
				LIN
	Module 5: SW Engineering and Testing Practices
		Part 1: SW Engineering
			SW Engineering Concepts
			SW Development Life Cycle
				Waterfall Model
				V-Model
				Agile Model
				Other Models Concepts
			SW Requirements Management
				Requirements Activities
				Requirements Traceability 
			SW Configuration Management
				Config Management Concepts
				Version Control Systems (Git)
			SW Project Management Concepts
			UML Concepts
				Use Cases Diagram
				Class Diagram
				Activity/State Chart Diagram
				Other Diagrams Concepts
		Part 2: Cont'd Software Engineering : Software Testing
			SW Testing Fundementals
			7 Testing Principles
			Fundamental Testing Process
			Psychology of Testing
			Test Levels
				Unit Testing 
				Integration Testing
				System Testing
				Acceptance Testing
			Test Types
				Functional Testing
				Non-functional Testing
				Other Testing Types Concepts
					Structural Testing
					Change-based Testing
			Test Development Process
				Test Analysis
				Test Design
				Traceability
			Test Techniques
				Static Testing
				Dynamic Testing
					White Box 
						Statement Coverage
						Decision Coverage
					Black Box
						Equivalence Partitioning (EP)
						Boundary Value Analysis (BVA)
						Decision Tables
					How to Select Proper Testing Technique
			Test Organization
			Test Planning and Estimation
			Risk and Testing
			Overview of Common Used Testing Tools
