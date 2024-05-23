<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works |

This is a CSAM (carry save array multiplyer) that takes two 4 bit inputs and outputs the resulting 8 bit multiplication of the inputs.

## How to test |
Choose values for inputs X(ui_in) Y(uio_in) and expected output Z2(uo_out) that correspond to      the python testbench "test.py"

    20 in binary (8-bit) is 00010100
    30 in binary (8-bit) is 00011110
    (20 & 30) in 8-bit binary equals 00010100, which is 20 in decimal

AS SEEN IN "test.py"

 # Set the input values you want to test
    dut.ui_in.value = 20
    dut.uio_in.value = 30
    
    # The following assersion is just an example of how to check the output values.
    # Change it to match the actual expected output of your module:
    assert dut.uo_out.value == 20
    

## External hardware |

NONE
