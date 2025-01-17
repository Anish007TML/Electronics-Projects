https://circuitverse.org/users/284085/projects/4-bit-alu-530e4eea-ada6-4a1c-a912-c3ef70a11d13
This module implements a 4 bit ALU that performs multiple tasks like addition, subtraction and logical operations like AND,OR and XOR of two 4 bit numbers.
It is implemented with the help of sub-circuits. 
Firstly, full adder is designed and then we used it as a sub circuit in 4-bit full adder cum subtractor with a mode input.When mode=0 then it acts as a full adder. When mode=1 then it acts as a full subtractor.
Then, that circuit is converted to a sub circuit and implemented in a single IC with 4+4+1 inputs and 4+1 outputs.
Then Multiplexer is used to perform different tasks as when required. Then we implemented a 1-bit ALU which takes S1S0 as select lines and when S1S0=00 then AND operation is performed.
When S1S0=01 then OR operation is performed  and when S1S0=10 then XOR operation is performed and when S1S0=11 then Adder cum subtractor can be implemented.
Then this 1-bit ALU is used as a sub circuit and implemented in the 4 bit ALU and hence it takes 4+4+1(MODE) as imputs and S1S0 as select lines and gives Y3Y2Y1Y0 as output and a carry output if adder-cum-subtracter is used.
