addi $1,$0,0
addi $2,$0,0

LOOP:
add $2,$2,$1
addi $1,$1,1
slti $11,$1,10
bne $11,$0,LOOP
nop
beq $11,$0,EXIT
nop

EXIT:
