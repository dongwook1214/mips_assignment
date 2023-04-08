addi $1,$0,10

LOOP: slti $11,$1,0

bne $11,$0,EXIT

nop

addi $1,$1,-1

j LOOP

nop

EXIT:
