```asm
str fp, [sp, #-4]!
add fp, sp, #0
str r1, [fp, #-0x14]
str r2, [fp, #-0x18]
str r3, [fp, #-0x14]
b #0x450
bne #0x3c
ldr r3, [fp, #-0x10]
ldr r3, [fp, #-0x14]
cmp r3, #2
bic r3, r3, #0x80000000
bic r3, r3, #0x80
and r3, r3, r2
cmp r3, #0
add r3, r3, #1
str r3, [fp, #-0x14]
beq #0x54
ldr r3, [fp, #-0x14]
b #0x2b8
ldr r3, [fp, #-0x14]
ldr r3, [fp, #-0x14]
cmp r3, #6
ldr r3, [pc, #0x244]
and r3, r3, r2
bne #0x84
ldr r3, [fp, #-0x10]
beq #0x7c
ldr r3, [fp, #-0x14]
mov r3, #0
str r3, [fp, #-0x14]
cmp r3, #9
bne #0xa0
sub sp, sp, #0x1c
str r0, [fp, #-0x10]
ldr r3, [fp, #-0x14]
cmp r3, #0
ldr r3, [fp, #-0x14]
cmp r3, #0
bic r3, r3, #0x40000000
bic r3, r3, #0x40
bne #0xc4
ldr r3, [fp, #-0x10]
cmp r3, #0
beq #0xbc
beq #0xc4
ldr r3, [fp, #-0x14]
b #0x3e0
ldr r3, [fp, #-0x14]
add r3, r3, #1
str r3, [fp, #-0x14]
cmp r3, #5
bne #0xf0
bne #0xf8
ldr r2, [fp, #-0x10]
cmp r3, #0
beq #0xf0
and r3, r3, #2
cmp r3, #0
add r3, r3, #1
str r3, [fp, #-0x14]
b #0x228
ldr r3, [fp, #-0x14]
ldr r3, [fp, #-0x10]
and r3, r3, #1
bne #0x128
ldr r2, [fp, #-0x10]
cmp r3, #0
beq #0x120
cmp r3, #0
beq #0x124
b #0x528
ldr r3, [fp, #-0x14]
mov r3, #0
str r3, [fp, #-0x14]
cmp r3, #3
bne #0x154
cmp r3, #3
bne #0x158
bic r3, r3, #0x80
cmp r3, #0
ldr r3, [fp, #-0x10]
bic r3, r3, #0x10000000
beq #0x158
mov r3, #0
ldr r3, [fp, #-0x14]
add r3, r3, #1
ldr r3, [fp, #-0x14]
cmp r3, #6
b #0x2c0
ldr r3, [fp, #-0x14]
ldr r3, [fp, #-0x10]
bic r3, r3, #2
cmp r3, #0
beq #0x188
str r3, [fp, #-0x14]
b #0x288
ldr r3, [pc, #0x464]
and r3, r3, r2
ldr r3, [fp, #-0x14]
add r3, r3, #1
mov r3, #0
str r3, [fp, #-0x14]
cmp r3, #1
bne #0x1c4
b #0x4f8
ldr r3, [fp, #-0x14]
ldr r2, [fp, #-0x10]
ldr r3, [pc, #0x354]
ldr r3, [fp, #-0x10]
bic r3, r3, #0x80000000
beq #0x1c8
mov r3, #0
bic r3, r3, #0x10
cmp r3, #0
str r3, [fp, #-0x14]
b #0x410
str r3, [fp, #-0x14]
b #0x3e8
bne #0x1fc
ldr r3, [fp, #-0x10]
cmp r3, #8
bne #0x204
cmp r3, #0
beq #0x1fc
ldr r3, [fp, #-0x14]
add r3, r3, #1
ldr r3, [fp, #-0x14]
cmp r3, #9
ldr r2, [fp, #-0x10]
ldr r3, [pc, #0x408]
beq #0x21c
ldr r3, [fp, #-0x14]
beq #0x220
mov r3, #0
ldr r3, [fp, #-0x14]
cmp r3, #2
str r3, [fp, #-0x14]
b #0x520
bne #0x250
ldr r2, [fp, #-0x10]
bne #0x254
ldr r3, [fp, #-0x10]
cmp r3, #0
beq #0x24c
bic r3, r3, #0x20000000
bic r3, r3, #0x20
mov r3, #0
str r3, [fp, #-0x14]
add r3, r3, #1
str r3, [fp, #-0x14]
cmp r3, #7
bne #0x280
bne #0x27c
ldr r3, [fp, #-0x10]
mov r3, #0
str r3, [fp, #-0x14]
ldr r3, [fp, #-0x18]
ldr r2, [pc, #0xd8]
add r3, r3, #4
ldr r2, [pc, #0xcc]
and r3, r3, r2
cmp r3, #0
add r3, r3, #1
str r3, [fp, #-0x14]
str r3, [fp, #-0x14]
b #0x648
bne #0x2c0
ldr r2, [fp, #-0x10]
ldr r3, [fp, #-0x14]
cmp r3, #4
ldr r3, [pc, #0x2fc]
and r3, r3, r2
bic r3, r3, #0x20000000
bic r3, r3, #0x20
mov r3, #0
str r3, [fp, #-0x14]
cmp r3, #0
beq #0x2d4
b #0x4b0
ldr r3, [fp, #-0x14]
b #0x488
ldr r3, [fp, #-0x14]
ldr r3, [fp, #-0x10]
bic r3, r3, #0x10000000
cmp r3, #1
bls #0x2f4
b #0x3d0
ldr r3, [fp, #-0x14]
str r2, [r3]
ldr r3, [fp, #-0x18]
str r2, [r3]
ldr r3, [fp, #-0x18]
b #0x6e0
ldr r3, [fp, #-0x14]
ldr r3, [fp, #-0x10]
bic r3, r3, #0x40000000
ldr r3, [pc, #0x3b0]
and r3, r3, r2
ldr r3, [fp, #-0x14]
add r3, r3, #1
cmp r3, #0
beq #0x338
str r3, [fp, #-0x14]
b #0x5f8
b #0x5d0
ldr r3, [fp, #-0x14]
ldr r2, [fp, #-0x10]
ldr r3, [pc, #0x2a4]
cmp r3, #7
bne #0x36c
and r3, r3, r2
cmp r3, #0
bic r3, r3, #0x10
cmp r3, #0
str r3, [fp, #-0x14]
b #0x4e8
cmp r3, #0xa
bne #0x440
cmp r3, #0
beq #0x438
add r3, r3, #8
ldr r2, [pc, #0xc0]
add r3, r3, #0xc
ldr r2, [pc, #0xb4]
cmp r3, #1
bne #0x3a8
bic r3, r3, #0x40
cmp r3, #0
cmp r3, #0
beq #0x3a8
str r3, [fp, #-0x14]
b #0x720
ldr r3, [fp, #-0x14]
add r3, r3, #1
ldr r3, [fp, #-0x14]
cmp r3, #4
cmp r3, #5
bne #0x3dc
and r3, r3, r2
cmp r3, #0
ldr r2, [fp, #-0x10]
ldr r3, [pc, #0x1ec]
beq #0x3dc
ldr r3, [fp, #-0x14]
beq #0x3e0
mov r3, #0
ldr r3, [fp, #-0x14]
cmp r3, #8
ldr r3, [fp, #-0x10]
and r3, r3, #8
mov r3, #0
str r3, [fp, #-0x14]
str r2, [r3]
ldr r3, [fp, #-0x18]
str r2, [r3]
ldr r3, [fp, #-0x18]
add r3, r3, #0x10
ldr r2, [pc, #0xa8]
add r3, r3, #0x14
ldr r2, [pc, #0x9c]
ldr r2, [fp, #-0x18]
add r3, r2, r3
lsl r3, r3, #2
ldr r2, [fp, #-0x18]
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
str r2, [r3]
ldr r3, [fp, #-0x18]
str r2, [r3]
ldr r3, [fp, #-0x18]
ldr r1, [r3]
ldr r3, [fp, #-8]
add r2, r2, r3
ldr r3, [pc, #0x5c]
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
add r3, r3, #0x18
ldr r2, [pc, #0x90]
str r3, [fp, #-8]
b #0x54c
eor r3, r3, r1
str r3, [r2]
str r3, [fp, #-8]
ldr r3, [fp, #-8]
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
str r2, [r3]
mov r3, #0
ldr r3, [fp, #-8]
lsl r3, r3, #2
ldr r3, [fp, #-8]
add r3, r3, #1
cmp r3, #6
ble #0x558
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
ldr r3, [fp, #-0x14]
mov r0, r3
bx lr
andmi r0, r0, r0, asr #32
svcpl #0x3759df
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
add sp, fp, #0
pop {fp}
andhi r0, r0, r0, lsl #1
andhs r0, r0, r0, lsr #32
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andne r0, r0, r0, lsl r0
ldrblo r3, [r4], #-0x8b7
ldmdalo sb, {r0, r1, r4, r5, r7, fp, sp, lr} ^
subeq r6, r4, r0, lsl #17
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
mcrreq p1, #0xb, r2, ip, c6
strbhs r3, [sp, #-0xa8]!
mrcvc p12, #2, r0, c9, c9, #5
svcpl #0x3753a2
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
andeq r0, r0, r0
```