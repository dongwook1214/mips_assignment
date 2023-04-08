addi $1,$0,0

addi $2,$0,0

LOOP: slti $11,$1,10

beq $11,$0,EXIT

nop

add $2,$2,$1

addi $1,$1,1

j LOOP

nop

EXIT:
