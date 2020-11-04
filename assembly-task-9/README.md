# DD1337 Week 9

This week is the **last week** of this course! Therefore, make sure to go back and correct **all** of your komplettering to get a tip top grade! 

## Assembly Language Design

Time to face it, MIPS, especially MARS, is for plebs (cool plebs)! You, yes YOU, can surely do a better job than that! For this reason, show your programming alphaness by designing your own assembly language. 

Your language must be an 8-bit assembly language, meaning that your assembly instructions has to be 8-bits long. See the [MIPS reference sheet](https://www.kth.se/social/files/563c63c9f276547044e8695f/mips-ref-sheet.pdf) and take inspiration from the MIPS 32-bit instruction encoding. Your instruction encoding determins:

| **Code** | **Size and Flexibility** |
|----------|--------------------------|
| `op` _(operation)_ | 2-3 bits operation code gives room for 4-8 instructions. |
| `rs`/`rt`/`rd` _(registry)_ | 2 bits registry addresses gives room for 4 registries. |
| `imm` _(immidiate)_ | 4-5 bits immidiate values gives room for 16-32 value unsigned constants or 8-16 value signed constants. |
| `label` _(jump address)_ | 4-6 bits jump address gives room for jumps (branching) of max 16-64 instructions per jump. Remember that jump chaining is tedious. |

Think carefully of how your instructions are encoded. More registries may mean a smaller instruction set or shorter constants.

Lastly, remember to give your language a killer name!!!

## Assignment

Summary:
- Fulfill one of the assignment levels below.
- Write a faculty calculator as described below.

### Prepare Assignment

1) Create a repository named `<KTH_ID>-assembly` under the `INDAPlus20` organisation and clone it.
2) Navigate into your newly created repository and start writing.

See `./bbvv` for an example language.

### Assignment Levels

Higher lever equals more alpha!

1) Copy the design of _Bacon Borde Vara Vegetariskt_ and implement an interpreter for the language in C, C++, Rust or another low level language.
2) Design your own language and implement an interpreter for your language in whatever programming language you want (excluding Python).
3) Design your own language and write an compiler as well as an emulator (we don't have time to design and order custom chips) for your language/architecture in whatever programming language you want (excluding Python).

For advanced implementations (only level 3), contenders for the most outrageous implementation, you are allowed to team up in pairs!

An interpretor reads a code file and run it instruction for instruction. A compiler reads a code file and outputs a system specific executable file. An emulator reads an executable file and executes it by interpretation.

**@Rustacians** Bonus points for whoever implements their solution using Rust! Tagga Rust!

**@Haskellers** Automatic A grade for whoever implements their solution using Haskell. Also, you are a madman if so!

**@Everyone** The most outrageous solution will get recognition from the fabled Ric himself! Be creative!

### Language Capabilities

Your language has to have the instructions for you to write a program that takes an integer `n` as user input, then calculates and outputs the value `n!`.

To prove your language's capabilities, write this program and include the file in your repository ready to be interpreted or compiled.