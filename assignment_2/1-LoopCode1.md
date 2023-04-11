addi $1,$0,10

LOOP: slti $11,$1,0

bne $11,$0,EXIT

nop

addi $1,$1,-1

j LOOP

nop

EXIT:

1번 수정:
L:
slti $2, $1, 0
beq $2, $0, EXIT
nop
addi $1, $1, -1

j L 
nop

EXIT:

