# Introductions

## What is Computer Science?

“the study of computers and algorithmic processes, including their principles, their hardware and software designs, their implementations, and their impact on society.”

Computational Thinking

- Decomposition: Break down the problem into smaller, more manageable parts.
- Pattern Recognition: Identify any patterns or similarities among the tasks or issues.
- Abstraction: Focus on the essential details while filtering out the irrelevant information
- Algorithmic Thinking: Develop a step by step plan to solve the problem or complete the task.

# Layers of Computing Systems

- Layer 1: Information
    - Machine language, Binary number system, data representation of text, image, audio, video, etc.
- Layer 2: Hardware
    - CPU, GPU, RAM, circuits, memories, logic gates, physical hardware.
- Layer 3: Programming
    - The instructions used to accomplish computations and manage data to solve problems
    - Algorithms: batching, looping, etc.
- Layer 4: Operating System
    - Managing the computer’s resources and provide a platform to interact for both user and application software.
- Layer 5: Applications
    - Programs to make use of the computer’s abilities to solve specific real-world problems.
- Layer 6: Communications
    - Communications with other computers to share information and resources.

![Screenshot 2024-09-05 at 10.05.07.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/a5654a72-d022-4c78-8443-9d85c39cf017/Screenshot_2024-09-05_at_10.05.07.png)

# Binary/Number Systems

Goal: Defining byte, binary, hexadecimal, etc. 

Computers are multimedia devices that deal with a vast variety of information categories. Computers store, present, and help us modify:

- Numbers
- Text
- Audio
- Images and graphics
- Video

## Denary/Decimal

- The number system we use in daily life
- Base 10 system, digits 0-9
- Numbers in the system are built using powers of 10, where the number 10 is raised to represents the location of the digit.

## Positional Notation

- A way to notate digit placement using powers of 10.
    
    ![Screenshot 2024-10-22 at 23.20.20.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/06da9651-fb09-44b7-8052-bab8f192ace1/Screenshot_2024-10-22_at_23.20.20.png)
    
- Here, the power 10 is raised to represents where the number will be placed, or what digit it will be. The nth digit will have 10 raised to the power to n-1.

## Binary

- 0 and 1 represented and processes data on two states (on/off)
- One digit is called one bit.
- Each bit stands for a power of 2.
- Lowest number on the right, highest number value on the left.
- Also known as base-2 system. (Due to the two different states on and off or true and false.)
- One byte contains 8 bits, when adding the total you should get a number that that byte is representing.

### Representing Negative Numbers

- Using the two’s complement.
- The logic behind is adding a certain number to -128.
- You change all the numbers to their opposite status. (All 0s to 1s, and 1s to 0s.)
- Add 1. (This is done because of how there is a 0)

## Hexadecimal

- Base-16 number system
- Uses 16 symbols to represent numbers.
    - 0-9 and A-F, with A representing 10 and F representing 15.
- Commonly used as it is a more compressed way of representing binary, especially large binary numbers.
- Each hexadecimal digit is composed of four binary digits.

## ASCII

- American Standard Code for Information Interchange
- Originally used 7 bits for 128 unique characters, but was then extended to 8 allowing for 255.
- ASCII is not suitable for international use, only for languages that use an alphabet
    - For instance Chinese or Japanese have thousands upon thousands of characters, which you cannot represent with only 255 unique characters.
- Uses something called a character encoding table or character set to map out keys.

## Unicode

- One Unicode set uses 16 bits per character, allowing for a wider variety of unique characters.
- UTF-8, UTF-16, UTF-32
    - UTF-8: Ranges from 1 - 4 bytes (8 - 32 bits)
    - UTF-16: Ranges from 2 - 4 bytes (16 - 32 bits)
    - UTF-32: Uses 4 bytes (32 bits)
        
        ![Screenshot 2024-10-23 at 09.33.13.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/3f36d71b-00f0-4484-9c51-979f62d7b4ab/Screenshot_2024-10-23_at_09.33.13.png)
        
- Uses something called a character encoding table or character set to map out keys.

## Encoding Video/RGB

- Color Depth
    - Named in the format RGBXXX
    - XXX is the number of bits allocated to each RGB value.
        - For instance RGB565 is a 16 bit color depth format in which R has 5 bits, G has 6 bits, B has 5 bits.
        - 16 bit RGB also has RGB555, where the extra one bit is allocated to alpha (opacity) or completely unused
    - RGB 24 bit is where RGB each have 8 bits, allowing for 16,777,216 different colors.
    

### Metadata

- At the very front of most media files, a few bytes will be used to represent the information of the file.
- For instance, file height and width, total file size, etc.

## Data Type

- Integers
    - Integers are mathematical numbers that are represented using a group of binary digits.
- Strings
    - A string is a sequence of characters. Encoded using a character encoding table. Uses something like ASCII or Unicode.

## Encoding Audio

- 

## Compression

- 

# Data Representation Poster

