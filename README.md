# coe328-lab-2-solved
**TO GET THIS SOLUTION VISIT:** [COE328 Lab 2 Solved](https://mantutor.com/product/coe328-solved-2/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112719&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COE328 Lab 2  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
Objective:

This objective of this laboratory experiment is to design and construct an Arithmetic and Logic Unit (ALU) in VHDL environment and implement it on an FPGA board.

• Design and build all functions of the ALU.

• Design, simulate the ALU using VHDL (Based on Functional Simulation in Quartus Simulator).

Procedure:

This unit consists of different parts that would come together to create a functional ALU. A processing unit is usually divided to 4 distinct components. The control unit performs the fetching of instructions and signals. The bus controls access to data values throughout the processing unit – these registers act as temporary storage units. The ALU Core performs the arithmetic and logical operations on desired inputs and produces the required outputs. This project focuses on all four components of a typical ALU.

Part I: Procuring input data

The ALU is to perform a set of arithmetical and logical functions on two 8-bit inputs A and B. These inputs are first utilized in simulation phase through waveform editor on Quartus II, Inputs A and B are procured using the last four digits of your student ID. For instance, if the student ID is 500864395, then translating

to

Figure 1. The Block Diagram of the GPU

Part II: Storage Unit (Register)

The storage units which are sometimes called Registers are utilized to temporary store the input values and then pass them to the following components in the system. As portrayed in Figure 1, two 8-bit register units are utilized in the ALU to store inputs A and B. The register reads the bit values on its input on the rising edge of the clock signal and passes those bit values to the output port on the next rising edge of the clock signal.

Write the VHDL code using Figure 2 for a register unit and confirm its functionality with the help of a truth table. Thereafter, create a symbol of your design to be utilized in the final circuit design. Next, import the symbol to the GPU project. Import the same symbol twice as the system needs one register unit for each respective 8-bit input.

Figure 2. Code template for implementing Register Storage Unit.

Part III: Control Unit

The Control unit decides the microcode that is to be delivered to the ALU core and will act as the operations-selector for the ALU core. The Control Unit produces an output OP, which is passed to ALU core as the operations selector. This component consists of two sub-components – the FSM and a 4 to 16 decoder.

Part III (a): Finite State Machine (FSM)

In the initial design of the Control unit, the current state of the FSM is to be passed to the decoder unit. In other words, the FSM sub-component in the initial Control unit design will only act as an up-counter, cycling through states 0 to 8 consecutively (modification required for consecutive state transition) and back to state 0 while the student_id will be displayed on a 7segment. The FSM takes the clock signal as the input, and produces the 4-bit output current_state and passes it to the decoder sub-component. Upon completing the FSM design, create a symbol representing the FSM sub-component which is to be used in the final design.

Part III (b): 4 to 16 Decoder (4×16 Dec)

The decoder is tasked with receiving the signal current_state from FSM and decoding it to the operation-selector microcode. In the initial design of the Control unit, the Decoder unit passes the signal OP to the ALU core, which will then translate to operations selector for the ALU core and follow the functions enlisted in Table 1.

A 3×8 decoder design has been designed and utilized in the previous labs. You can import the same design and extend it to the 4×16 decoder following the schematics portrayed in Figure 2. When the decoder design is completed, create a symbol of the sub-component to be utilized in the final circuit design.

Figure 3. Implementation of 4×16 Decoder using 3×8 decoders

Part IV: Description of the ALU core

The heart of every GPU unit is the ALU core where all arithmetic and logical operations are to be implemented and applied as required. In this part students are required to implement all functionalities and operations using VHDL syntax compatible with Altera FPGA boards. The ALU core will take two 8-bit inputs (A and B) and a 16-bit input from Control unit. The microcode input from controller unit is the operation-selector signal, deciding the operation that is to be applied on the inputs A and B. Although the microcode received from the Control unit is 16 bits, only 9 distinct operations are to be implemented. The functionalities of the ALU core and their corresponding microcode are listed in Table 1. The microcode is delivered from the Control unit and will decide what operation the inputs would undergo.

Operations listed in Table 1 are to be implemented in the ALU core by writing the proper VHDL code for the ALU core. The 8-bit output (Result) of the ALU Core is to be displayed on two 7segment display or LEDs. When the ALU Core design is completed, create a symbol to represent this component in the final design.

Table 1. ALU Core Operations for Problem 1

Figure 4. Code Template for ALU Core.

Part V: Displaying the Output

The ALU core produces an 8-bit output called Result, which is the result of the operations applied on A and B.

In the simulation phase of the design, the output Result is to be displayed in bit-value format in the waveform editor window. In implementation phase where the design is programed on the

FPGA board, this output is to be displayed on two 7-segment displays in hexadecimal format.

For example, if then the 7-segment combined unit displays as illustrated in

Figure 4.

Figure 5. Typical 8-bit Seven Segment Display

Part VI: Final Design

As the designs for different components (Register, ALU Core, FSM and Decoder units) are completed, they should all be ported to one final circuit design.

1. Open a new schematic design and import all the required units. When importing is completed, you should have the following components: two Registers (one per input), one ALU Core, one FSM, Decoder, three 7-segment displays (one for student_id and two for the output Result from the ALU).

2. Create the 8-bit input ports A and B, 8-bit output port Result and the single-bit input Clock port.

3. Connect all the components using single and multi-bit data buses. Follow the schematics portrayed in Appendix A. Figure 6.

4. Name the data buses to represent the proper signals, for e.g. OP and A.

Part VIII: Problem Sets

Problem 1: Initial Design

Implement the initial design of the General Processor Unit (GPU). In this design, the FSM output current_state follows an up-counting pattern, which will then dictate the operation selector signal to the ALU core. Thus, the output of the ALU core, Result, will represent the outputs of operations shown in Table 1 and following the same order.

Problem 2: Modified ALU Core

Function # Operation / Function

1 Increment A by 2

2 Shift B to right by two bits, input bit = 0 (SHR)

3 Shift A to right by four bits, input bit = 1 (SHR)

4 Find the smaller value of A and B and produce the results ( Min(A,B) )

5 Rotate A to right by two bits (ROR)

6 Invert the bit-significance order of B

7 Produce the result of XORing A and B

8 Produce the summation of A and B, then decrease it by 4

9 Produce all high bits on the output

b)

