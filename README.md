# Assembly-hello_world-
***

If you want to execute this program, you first need the Netwide Assembler, nasm, because this code uses its syntax. Then use the following commands (assuming the code is in the file helloworld.asm). They are needed for assembling, linking and executing, respectively.

```
~/ apt install nasm
  ...................
~/ nasm -felf64 helloworld.asm

        //-f: fromat, select an output format.
        //-e: preprocess only (writes output to stdout by default).
        //-l: listfile, write listing to a listfile.
        //-f64: fromat 64.
        
~/ ld helloworld.o -o helloworld

      //ld: to linker format
      
~/ ./helloworld