[Data Representation Whiteboard.pdf](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/1d070669-f4eb-4324-8332-7ebed92fde7e/Data_Representation_Whiteboard.pdf)

![Data Representation Whiteboard.jpg](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/0a4604a7-de1f-4304-a744-7efc09e5ba33/Data_Representation_Whiteboard.jpg)

## Logic Gates

### Boolean Algebra

- Consists of only two states: true and false
    - Makes for an ideal way to use in binary

### Gates

- Definition
    - A gate is a device that performs a basic operation on electric signals, accepting one or more input signals and producing a single output signal.

- NOT Gate
    - A NOT Gate accepts one input signal and returns the opposite signal as output

Truth Table

| A | X |
| --- | --- |
| 1 | 0 |
| 0 | 1 |

- AND Gate
    - An AND gate will output 1 if both inputs are 1, otherwise the output is 0.
    - X = A*B = AB = A.B = A^B = A OR B
    
    Truth Table
    
    | A | B | X |
    | --- | --- | --- |
    | 0 | 0 | 0 |
    | 0 | 1 | 0 |
    | 1 | 0 | 0 |
    | 1 | 1 | 1 |
- OR Gate
    - An OR gate accepts two input signals
    - The output is 1 when either input is 1. The output is 0 if both are 0.
    - X = A v B = A + B = A OR B
    
    Truth Table
    
    | A | B | X |
    | --- | --- | --- |
    | 0 | 0 | 0 |
    | 1 | 0 | 1 |
    | 0 | 1 | 1 |
    | 1 | 1 | 1 |
- XOR Gate (eXclusive OR)
    - The difference between XOR gate only differ in one input situation
    - When both input signals are 1 XOR outputs a 0

Truth Table

| A | B | X |
| --- | --- | --- |
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 0 |

- NAND Gate (NOT AND)
    - NAND gate accepts two input signals like the AND gate.
    - Essentially a NOT gate on an AND gate
    - If both inputs are 1 the output is 0, otherwise it stays a constant 1

Truth Table

| A | B | X |
| --- | --- | --- |
| 0 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

- NOR Gate (NOT OR)
    - NOR gate accepts multiple inputs, but usually no more than 3.
    - If both are 0 the output is 1; otherwise output is 0
    - Reversed OR gate

Truth Table

| A | B | X |
| --- | --- | --- |
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

Computation Order for Gates

NOT, AND, OR

## Transistors

- Transistors use semiconductors
    - Silicon treated with different elements such as boron or phosphorus
    - This creates an electron emitting N-TYPE and an electron absorbing P-TYPE
    - Arranged in three alternating layers. Each has a terminal attached.
        
        ![Screenshot 2024-10-24 at 20.21.47.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/138ca030-9e51-4022-b503-b1f974706137/Screenshot_2024-10-24_at_20.21.47.png)
        
    - The emitter, the base, the collector, respectively.
    - This is called an NPN transistor
    - Between the P and N, a special field called a P-N Junction is created, allowing electron flow only when voltage exceeds a certain threshold. Otherwise it is off.

## Computer Architecture

- Central Processing Unit

![Screenshot 2024-10-24 at 20.27.50.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0a1acae3-9490-44b3-9111-d203cb3c547b/b46c962e-37f9-4a32-a90e-a6dcba3801a2/Screenshot_2024-10-24_at_20.27.50.png)

- Arithmetic Logic Unit
    - Does all the logical processing and arithmetic processing. Referred to as a core.

- Control Unit
    - Decodes the instructions and controls other components of the CPU. (Directs data flow and the operation of the ALU).
    - Fetches each instruction from memory.
    - Decodes  into several commands/signals that are sent to other units for execution
    - Generates clock pulses that regulate the speed of the CPU and synchronizes it.

Registers - Small, fast, temporary storage units.

- Program Counter
    - holds the memory address of the next instruction (which program to execute next)
- MAR
    - Memory Address Register
    - Stores the address that is currently being read. (One way)
- MDR
    - Memory Data Register
    - Stores the data awaiting to be written into memory or to be processed.
- CIR
    - Current Instruction Register
    - Stores the instructions that has just been fetched from memory that is currently being decoded by the CU.

CPU Buses

- Address Bus
- Data Bus
- Diagram

## Fetch-Decode-Execute Cylce

1. Fetch
2. Decode
    1. Get data if needed
3. Execute
4. Store

- Fetch instruction from primary memory to control unit
    - MAR ⇒ RAM ⇒ send data via data bus to CU
- Decode instruction in control unit CU
    - CU decode the instruction and fetch additional data if needed
- Execute instruction
    - ALU Executes the instruction (additional data maybe fetched again according to the results)
- Store result of execution and check for next instruction
    - Store the result in the primary memory and then CPU checks for the next instruction

PC ⇒ MAR ⇒ RAM ⇒ MDR ⇒ CIR ⇒ CU ⇒ ALU ⇒ Accumulator
