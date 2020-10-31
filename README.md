# ESP32 reversing
A curated list of ESP32 related reversing resources

- [ESP32 Reversing](#esp32-reversing)
    - [Hardware](#hardware)
    - [Firmware](#firmware)
        - [Bootloader](#bootloader)
        - [bin2elf](#bin2elf)
        - [ELF format](#elf)
    - [Debuggers](#debuggers)
        - [IDA](#ida)
        - [radare2](#radare2)
        - [Ghidra](#ghidra)
        - [gdb](#gdb)
    - [JTAG](#jtag)
    - [QEMU](#qemu)
    - [Books](#books)
    - [Git](#git)
    - [Links](#links)
    - [Fun](#fun)

- - -


## Hardware

### ESP32 general

- [ESP32 datasheet](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [Xtensa®Instruction Set Architecture (ISA)](https://0x04.net/~mwk/doc/xtensa.pdf)
- [ABI Interface/Argument passing](http://wiki.linux-xtensa.org/index.php/ABI_Interface)
- [An short guide to Xtensa assembly language](http://cholla.mmto.org/esp8266/xtensa.html)
- Nullcon Goa 2018: Expanding Exploitation Beyond X86 And ARM : [slides](https://nullcon.net/website/archives/pdf/goa-2018/carel-nullcon-arm-vs-xtensa-exploitation-%28final%29.pdf), [video](https://www.youtube.com/watch?v=DNl2ykqBB4U)


### NNCBadge2019
- [Official info](https://2019.nonamecon.org/badge)
- [Write-ups by VVS](https://gitlab.com/coders-in-ua/nonamebadge-2019-ctf)
- Some basic hacking techniques via example: NoNameCon badge by Oleksii Sobolevskyi [video](https://www.facebook.com/watch/?v=2357574994326811&extid=7aponckVbhwv81gY), [slides](https://speakerdeck.com/macpawtechtalks/some-basic-hacking-techniques-via-example-nonamecon-badge-by-oleksii-sobolevskyi)
- [NoNameBadge 2019 - Public Version](https://gitlab.com/techmaker/nnc-badge-2019)

### NNCBadge2020
- [Official info](https://nonamecon.org/nonamebadge-2-0/)

- - -

## Firmware

- [API Reference](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/index.html)
- [App Image Format](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/system/app_image_format.html)
- [Reversing ESP8266 Firmware (Part 1..6)](https://boredpentester.com/category/reverse-engineering/)
- [Reverse Engineering ESP8266, rus](https://habr.com/ru/post/255135/)

### Bootloader

- [ESP8266 BOOT PROCESS](https://richard.burtons.org/2015/05/17/esp8266-boot-process/)
- [DECOMPILING THE ESP8266 BOOT LOADER V1.3(B3)](https://richard.burtons.org/2015/05/17/decompiling-the-esp8266-boot-loader-v1-3b3/)

### BIN2ELF

- [ESP32 Firmware Image to ELF](https://github.com/tenable/esp32_image_parser)
- [Tiny project allows converting ESP32 ROM blob to ELF file with symbols](https://github.com/gschorcht/esp32-elf-rom)
- [Converts a flash dump from an esp8266 device into an ELF executable](https://github.com/jsandin/esp-bin2elf)

- Extracting_an_ELF_from_an_ESP32,Chris Lyne and Nick Miles (Shmoocon 2020) 
[video](https://www.youtube.com/watch?v=w4_3vwN_2dI), [slides](https://github.com/tenable/presentations/blob/master/Extracting_an_ELF_from_an_ESP32/Extracting_an_ELF_from_an_ESP32_2020.pdf), [tool](https://github.com/tenable/esp32_image_parser)

### ELF

- [The 101 of ELF files on Linux: Understanding and Analysis](https://linux-audit.com/elf-binaries-on-linux-understanding-and-analysis/#elf-sections)

- - -

## Debuggers

### IDA
#### Plug-ins

- [Flare IDA](https://github.com/fireeye/flare-ida)
- [Processor plugin for IDA 7.x, to support the Xtensa](https://github.com/themadinventor/ida-xtensa)
- [A loader for the esp-idf application images for IDA Pro](https://github.com/jrozner/esp-image-ida)
- [A list of IDA Plugins](https://github.com/onethawt/idaplugins-list)
- [IDA export symbols plugin by BlackVS](https://github.com/BlackVS/IDA-exportsymbols)

#### Signatures, IDA

- [Using and Making IDA Pro Signatures (Flirt)](https://rvsec0n.wordpress.com/2019/09/21/using-and-making-ida-pro-signatures-flirt/)
- [IDA SigMaker Plugin updated for the IDA Pro 7.0 SDK by dude719](https://github.com/ajkhoury/SigMaker-x64)

- - -
### radare2
- [Awesome Radare2](https://github.com/radareorg/awesome-radare2)
- [ESIL](https://monosource.gitbooks.io/radare2-explorations/content/tut3/tut3_-_esil.html)
- [ESIL Solve](https://github.com/aemmitt-ns/esilsolve)
- [asm options](https://r2wiki.readthedocs.io/en/latest/options/e/values-that-e-can-modify/asm/)

#### CTF with Radare2

- [CTF solving using radare2 / Blogs](https://r2wiki.readthedocs.io/en/latest/home/ctf-solving-using-radare2/)
- [Знакомство с Radare2](https://forum.reverse4you.org/t/radare-2/1113)
- [Emulating a MIPS binary with radare2](http://chasekanipe.com/writeups/emulatingmips.pdf)

- - -
### Ghidra

- [Ghidra](https://ghidra-sre.org/)
- [Tensilica Xtensa module for Ghidra](https://github.com/yath/ghidra-xtensa)

- - -
### gdb

#### Plug-ins

- [console UI for gdb](https://github.com/cyrus-and/gdb-dashboard)
- - -

## JTAG

## QEMU

- [ESP32 in QEMU](https://github.com/Ebiroll/qemu_esp32)

- - -

## Books

- [Kolban's book on ESP32](https://leanpub.com/kolban-ESP32), Free download

- - -

## Git

- ]Neil Kolban](https://github.com/nkolban)
- [ELF reader-writer library for Python3](https://github.com/v3l0c1r4pt0r/makeelf)

- - -

## Links

- [Tom Trebisky's ESP32 notes](http://cholla.mmto.org/esp32/)
- [A curated list of awesome reversing resources](https://github.com/tylerha97/awesome-reversing)
- [Awesome Reverse Engineering](https://github.com/ReversingID/Awesome-Reversing)
- [lucadentella.it , ESP32 tutorials](http://www.lucadentella.it/en/category/esp32/)
- [ESP32: Анализ использования оперативной памяти](https://www.terraelectronica.ru/news/6231)

- - -

## Fun

- [Pwn the ESP32 Forever: Flash Encryption and Sec. Boot Keys Extraction](https://limitedresults.com/2019/11/pwn-the-esp32-forever-flash-encryption-and-sec-boot-keys-extraction/)

### z3 and reverse

- [SAT/SMT by Example Dennis Yurichev](https://yurichev.com/writings/SAT_SMT_by_example.pdf)
- [Intro to Binary Analysis with Z3 and angr](https://github.com/FSecureLABS/z3_and_angr_binary_analysis_workshop)
- [Code & screenshots for various Z3 based CTF challenge writeups](https://github.com/sam-b/z3-stuff)
- [Writeup: Sharky CTF 2020 - Z3 Robot](https://cesena.github.io/2020/05/13/z3-robot/)
- [PicoCTF 2018 - Reverse Engineering writeups](https://shizz3r.blogspot.com/2019/03/picoctf-2018-reverse-engineering.html)
- [PicoCTF 2018 Writeup: Reversing](https://tcode2k16.github.io/blog/posts/picoctf-2018-writeup/reversing/)


