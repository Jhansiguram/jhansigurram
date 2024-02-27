By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V


Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**

![1](https://github.com/Jhansiguram/jhansigurram/assets/160741021/e470d7f2-7926-46b4-ac13-c610f3787b8d)

**Step 2: Writing the C code in the leafpad editor using the following command
leafpad sum1ton.c&

![2](https://github.com/Jhansiguram/jhansigurram/assets/160741021/3216a725-7e1e-4461-b44a-643d8a7e86c6)

Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c

Step 5: Check the output by using the command

./a.out

The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c

**Step 2: Writing the C code in the leafpad editor using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![3](https://github.com/Jhansiguram/jhansigurram/assets/160741021/791a2874-817c-42c0-91f3-b7f5e5e97736)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command
ls -ltr sum1ton.c


![4](https://github.com/Jhansiguram/jhansigurram/assets/160741021/4806ef2c-9c99-4f26-9316-00da2b772aac)

Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution


![5](https://github.com/Jhansiguram/jhansigurram/assets/160741021/e70c2d74-2fe4-4cfd-b21d-871756012138)
![7](https://github.com/Jhansiguram/jhansigurram/assets/160741021/1204b45f-fcc1-42be-abe1-4835cfb02918)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![8](https://github.com/Jhansiguram/jhansigurram/assets/160741021/ceb6f1c9-db09-4dd6-9b4e-521389ce4eca)

![6](https://github.com/Jhansiguram/jhansigurram/assets/160741021/bf451803-7872-4504-8d1a-85fa7ce42734)
