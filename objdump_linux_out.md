# $ objdump --dwarf a.out # produced on Linux
```

a.out:     file format elf64-littleaarch64

Contents of the .eh_frame section:


00000000 0000000000000010 00000000 CIE
  Version:               1
  Augmentation:          "zR"
  Code alignment factor: 4
  Data alignment factor: -8
  Return address column: 30
  Augmentation data:     1b
  DW_CFA_def_cfa: r31 (sp) ofs 0

00000014 0000000000000010 00000018 FDE cie=00000000 pc=0000000000000600..0000000000000634
  DW_CFA_advance_loc: 4 to 0000000000000604
  DW_CFA_undefined: r30 (x30)

00000028 0000000000000010 0000002c FDE cie=00000000 pc=0000000000000650..0000000000000680
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

0000003c 0000000000000010 00000040 FDE cie=00000000 pc=0000000000000680..00000000000006bc
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

00000050 0000000000000020 00000054 FDE cie=00000000 pc=00000000000006c0..0000000000000708
  DW_CFA_advance_loc: 4 to 00000000000006c4
  DW_CFA_def_cfa_offset: 32
  DW_CFA_offset: r29 (x29) at cfa-32
  DW_CFA_offset: r30 (x30) at cfa-24
  DW_CFA_advance_loc: 8 to 00000000000006cc
  DW_CFA_offset: r19 (x19) at cfa-16
  DW_CFA_advance_loc: 56 to 0000000000000704
  DW_CFA_restore: r30 (x30)
  DW_CFA_restore: r29 (x29)
  DW_CFA_restore: r19 (x19)
  DW_CFA_def_cfa_offset: 0
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

00000074 0000000000000010 00000078 FDE cie=00000000 pc=0000000000000710..0000000000000714
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

00000088 0000000000000010 00000000 CIE
  Version:               1
  Augmentation:          "zR"
  Code alignment factor: 1
  Data alignment factor: -4
  Return address column: 30
  Augmentation data:     1b
  DW_CFA_def_cfa: r31 (sp) ofs 0

0000009c 0000000000000010 00000018 FDE cie=00000088 pc=0000000000000714..0000000000000718
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

000000b0 0000000000000024 0000002c FDE cie=00000088 pc=0000000000000718..000000000000074c
  DW_CFA_advance_loc: 4 to 000000000000071c
  DW_CFA_def_cfa_offset: 48
  DW_CFA_advance_loc: 8 to 0000000000000724
  DW_CFA_def_cfa: r29 (x29) ofs 16
  DW_CFA_offset: r30 (x30) at cfa-8
  DW_CFA_offset: r29 (x29) at cfa-16
  DW_CFA_advance_loc: 28 to 0000000000000740
  DW_CFA_def_cfa: r31 (sp) ofs 48
  DW_CFA_advance_loc: 8 to 0000000000000748
  DW_CFA_def_cfa_offset: 0
  DW_CFA_restore: r30 (x30)
  DW_CFA_restore: r29 (x29)
  DW_CFA_nop
  DW_CFA_nop
  DW_CFA_nop

000000d8 0000000000000014 00000054 FDE cie=00000088 pc=000000000000074c..000000000000075c
  DW_CFA_advance_loc: 4 to 0000000000000750
  DW_CFA_def_cfa_offset: 16
  DW_CFA_offset: r30 (x30) at cfa-16
  DW_CFA_nop
  DW_CFA_nop

000000f0 ZERO terminator


Contents of the .debug_info section:

  Compilation Unit @ offset 0x0:
   Length:        0x68 (32-bit)
   Version:       5
   Unit Type:     DW_UT_compile (1)
   Abbrev Offset: 0x0
   Pointer Size:  8
 <0><c>: Abbrev Number: 1 (DW_TAG_compile_unit)
    <d>   DW_AT_producer    : (indexed string: 0x0): clang version 19.0.0git (https://github.com/llvm/llvm-project.git 80cff273906b200eed2f779913f49a64cad8c0c6)
    <e>   DW_AT_language    : 29	(C11)
    <10>   DW_AT_name        : (indexed string: 0x1): /root/llvm-project/lldb/test/API/functionalities/inline-sourcefile/main.c
    <11>   DW_AT_str_offsets_base: 0x8
    <15>   DW_AT_stmt_list   : 0x0
    <19>   DW_AT_comp_dir    : (indexed string: 0x2): /root/llvm-project/build/lldb-test-build.noindex/functionalities/inline-sourcefile/TestInlineSourceFiles.test_dwarf
    <1a>   DW_AT_low_pc      : (addr_index: 0x0): 714
    <1b>   DW_AT_high_pc     : 0x38
    <1f>   DW_AT_addr_base   : 0x8
 <1><23>: Abbrev Number: 2 (DW_TAG_subprogram)
    <24>   DW_AT_low_pc      : (addr_index: 0x0): 714
    <25>   DW_AT_high_pc     : 0x4
    <29>   DW_AT_frame_base  : 1 byte block: 6f 	(DW_OP_reg31 (sp))
    <2b>   DW_AT_name        : (indexed string: 0x3): stop
    <2c>   DW_AT_decl_file   : 1
    <2d>   DW_AT_decl_line   : 2
    <2e>   DW_AT_external    : 1
 <1><2e>: Abbrev Number: 3 (DW_TAG_subprogram)
    <2f>   DW_AT_low_pc      : (addr_index: 0x1): 718
    <30>   DW_AT_high_pc     : 0x34
    <34>   DW_AT_frame_base  : 1 byte block: 6d 	(DW_OP_reg29 (x29))
    <36>   DW_AT_name        : (indexed string: 0x4): main
    <37>   DW_AT_decl_file   : 1
    <38>   DW_AT_decl_line   : 4
    <39>   DW_AT_prototyped  : 1
    <39>   DW_AT_type        : <0x54>
    <3d>   DW_AT_external    : 1
 <2><3d>: Abbrev Number: 4 (DW_TAG_formal_parameter)
    <3e>   DW_AT_location    : 2 byte block: 91 78 	(DW_OP_fbreg: -8)
    <41>   DW_AT_name        : (indexed string: 0x6): argc
    <42>   DW_AT_decl_file   : 1
    <43>   DW_AT_decl_line   : 4
    <44>   DW_AT_type        : <0x54>
 <2><48>: Abbrev Number: 4 (DW_TAG_formal_parameter)
    <49>   DW_AT_location    : 2 byte block: 8f 10 	(DW_OP_breg31 (sp): 16)
    <4c>   DW_AT_name        : (indexed string: 0x7): argv
    <4d>   DW_AT_decl_file   : 1
    <4e>   DW_AT_decl_line   : 4
    <4f>   DW_AT_type        : <0x58>
 <2><53>: Abbrev Number: 0
 <1><54>: Abbrev Number: 5 (DW_TAG_base_type)
    <55>   DW_AT_name        : (indexed string: 0x5): int
    <56>   DW_AT_encoding    : 5	(signed)
    <57>   DW_AT_byte_size   : 4
 <1><58>: Abbrev Number: 6 (DW_TAG_pointer_type)
    <59>   DW_AT_type        : <0x5d>
 <1><5d>: Abbrev Number: 6 (DW_TAG_pointer_type)
    <5e>   DW_AT_type        : <0x62>
 <1><62>: Abbrev Number: 7 (DW_TAG_const_type)
    <63>   DW_AT_type        : <0x67>
 <1><67>: Abbrev Number: 5 (DW_TAG_base_type)
    <68>   DW_AT_name        : (indexed string: 0x8): char
    <69>   DW_AT_encoding    : 8	(unsigned char)
    <6a>   DW_AT_byte_size   : 1
 <1><6b>: Abbrev Number: 0
  Compilation Unit @ offset 0x6c:
   Length:        0x2c (32-bit)
   Version:       5
   Unit Type:     DW_UT_compile (1)
   Abbrev Offset: 0x6a
   Pointer Size:  8
 <0><78>: Abbrev Number: 1 (DW_TAG_compile_unit)
    <79>   DW_AT_producer    : (indexed string: 0x0): clang version 19.0.0git (https://github.com/llvm/llvm-project.git 80cff273906b200eed2f779913f49a64cad8c0c6)
    <7a>   DW_AT_language    : 29	(C11)
    <7c>   DW_AT_name        : (indexed string: 0x1): /root/llvm-project/lldb/test/API/functionalities/inline-sourcefile/main.c
    <7d>   Unknown AT value: 3e02: (indexed string: 0x2): /root/llvm-project/build/lldb-test-build.noindex/functionalities/inline-sourcefile/TestInlineSourceFiles.test_dwarf
    <7e>   DW_AT_str_offsets_base: 0x34
    <82>   DW_AT_stmt_list   : 0x7a
    <86>   DW_AT_comp_dir    : (indexed string: 0x3): stop
    <87>   DW_AT_low_pc      : (addr_index: 0x0): 74c
    <88>   DW_AT_high_pc     : 0x10
    <8c>   DW_AT_addr_base   : 0x20
 <1><90>: Abbrev Number: 2 (DW_TAG_subprogram)
    <91>   DW_AT_low_pc      : (addr_index: 0x0): 74c
    <92>   DW_AT_high_pc     : 0x10
    <96>   DW_AT_frame_base  : 1 byte block: 6f 	(DW_OP_reg31 (sp))
    <98>   DW_AT_name        : (indexed string: 0x4): main
    <99>   DW_AT_decl_file   : 1
    <9a>   DW_AT_decl_line   : 2
    <9b>   DW_AT_external    : 1
 <1><9b>: Abbrev Number: 0

Contents of the .debug_abbrev section:

  Number TAG (0x0)
   1      DW_TAG_compile_unit    [has children]
    DW_AT_producer     DW_FORM_strx1
    DW_AT_language     DW_FORM_data2
    DW_AT_name         DW_FORM_strx1
    DW_AT_str_offsets_base DW_FORM_sec_offset
    DW_AT_stmt_list    DW_FORM_sec_offset
    DW_AT_comp_dir     DW_FORM_strx1
    DW_AT_low_pc       DW_FORM_addrx
    DW_AT_high_pc      DW_FORM_data4
    DW_AT_addr_base    DW_FORM_sec_offset
    DW_AT value: 0     DW_FORM value: 0
   2      DW_TAG_subprogram    [no children]
    DW_AT_low_pc       DW_FORM_addrx
    DW_AT_high_pc      DW_FORM_data4
    DW_AT_frame_base   DW_FORM_exprloc
    DW_AT_name         DW_FORM_strx1
    DW_AT_decl_file    DW_FORM_data1
    DW_AT_decl_line    DW_FORM_data1
    DW_AT_external     DW_FORM_flag_present
    DW_AT value: 0     DW_FORM value: 0
   3      DW_TAG_subprogram    [has children]
    DW_AT_low_pc       DW_FORM_addrx
    DW_AT_high_pc      DW_FORM_data4
    DW_AT_frame_base   DW_FORM_exprloc
    DW_AT_name         DW_FORM_strx1
    DW_AT_decl_file    DW_FORM_data1
    DW_AT_decl_line    DW_FORM_data1
    DW_AT_prototyped   DW_FORM_flag_present
    DW_AT_type         DW_FORM_ref4
    DW_AT_external     DW_FORM_flag_present
    DW_AT value: 0     DW_FORM value: 0
   4      DW_TAG_formal_parameter    [no children]
    DW_AT_location     DW_FORM_exprloc
    DW_AT_name         DW_FORM_strx1
    DW_AT_decl_file    DW_FORM_data1
    DW_AT_decl_line    DW_FORM_data1
    DW_AT_type         DW_FORM_ref4
    DW_AT value: 0     DW_FORM value: 0
   5      DW_TAG_base_type    [no children]
    DW_AT_name         DW_FORM_strx1
    DW_AT_encoding     DW_FORM_data1
    DW_AT_byte_size    DW_FORM_data1
    DW_AT value: 0     DW_FORM value: 0
   6      DW_TAG_pointer_type    [no children]
    DW_AT_type         DW_FORM_ref4
    DW_AT value: 0     DW_FORM value: 0
   7      DW_TAG_const_type    [no children]
    DW_AT_type         DW_FORM_ref4
    DW_AT value: 0     DW_FORM value: 0
  Number TAG (0x6a)
   1      DW_TAG_compile_unit    [has children]
    DW_AT_producer     DW_FORM_strx1
    DW_AT_language     DW_FORM_data2
    DW_AT_name         DW_FORM_strx1
    Unknown AT value: 3e02 DW_FORM_strx1
    DW_AT_str_offsets_base DW_FORM_sec_offset
    DW_AT_stmt_list    DW_FORM_sec_offset
    DW_AT_comp_dir     DW_FORM_strx1
    DW_AT_low_pc       DW_FORM_addrx
    DW_AT_high_pc      DW_FORM_data4
    DW_AT_addr_base    DW_FORM_sec_offset
    DW_AT value: 0     DW_FORM value: 0
   2      DW_TAG_subprogram    [no children]
    DW_AT_low_pc       DW_FORM_addrx
    DW_AT_high_pc      DW_FORM_data4
    DW_AT_frame_base   DW_FORM_exprloc
    DW_AT_name         DW_FORM_strx1
    DW_AT_decl_file    DW_FORM_data1
    DW_AT_decl_line    DW_FORM_data1
    DW_AT_external     DW_FORM_flag_present
    DW_AT value: 0     DW_FORM value: 0

Raw dump of debug contents of section .debug_line:

  Offset:                      0x0
  Length:                      118
  DWARF Version:               5
  Address size (bytes):        8
  Segment selector (bytes):    0
  Prologue Length:             80
  Minimum Instruction Length:  1
  Maximum Ops per Instruction: 1
  Initial value of 'is_stmt':  1
  Line Base:                   -5
  Line Range:                  14
  Opcode Base:                 13

 Opcodes:
  Opcode 1 has 0 args
  Opcode 2 has 1 arg
  Opcode 3 has 1 arg
  Opcode 4 has 1 arg
  Opcode 5 has 1 arg
  Opcode 6 has 0 args
  Opcode 7 has 0 args
  Opcode 8 has 0 args
  Opcode 9 has 1 arg
  Opcode 10 has 0 args
  Opcode 11 has 0 args
  Opcode 12 has 1 arg

 The Directory Table (offset 0x22, lines 2, columns 1):
  Entry	Name
  0	(indirect line string, offset: 0x0): /root/llvm-project/build/lldb-test-build.noindex/functionalities/inline-sourcefile/TestInlineSourceFiles.test_dwarf
  1	(indirect line string, offset: 0x74): /root/llvm-project

 The File Name Table (offset 0x32, lines 2, columns 3):
  Entry	Dir	MD5				Name
  0	0 0x729aae838de0d2dd88e503cc6baa303d	(indirect line string, offset: 0x87): /root/llvm-project/lldb/test/API/functionalities/inline-sourcefile/main.c
  1	1 0x729aae838de0d2dd88e503cc6baa303d	(indirect line string, offset: 0x9a): lldb/test/API/functionalities/inline-sourcefile/main.c

 Line Number Statements:
  [0x0000005c]  Set column to 14
  [0x0000005e]  Set prologue_end to true
  [0x0000005f]  Extended opcode 2: set Address to 0x714
  [0x0000006a]  Special opcode 6: advance Address by 0 to 0x714 and Line by 1 to 2
  [0x0000006b]  Set column to 0
  [0x0000006d]  Special opcode 63: advance Address by 4 to 0x718 and Line by 2 to 4
  [0x0000006e]  Set column to 3
  [0x00000070]  Set prologue_end to true
  [0x00000071]  Advance PC by constant 17 to 0x729
  [0x00000072]  Special opcode 216: advance Address by 15 to 0x738 and Line by 1 to 5
  [0x00000073]  Set epilogue_begin to true
  [0x00000074]  Special opcode 118: advance Address by 8 to 0x740 and Line by 1 to 6
  [0x00000075]  Advance PC by 12 to 0x74c
  [0x00000077]  Extended opcode 1: End of Sequence


  Offset:                      0x7a
  Length:                      90
  DWARF Version:               5
  Address size (bytes):        8
  Segment selector (bytes):    0
  Prologue Length:             57
  Minimum Instruction Length:  1
  Maximum Ops per Instruction: 1
  Initial value of 'is_stmt':  1
  Line Base:                   -5
  Line Range:                  14
  Opcode Base:                 13

 Opcodes:
  Opcode 1 has 0 args
  Opcode 2 has 1 arg
  Opcode 3 has 1 arg
  Opcode 4 has 1 arg
  Opcode 5 has 1 arg
  Opcode 6 has 0 args
  Opcode 7 has 0 args
  Opcode 8 has 0 args
  Opcode 9 has 1 arg
  Opcode 10 has 0 args
  Opcode 11 has 0 args
  Opcode 12 has 1 arg

 The Directory Table (offset 0x9c, lines 2, columns 1):
  Entry	Name
  0	(indirect line string, offset: 0xd1): /Volumes/Data/llvm-project
  1	(indirect line string, offset: 0xec): /INLINE

 The File Name Table (offset 0xad, lines 2, columns 3):
  Entry	Dir	(Unknown format content type 8193)	Name
  0	0	(indirect line string, offset: 0x159): 	(indirect line string, offset: 0xf4): /INLINE/inlined.c
  1	1	(indirect line string, offset: 0x106): void stop();
void f() {
  // This is inline source code.
  stop(); // break here
}
	(indirect line string, offset: 0xfc): inlined.c

 Line Number Statements:
  [0x000000bf]  Extended opcode 2: set Address to 0x74c
  [0x000000ca]  Special opcode 6: advance Address by 0 to 0x74c and Line by 1 to 2
  [0x000000cb]  Set column to 3
  [0x000000cd]  Set prologue_end to true
  [0x000000ce]  Special opcode 63: advance Address by 4 to 0x750 and Line by 2 to 4
  [0x000000cf]  Set column to 1
  [0x000000d1]  Set epilogue_begin to true
  [0x000000d2]  Special opcode 62: advance Address by 4 to 0x754 and Line by 1 to 5
  [0x000000d3]  Advance PC by 8 to 0x75c
  [0x000000d5]  Extended opcode 1: End of Sequence


Contents of the .debug_str section:

  0x00000000 636c616e 67207665 7273696f 6e203139 clang version 19
  0x00000010 2e302e30 67697420 28687474 70733a2f .0.0git (https:/
  0x00000020 2f676974 6875622e 636f6d2f 6c6c766d /github.com/llvm
  0x00000030 2f6c6c76 6d2d7072 6f6a6563 742e6769 /llvm-project.gi
  0x00000040 74203830 63666632 37333930 36623230 t 80cff273906b20
  0x00000050 30656564 32663737 39393133 66343961 0eed2f779913f49a
  0x00000060 36346361 64386330 63362900 2f726f6f 64cad8c0c6)./roo
  0x00000070 742f6c6c 766d2d70 726f6a65 63742f6c t/llvm-project/l
  0x00000080 6c64622f 74657374 2f415049 2f66756e ldb/test/API/fun
  0x00000090 6374696f 6e616c69 74696573 2f696e6c ctionalities/inl
  0x000000a0 696e652d 736f7572 63656669 6c652f6d ine-sourcefile/m
  0x000000b0 61696e2e 63002f72 6f6f742f 6c6c766d ain.c./root/llvm
  0x000000c0 2d70726f 6a656374 2f627569 6c642f6c -project/build/l
  0x000000d0 6c64622d 74657374 2d627569 6c642e6e ldb-test-build.n
  0x000000e0 6f696e64 65782f66 756e6374 696f6e61 oindex/functiona
  0x000000f0 6c697469 65732f69 6e6c696e 652d736f lities/inline-so
  0x00000100 75726365 66696c65 2f546573 74496e6c urcefile/TestInl
  0x00000110 696e6553 6f757263 6546696c 65732e74 ineSourceFiles.t
  0x00000120 6573745f 64776172 66007374 6f70006d est_dwarf.stop.m
  0x00000130 61696e00 696e7400 61726763 00617267 ain.int.argc.arg
  0x00000140 76006368 61720063 6c616e67 20766572 v.char.clang ver
  0x00000150 73696f6e 2031382e 302e3067 69742028 sion 18.0.0git (
  0x00000160 67697440 67697468 75622e63 6f6d3a6c git@github.com:l
  0x00000170 6c766d2f 6c6c766d 2d70726f 6a656374 lvm/llvm-project
  0x00000180 2e676974 20323965 65363666 34613039 .git 29ee66f4a09
  0x00000190 36376534 33613033 35663134 37633936 67e43a035f147c96
  0x000001a0 30373433 63376236 34306632 6629002f 0743c7b640f2f)./
  0x000001b0 494e4c49 4e452f69 6e6c696e 65642e63 INLINE/inlined.c
  0x000001c0 002f002f 566f6c75 6d65732f 44617461 ././Volumes/Data
  0x000001d0 2f6c6c76 6d2d7072 6f6a6563 7400     /llvm-project.

Contents of the .debug_addr section:

  For compilation unit at offset 0x0:
	Index	Address
	0:	0000000000000714 
	1:	0000000000000718 
  For compilation unit at offset 0x6c:
	Index	Address
	0:	000000000000074c 

Contents of the .debug_line_str section:

  0x00000000 2f726f6f 742f6c6c 766d2d70 726f6a65 /root/llvm-proje
  0x00000010 63742f62 75696c64 2f6c6c64 622d7465 ct/build/lldb-te
  0x00000020 73742d62 75696c64 2e6e6f69 6e646578 st-build.noindex
  0x00000030 2f66756e 6374696f 6e616c69 74696573 /functionalities
  0x00000040 2f696e6c 696e652d 736f7572 63656669 /inline-sourcefi
  0x00000050 6c652f54 65737449 6e6c696e 65536f75 le/TestInlineSou
  0x00000060 72636546 696c6573 2e746573 745f6477 rceFiles.test_dw
  0x00000070 61726600 2f726f6f 742f6c6c 766d2d70 arf./root/llvm-p
  0x00000080 726f6a65 6374002f 726f6f74 2f6c6c76 roject./root/llv
  0x00000090 6d2d7072 6f6a6563 742f6c6c 64622f74 m-project/lldb/t
  0x000000a0 6573742f 4150492f 66756e63 74696f6e est/API/function
  0x000000b0 616c6974 6965732f 696e6c69 6e652d73 alities/inline-s
  0x000000c0 6f757263 6566696c 652f6d61 696e2e63 ourcefile/main.c
  0x000000d0 002f566f 6c756d65 732f4461 74612f6c ./Volumes/Data/l
  0x000000e0 6c766d2d 70726f6a 65637400 2f494e4c lvm-project./INL
  0x000000f0 494e4500 2f494e4c 494e452f 696e6c69 INE./INLINE/inli
  0x00000100 6e65642e 6300766f 69642073 746f7028 ned.c.void stop(
  0x00000110 293b0a76 6f696420 66282920 7b0a2020 );.void f() {.  
  0x00000120 2f2f2054 68697320 69732069 6e6c696e // This is inlin
  0x00000130 6520736f 75726365 20636f64 652e0a20 e source code.. 
  0x00000140 2073746f 7028293b 202f2f20 62726561  stop(); // brea
  0x00000150 6b206865 72650a7d 0a00              k here.}..

Contents of the .debug_names section:

Version 5
Augmentation string: 4c 4c 56 4d 30 37 30 30  ("LLVM0700")
CU table:
[  0] 0x6c

TU table:

Foreign TU table:

Used 1 of 1 bucket.
Out of 1 items there are 0 bucket clashes (longest of 0 entries).

Symbol table:
[  0] #0002b60b f: <1> DW_TAG_subprogram DW_IDX_die_offset=<0x24> DW_IDX_parent=1
Contents of the .debug_str_offsets section:

    Length: 0x28
    Version: 0x5
       Index   Offset [String]
           0        0 clang version 19.0.0git (https://github.com/llvm/llvm-project.git 80cff273906b200eed2f779913f49a64cad8c0c6)
           1       6c /root/llvm-project/lldb/test/API/functionalities/inline-sourcefile/main.c
           2       b6 /root/llvm-project/build/lldb-test-build.noindex/functionalities/inline-sourcefile/TestInlineSourceFiles.test_dwarf
           3      12a stop
           4      12f main
           5      134 int
           6      138 argc
           7      13d argv
           8      142 char
    Length: 0x18
    Version: 0x5
       Index   Offset [String]
           0      147 clang version 18.0.0git (git@github.com:llvm/llvm-project.git 29ee66f4a0967e43a035f147c960743c7b640f2f)
           1      1af /INLINE/inlined.c
           2      1c1 /
           3      1c3 /Volumes/Data/llvm-project
           4      128 f
```