Function # Operation / Function

1 Swap the lower and upper 4 bits of A

2 Produce the result of ORing A and B

3 Decrement B by 5

4 Invert all bits of A

5 Invert the bit-significance order of A

6 Find the greater value of A and B and produce the results ( Max(A,B) )

7 Produce the difference between A and B

8 Produce the result of XNORing A and B

9 Rotate B to left by three bits (ROL)

c)

Function # Operation / Function

1 Produce the difference between A and B

2 Produce the 2’s complement of B

3 Swap the lower 4 bits of A with lower 4 bits of B

4 Produce null on the output

5 Decrement B by 5

6 Invert the bit-significance order of A

7 Shift B to left by three bits, input bit = 1 (SHL)

8 Increment A by 3

9 Invert all bits of B

d)

Function # Operation / Function

1 Shift A to right by two bits, input bit = 1 (SHR)

2 Produce the difference of A and B and then increment by 4

3 Find the greater value of A and B and produce the results ( Max(A,B) )

4 Swap the upper 4 bits of A by the lower 4 bits of B

5 Increment A by 1

6 Produce the result of ANDing A and B

7 Invert the upper four bits of A

8 Rotate B to left by 3 bits (ROL)

9 Show null on the output

e)

Function # Operation / Function

1 Replace the odd bits of A with odd bits of B

2 Produce the result of NANDing A and B

3 Calculate the summation of A and B and decrease it by 5

4 Produce the 2’s complement of B

5 Invert the even bits of B

6 Shift A to left by 2 bits, input bit = 1 (SHL)

7 Produce null on the output

8 Produce 2’s complement of A

9 Rotate B to right by 2 bits (ROR)

f)

Function # Operation / Function

1 Decrement B by 9

2 Swap the lower and upper 4 bits of B

3 Shift A to left by 2 bits, input bit = 0 (SHL)

4 Produce the result of NANDing A and B

5 Find the greater value of A and B and produce the results ( Max(A,B) )

6 Invert the even bits of B

7 Produce null on the output

8 Replace the upper four bits of B by upper four bits of A

9 Show A on the output

g)

Function # Operation / Function

1 Invert the bit-significance order of A

2 Shift A to left by 4 bits, input bit = 1 (SHL)

3 Invert upper four bits of B

4 Find the smaller value of A and B and produce the results ( Min(A,B) )

5 Calculate the summation of A and B and increase it by 4

6 Increment A by 3

7 Replace the even bits of A with even bits of B

8 Produce the result of XNORing A and B

9 Rotate B to right by 3 bits (ROR)

h)

Function # Operation / Function

1 Rotate A to right by 4 bits (ROR)

2 Produce the result of XORing A and B

3 Invert the bit-significance order of B

4 Calculate the summation of A and B and decrease it by 2

5 Rotate B to left by 2 bits (ROL)

6 Invert the even bits of B

7 Swap the lower 4 bits of B with lower 4 bits of A

8 Shift B to right by 2 bits, input bit = 0 (SHR)

9 Invert lower four bits of A

Problem 3: Modified Control Unit (FSM)

a) For each microcode instruction, display ‘y’ if the FSM output (student_id) is odd and ‘n’ otherwise

b) For each microcode instruction, display ‘y’ if the FSM output (student_id) is even and ‘n’ otherwise

c) For each microcode instruction, display ‘y’ if the FSM output (student_id) had an odd parity and ‘n’ otherwise

d) For each microcode instruction, display ‘y’ if the FSM output (student_id) had an even parity and ‘n’ otherwise

e) For each microcode instruction, display ‘y’ if one of the 2 digits of A are greater than FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

f) For each microcode instruction, ‘y’ if one of the 2 digits of A are less than FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

g) For each microcode instruction, ‘y’ if one of the 2 digits of A are equal to FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

h) For each microcode instruction, display ‘y’ if one of the 2 digits of B are greater than FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

i) For each microcode instruction, ‘y’ if one of the 2 digits of B are less than FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

j) For each microcode instruction, ‘y’ if one of the 2 digits of B are equal to FSM output (student_id) and ‘n’ otherwise. Use the microcode instruction from part 1 of the lab.

Appendix A

Figure 6. Typical Block Schematic for Problem 1

Figure 7. Typical Block Schematic for Problem 3
