# rithika-sahyadri-ece
Repository for Samsung RISC-V Talent Development Program

The program harnesses the RISC-V architecture and employs open-source tools to instruct individuals on the design of VLSI chips and the fundamentals of RISC-V

BASIC DETAILS:

Name: rithika

College: Sahyadri college of Engineering and management,Adyar,Mangalore-575007

College mail: rithika.ec23@sahyadri.edu.in

Email ID: rithikakunder@gmail.com

GitHub profile:https:https://github.com/rithika

Linkedin profile:https://www.linkedin.com/in/rithika-kunder-8943b2293?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app

Task1

![image](https://github.com/user-attachments/assets/5b13e0eb-85b4-4341-8797-87ebd4ffe288)

![image](https://github.com/user-attachments/assets/4c5698e9-0e20-47a6-8ac5-023bccc62611)

![image](https://github.com/user-attachments/assets/3de616ed-35e0-4b6a-8ebc-fdf6430e0feb)

Task2

![image](https://github.com/user-attachments/assets/737f1630-3c16-4f86-a807-b1f63a863774)

![image](https://github.com/user-attachments/assets/61ee8c44-2505-4bd1-8a01-cc6b751708b5)

Task3

Task 3.1

![image](https://github.com/user-attachments/assets/e25186c3-9135-4a52-8ff1-0717020ce3ef)

Task 3.2

![image](https://github.com/user-attachments/assets/7fb949cb-737c-4e71-81b4-eae3c93aa024)

RISC-V Instruction Types and Fields

RISC-V instructions are categorized into different types based on how their fields are structured. These fields include:

Opcode (7 bits): Identifies the type of instruction.

funct3 (3 bits): Specifies the operation within the instruction type.

funct7 (7 bits, only for R-type): Further refines the operation.

Register Fields (rd, rs1, rs2): Specify the registers involved.

Immediate (various sizes): Represents constants used in operations.

Each instruction type is designed for specific operations.

R-type (Register Type) Used for: Arithmetic and logical operations involving registers. Fields: Field Bits Description funct7 7 Defines the operation (e.g., addition vs. subtraction). rs2 5 Second source register. rs1 5 First source register. funct3 3 Additional operation information. rd 5 Destination register. opcode 7 Instruction category. Example: add a0, a1, a2 Adds a1 and a2, storing the result in a0. Binary Encoding: funct7 | rs2 | rs1 | funct3 | rd | opcode
0000000 | 00110 | 00101 | 000 | 00100 | 0110011

I-type (Immediate Type) Used for: Immediate operations, loads, and jumps. Fields: Field Bits Description imm[11:0] 12 Signed immediate value. rs1 5 Source register. funct3 3 Operation type. rd 5 Destination register. opcode 7 Instruction category. Example: addi a0, a1, 10 Adds 10 to a1, storing the result in a0. Binary Encoding: imm[11:0] | rs1 | funct3 | rd | opcode
000000001010 | 00001 | 000 | 00010 | 0010011

S-type (Store Type) Used for: Storing values into memory. Fields: Field Bits Description imm[11:5] 7 Upper part of immediate value. rs2 5 Data register. rs1 5 Base address register. funct3 3 Operation type. imm[4:0] 5 Lower part of immediate value. opcode 7 Instruction category. Example: sw a0, 16(sp) Stores a0 at memory address sp + 16. Binary Encoding: imm[11:5] | rs2 | rs1 | funct3 | imm[4:0] | opcode
0000010 | 00010 | 00010 | 010 | 00000 | 0100011

B-type (Branch Type) Used for: Conditional branching (e.g., beq, bne). Fields: Field Bits Description imm[12 10:5] 7 rs2 5 Second register for comparison. rs1 5 First register for comparison. funct3 3 Defines branch type (e.g., equal, not equal). imm[4:1 11] 5 opcode 7 Instruction category. Example: beq a0, a1, 16 If a0 == a1, jump to PC + 16. Binary Encoding: imm[12|10:5] | rs2 | rs1 | funct3 | imm[4:1|11] | opcode
000000 | 00001 | 00000 | 000 | 00000 | 1100011

U-type (Upper Immediate Type) Used for: Loading large immediate values (lui, auipc). Fields: Field Bits Description imm[31:12] 20 Immediate value (upper bits). rd 5 Destination register. opcode 7 Instruction category. Example: lui a0, 0x12345 Loads 0x12345000 into a0. Binary Encoding: imm[31:12] | rd | opcode
00010010001101000101 | 00010 | 0110111

J-type (Jump Type) Used for: Jumping to an address (jal). Fields: Field Bits Description imm[20 10:1 11 rd 5 Destination register (stores return address). opcode 7 Instruction category. Example: jal ra, 1024 Jumps to address PC + 1024 and stores return address in ra. Binary Encoding: imm[20|10:1|11|19:12] | rd | opcode
000000100000 | 00001 | 1101111
Summary of Instruction Types Type Purpose Example R-type Register operations add a0, a1, a2 I-type Immediate operations, loads addi a0, a1, 10 S-type Store operations sw a0, 16(sp) B-type Conditional branching beq a0, a1, 16 U-type Large immediate values lui a0, 0x12345 J-type Unconditional jumps jal ra, 1024 Each type is designed for a specific set of operations, making RISC-V simple yet powerful.

Task 4

Task 4.1

![image](https://github.com/user-attachments/assets/b428b8ed-74cb-49b0-8fb4-b1e0ebc2170c)

Task 4.2

![image](https://github.com/user-attachments/assets/71a11bd7-4500-46d3-89b5-81f4a59384d4)

Task 4.3

![image](https://github.com/user-attachments/assets/051de975-790b-45bb-b80f-12493a1f6eb5)

Task 4.4

![image](https://github.com/user-attachments/assets/e9f7a7a2-8e84-4e9d-bcc4-490e0c9b66f4)

Task 4.5

![image](https://github.com/user-attachments/assets/65236ad1-9aa2-4355-996c-42d46b55e259)
