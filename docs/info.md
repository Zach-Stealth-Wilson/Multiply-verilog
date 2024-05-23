<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works |

This is a CSAM (carry save array multiplyer) that takes two 4 bit inputs (Y, X) and outputs (Z2) the resulting 8 bit multiplication of the inputs.

Z2 = Y * X

## How to test |
Choose values for inputs Y(ui_in) X(uio_in) and expected output Z2(uo_out) that correspond to      the python testbench "test.py"

    11 in binary (4-bit) is 1011
    13 in binary (4-bit) is 1101
    (11 * 13) gives an 8-bit binary representation equal to 10011111, which is 143 in decimal

AS SEEN IN "test.py"

 # Set the input values you want to test
    dut.ui_in.value = 11
    dut.uio_in.value = 13
    
    # The following assersion is just an example of how to check the output values.
    # Change it to match the actual expected output of your module:
    assert dut.uo_out.value == 143
    

## External hardware |

NONE
