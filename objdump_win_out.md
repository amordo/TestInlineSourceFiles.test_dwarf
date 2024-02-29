# $ objdump --dwarf a.out # produced on Windows
```

a.out:     file format pei-x86-64

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

Contents of the .debug_addr section:

  For compilation unit at offset 0x0:
        Index   Address
        0:      0000000140001000 
        1:      0000000140001010 
  For compilation unit at offset 0x6c:
        Index   Address
        0:      0000000140001040 

Contents of the .debug_info section:

  Compilation Unit @ offset 0x0:
   Length:        0x68 (32-bit)
   Version:       5
   Unit Type:     DW_UT_compile (1)
   Abbrev Offset: 0x0
   Pointer Size:  8
 <0><c>: Abbrev Number: 1 (DW_TAG_compile_unit)
    <d>   DW_AT_producer    :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74000
 (indexed string: 0x0): <indirect index offset is too big>
    <e>   DW_AT_language    : 29        (C11)
    <10>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff7406c
 (indexed string: 0x1): <indirect index offset is too big>
    <11>   DW_AT_str_offsets_base: 0x8
    <15>   DW_AT_stmt_list   : 0x0
    <19>   DW_AT_comp_dir    :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff740c2
 (indexed string: 0x2): <indirect index offset is too big>
    <1a>   DW_AT_low_pc      : (addr_index: 0x0): 140001000
    <1b>   DW_AT_high_pc     : 0x31
    <1f>   DW_AT_addr_base   : 0x8
 <1><23>: Abbrev Number: 2 (DW_TAG_subprogram)
    <24>   DW_AT_low_pc      : (addr_index: 0x0): 140001000
    <25>   DW_AT_high_pc     : 0x1
    <29>   DW_AT_frame_base  : 1 byte block: 57         (DW_OP_reg7 (rsp))
    <2b>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74142
 (indexed string: 0x3): <indirect index offset is too big>
    <2c>   DW_AT_decl_file   : 1
    <2d>   DW_AT_decl_line   : 2
    <2e>   DW_AT_external    : 1
 <1><2e>: Abbrev Number: 3 (DW_TAG_subprogram)
    <2f>   DW_AT_low_pc      : (addr_index: 0x1): 140001010
    <30>   DW_AT_high_pc     : 0x21
    <34>   DW_AT_frame_base  : 1 byte block: 57         (DW_OP_reg7 (rsp))
    <36>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74147
 (indexed string: 0x4): <indirect index offset is too big>
    <37>   DW_AT_decl_file   : 1
    <38>   DW_AT_decl_line   : 4
    <39>   DW_AT_prototyped  : 1
    <39>   DW_AT_type        : <0x54>
    <3d>   DW_AT_external    : 1
 <2><3d>: Abbrev Number: 4 (DW_TAG_formal_parameter)
    <3e>   DW_AT_location    : 2 byte block: 91 24      (DW_OP_fbreg: 36)
    <41>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff7415a
 (indexed string: 0x8): <indirect index offset is too big>
    <42>   DW_AT_decl_file   : 1
    <43>   DW_AT_decl_line   : 4
    <44>   DW_AT_type        : <0x54>
 <2><48>: Abbrev Number: 4 (DW_TAG_formal_parameter)
    <49>   DW_AT_location    : 2 byte block: 91 28      (DW_OP_fbreg: 40)
    <4c>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74150
 (indexed string: 0x6): <indirect index offset is too big>
    <4d>   DW_AT_decl_file   : 1
    <4e>   DW_AT_decl_line   : 4
    <4f>   DW_AT_type        : <0x58>
 <2><53>: Abbrev Number: 0
 <1><54>: Abbrev Number: 5 (DW_TAG_base_type)
    <55>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff7414c
 (indexed string: 0x5): <indirect index offset is too big>
    <56>   DW_AT_encoding    : 5        (signed)
    <57>   DW_AT_byte_size   : 4
 <1><58>: Abbrev Number: 6 (DW_TAG_pointer_type)
    <59>   DW_AT_type        : <0x5d>
 <1><5d>: Abbrev Number: 6 (DW_TAG_pointer_type)
    <5e>   DW_AT_type        : <0x62>
 <1><62>: Abbrev Number: 7 (DW_TAG_const_type)
    <63>   DW_AT_type        : <0x67>
 <1><67>: Abbrev Number: 5 (DW_TAG_base_type)
    <68>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74155
 (indexed string: 0x7): <indirect index offset is too big>
    <69>   DW_AT_encoding    : 6        (signed char)
    <6a>   DW_AT_byte_size   : 1
 <1><6b>: Abbrev Number: 0
  Compilation Unit @ offset 0x6c:
   Length:        0x2c (32-bit)
   Version:       5
   Unit Type:     DW_UT_compile (1)
   Abbrev Offset: 0x6a
   Pointer Size:  8
 <0><78>: Abbrev Number: 1 (DW_TAG_compile_unit)
    <79>   DW_AT_producer    :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74000
 (indexed string: 0x0): <indirect index offset is too big>
    <7a>   DW_AT_language    : 29       (C11)
    <7c>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff7406c
 (indexed string: 0x1): <indirect index offset is too big>
    <7d>   Unknown AT value: 3e02:objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff740c2
 (indexed string: 0x2): <indirect index offset is too big>
    <7e>   DW_AT_str_offsets_base: 0x34
    <82>   DW_AT_stmt_list   : 0x7c
    <86>   DW_AT_comp_dir    :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74142
 (indexed string: 0x3): <indirect index offset is too big>
    <87>   DW_AT_low_pc      : (addr_index: 0x0): 140001040
    <88>   DW_AT_high_pc     : 0xf
    <8c>   DW_AT_addr_base   : 0x20
 <1><90>: Abbrev Number: 2 (DW_TAG_subprogram)
    <91>   DW_AT_low_pc      : (addr_index: 0x0): 140001040
    <92>   DW_AT_high_pc     : 0xf
    <96>   DW_AT_frame_base  : 1 byte block: 57         (DW_OP_reg7 (rsp))
    <98>   DW_AT_name        :objdump: Warning: DW_FORM_GNU_str_index indirect offset too big: 0xfffffffebff74147
 (indexed string: 0x4): <indirect index offset is too big>
    <99>   DW_AT_decl_file   : 1
    <9a>   DW_AT_decl_line   : 2
    <9b>   DW_AT_external    : 1
 <1><9b>: Abbrev Number: 0

Raw dump of debug contents of section .debug_line:

  Offset:                      0x0
  Length:                      120
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
  Entry Name
  0objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a000
        (indirect line string, offset: 0x4008a000): <offset is too big>
  1objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a080
        (indirect line string, offset: 0x4008a080): <offset is too big>

 The File Name Table (offset 0x32, lines 2, columns 3):
  Entry Dir     MD5                             Name
  0     0 0x729aae838de0d2dd88e503cc6baa303dobjdump: Warning: DW_FORM_line_strp offset too big: 0x4008a09f
        (indirect line string, offset: 0x4008a09f): <offset is too big>
  1     1 0x729aae838de0d2dd88e503cc6baa303dobjdump: Warning: DW_FORM_line_strp offset too big: 0x4008a0f5
        (indirect line string, offset: 0x4008a0f5): <offset is too big>

 Line Number Statements:
  [0x0000005c]  Set column to 14
  [0x0000005e]  Set prologue_end to true
  [0x0000005f]  Extended opcode 2: set Address to 0x140001000
  [0x0000006a]  Special opcode 6: advance Address by 0 to 0x140001000 and Line by 1 to 2
  [0x0000006b]  Set column to 0
  [0x0000006d]  Special opcode 231: advance Address by 16 to 0x140001010 and Line by 2 to 4
  [0x0000006e]  Set column to 3
  [0x00000070]  Set prologue_end to true
  [0x00000071]  Advance PC by constant 17 to 0x140001021
  [0x00000072]  Special opcode 62: advance Address by 4 to 0x140001025 and Line by 1 to 5
  [0x00000073]  Special opcode 76: advance Address by 5 to 0x14000102a and Line by 1 to 6
  [0x00000074]  Set is_stmt to 0
  [0x00000075]  Set epilogue_begin to true
  [0x00000076]  Special opcode 33: advance Address by 2 to 0x14000102c and Line by 0 to 6
  [0x00000077]  Advance PC by 5 to 0x140001031
  [0x00000079]  Extended opcode 1: End of Sequence


  Offset:                      0x7c
  Length:                      92
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

 The Directory Table (offset 0x9e, lines 2, columns 1):
  Entry Name
  0objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a12c
        (indirect line string, offset: 0x4008a12c): <offset is too big>
  1objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a147
        (indirect line string, offset: 0x4008a147): <offset is too big>

 The File Name Table (offset 0xaf, lines 2, columns 3):
  Entry Dir     (Unknown format content type 8193)      Name
  0     0objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a161
        (indirect line string, offset: 0x4008a161): <offset is too big>objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a14f
        (indirect line string, offset: 0x4008a14f): <offset is too big>
  1     1objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a16c
        (indirect line string, offset: 0x4008a16c): <offset is too big>objdump: Warning: DW_FORM_line_strp offset too big: 0x4008a162
        (indirect line string, offset: 0x4008a162): <offset is too big>

 Line Number Statements:
  [0x000000c1]  Extended opcode 2: set Address to 0x140001040
  [0x000000cc]  Special opcode 6: advance Address by 0 to 0x140001040 and Line by 1 to 2
  [0x000000cd]  Set column to 3
  [0x000000cf]  Set prologue_end to true
  [0x000000d0]  Special opcode 63: advance Address by 4 to 0x140001044 and Line by 2 to 4
  [0x000000d1]  Set column to 1
  [0x000000d3]  Special opcode 76: advance Address by 5 to 0x140001049 and Line by 1 to 5
  [0x000000d4]  Set is_stmt to 0
  [0x000000d5]  Set epilogue_begin to true
  [0x000000d6]  Special opcode 19: advance Address by 1 to 0x14000104a and Line by 0 to 5
  [0x000000d7]  Advance PC by 5 to 0x14000104f
  [0x000000d9]  Extended opcode 1: End of Sequence


Contents of the .debug_line_str section:

  0x14008a000 433a5c55 73657273 5c69616d 6d6f726a C:\Users\iammorj
  0x14008a010 6a5c6c6c 766d2d70 726f6a65 63745c62 j\llvm-project\b
  0x14008a020 75696c64 5c6c6c64 622d7465 73742d62 uild\lldb-test-b
  0x14008a030 75696c64 2e6e6f69 6e646578 5c66756e uild.noindex\fun
  0x14008a040 6374696f 6e616c69 74696573 5c696e6c ctionalities\inl
  0x14008a050 696e652d 736f7572 63656669 6c655c54 ine-sourcefile\T
  0x14008a060 65737449 6e6c696e 65536f75 72636546 estInlineSourceF
  0x14008a070 696c6573 2e746573 745f6477 61726600 iles.test_dwarf.
  0x14008a080 433a5c55 73657273 5c69616d 6d6f726a C:\Users\iammorj
  0x14008a090 6a5c6c6c 766d2d70 726f6a65 63740043 j\llvm-project.C
  0x14008a0a0 3a5c5573 6572735c 69616d6d 6f726a6a :\Users\iammorjj
  0x14008a0b0 5c6c6c76 6d2d7072 6f6a6563 745c6c6c \llvm-project\ll
  0x14008a0c0 64625c74 6573745c 4150495c 66756e63 db\test\API\func
  0x14008a0d0 74696f6e 616c6974 6965735c 696e6c69 tionalities\inli
  0x14008a0e0 6e652d73 6f757263 6566696c 655c6d61 ne-sourcefile\ma
  0x14008a0f0 696e2e63 006c6c64 625c7465 73745c41 in.c.lldb\test\A
  0x14008a100 50495c66 756e6374 696f6e61 6c697469 PI\functionaliti
  0x14008a110 65735c69 6e6c696e 652d736f 75726365 es\inline-source
  0x14008a120 66696c65 5c6d6169 6e2e6300 2f566f6c file\main.c./Vol
  0x14008a130 756d6573 2f446174 612f6c6c 766d2d70 umes/Data/llvm-p
  0x14008a140 726f6a65 6374002f 494e4c49 4e45002f roject./INLINE./
  0x14008a150 494e4c49 4e452f69 6e6c696e 65642e63 INLINE/inlined.c
  0x14008a160 0000696e 6c696e65 642e6300 766f6964 ..inlined.c.void
  0x14008a170 2073746f 7028293b 0a766f69 64206628  stop();.void f(
  0x14008a180 29207b0a 20202f2f 20546869 73206973 ) {.  // This is
  0x14008a190 20696e6c 696e6520 736f7572 63652063  inline source c
  0x14008a1a0 6f64652e 0a202073 746f7028 293b202f ode..  stop(); /
  0x14008a1b0 2f206272 65616b20 68657265 0a7d0a00 / break here.}..

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
Contents of the .debug_str section:

  0x14008c000 636c616e 67207665 7273696f 6e203139 clang version 19
  0x14008c010 2e302e30 67697420 28687474 70733a2f .0.0git (https:/
  0x14008c020 2f676974 6875622e 636f6d2f 6c6c766d /github.com/llvm
  0x14008c030 2f6c6c76 6d2d7072 6f6a6563 742e6769 /llvm-project.gi
  0x14008c040 74203464 30346134 30616462 36386632 t 4d04a40adb68f2
  0x14008c050 38343335 30383331 39313161 36353837 84350831911a6587
  0x14008c060 31353133 34633636 64382900 433a5c55 15134c66d8).C:\U
  0x14008c070 73657273 5c69616d 6d6f726a 6a5c6c6c sers\iammorjj\ll
  0x14008c080 766d2d70 726f6a65 63745c6c 6c64625c vm-project\lldb\
  0x14008c090 74657374 5c415049 5c66756e 6374696f test\API\functio
  0x14008c0a0 6e616c69 74696573 5c696e6c 696e652d nalities\inline-
  0x14008c0b0 736f7572 63656669 6c655c6d 61696e2e sourcefile\main.
  0x14008c0c0 6300433a 5c557365 72735c69 616d6d6f c.C:\Users\iammo
  0x14008c0d0 726a6a5c 6c6c766d 2d70726f 6a656374 rjj\llvm-project
  0x14008c0e0 5c627569 6c645c6c 6c64622d 74657374 \build\lldb-test
  0x14008c0f0 2d627569 6c642e6e 6f696e64 65785c66 -build.noindex\f
  0x14008c100 756e6374 696f6e61 6c697469 65735c69 unctionalities\i
  0x14008c110 6e6c696e 652d736f 75726365 66696c65 nline-sourcefile
  0x14008c120 5c546573 74496e6c 696e6553 6f757263 \TestInlineSourc
  0x14008c130 6546696c 65732e74 6573745f 64776172 eFiles.test_dwar
  0x14008c140 66007374 6f70006d 61696e00 696e7400 f.stop.main.int.
  0x14008c150 61726776 00636861 72006172 67630063 argv.char.argc.c
  0x14008c160 6c616e67 20766572 73696f6e 2031382e lang version 18.
  0x14008c170 302e3067 69742028 67697440 67697468 0.0git (git@gith
  0x14008c180 75622e63 6f6d3a6c 6c766d2f 6c6c766d ub.com:llvm/llvm
  0x14008c190 2d70726f 6a656374 2e676974 20323965 -project.git 29e
  0x14008c1a0 65363666 34613039 36376534 33613033 e66f4a0967e43a03
  0x14008c1b0 35663134 37633936 30373433 63376236 5f147c960743c7b6
  0x14008c1c0 34306632 6629002f 494e4c49 4e452f69 40f2f)./INLINE/i
  0x14008c1d0 6e6c696e 65642e63 002f002f 566f6c75 nlined.c././Volu
  0x14008c1e0 6d65732f 44617461 2f6c6c76 6d2d7072 mes/Data/llvm-pr
  0x14008c1f0 6f6a6563 74006600                   oject.f.

Contents of the .debug_str_offsets section:

    Length: 0x28
    Version: 0x5
       Index   Offset [String]
           0        0 clang version 19.0.0git (https://github.com/llvm/llvm-project.git 4d04a40adb68f284350831911a658715134c66d8)
           1       6c C:\Users\iammorjj\llvm-project\lldb\test\API\functionalities\inline-sourcefile\main.c
           2       c2 C:\Users\iammorjj\llvm-project\build\lldb-test-build.noindex\functionalities\inline-sourcefile\TestInlineSourceFiles.test_dwarf
           3      142 stop
           4      147 main
           5      14c int
           6      150 argv
           7      155 char
           8      15a argc
    Length: 0x18
    Version: 0x5
       Index   Offset [String]
           0      15f clang version 18.0.0git (git@github.com:llvm/llvm-project.git 29ee66f4a0967e43a035f147c960743c7b640f2f)
           1      1c7 /INLINE/inlined.c
           2      1d9 /
           3      1db /Volumes/Data/llvm-project
           4      1f6 f
```
