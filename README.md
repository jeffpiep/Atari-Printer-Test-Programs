# Atari-Printer-Test-Programs
Here I have different Atari BASIC programs for testing printers. Some come from the field service manuals and others were written to test behavior. Some where found in the pigwa FTP archive. This repository originated from writing printer simulators for the [FujiNet project](https://github.com/FujiNetWIFI) and needing to validate their behavior. Below is some discussion on each program and links to relevant source material.

## Atari 820
The [Atari 820 Field Service Manual](https://archive.org/details/FD100048_Atari820FieldServiceManual/page/n53/mode/2up) has a type-in program and sample output for testing the printer. The version here I called T820.BAS has a couple statements removed from the original. It appears the original had some incomplete algorithm to make it loop, perhaps like the later T0127.BAS does.

I wrote some new test programs for the Atari 820 to check out its characeter sets and behavior, especially in the peculiar "sideways" mode. There are:
* CHARSET.BAS - prints out a numbered characeter set between ASCII 32 and 127 in normal mode.
* SIDESET.BAS - prints out a numbered characeter set between ASCII 32 and 127 in sideways mode.
* MORE820.BAS - explores some behavior of combining normal and sideways modes. This program crashes my 130XE but not Altirra.

These programs are on the [A820.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/A820.ATR) disk image.

[ANTIC Magazine Vol.2 No.10](https://archive.org/details/1984-01-anticmagazine/page/n31/mode/2up) has two type-in programs that use the 820 to print a [pocket-sized calendar](https://www.atarimagazines.com/v2n10/PocketCalendar1984.html). I included the CALENDAR.BAS and SIDEWRIT.BAS programs on the ATR as well.

The [Atari Home Computer Technical Reference Notes](https://archive.org/details/bitsavers_atari40080mputerTechnicalReferenceNotes1982_20170986/page/n179/mode/2up) has some description of the Atari 820, too.

## Atari 822
Page 7 of the [Atari 822 Operator's Manual](https://archive.org/details/atari_822_operators_manual/page/n7/mode/2up) contains a type-in BASIC program to plot a GRAPHICS 8 screen and print it on the Atari 822. That program is on the [A822.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/A822.ATR) image.

## Atari 825
Page 2 of the [Atari 825 Operator's Manual](https://archive.org/details/Atari825PrinterOperatorsManual/page/n5/mode/2up) shows the 3 different character sets in normal and elongated mode. An original BASIC program "A825CHAR.BAS" that recreates this page is on the [A825.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/A825.ATR) image. 

## Atari 1020
The program T1020.BAS is cited in the [Atari 1020 Field Service Manual](https://archive.org/details/atari1020colorprinterfieldservicemanualrev.011983atari/page/n31/mode/2up). Sample printouts are shown in the manual. The program can be found on the [Atari FTP Archive](http://ftp.pigwa.net/stuff/collections/holmes%20cd/Holmes%202/Programming/Basic/index.html) or on the [PRINTERS.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/PRINTERS.ATR) disk image.

## Atari 1025
The program T1025.BAS can be found on the [Atari FTP Archive](http://ftp.pigwa.net/stuff/collections/holmes%20cd/Holmes%202/Programming/Basic/index.html) or on the [PRINTERS.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/PRINTERS.ATR) disk image.

## Atari 1027
The program T1027.BAS is cited in the [Atari 1027 Field Service Manual](https://archive.org/details/Atari1027PrinterFieldServiceManualRev01/page/n19/mode/2up). The manual has sample output from the program, although I think what is printed in the manual was not generated with the exact program found online. Use caution when viewing the sample output in a PDF as there are two versions of the manual: one is scanned showing the original 1027 font (Prestige Elite?) and the other uses PDF built-in Adobe Type1 Courier font. If you have a restored 1027 and would run this program, a scanned image of your output would be appreciated. The program (and two other test programs for the 1020 and 1025) can be found on the [Atari FTP Archive](http://ftp.pigwa.net/stuff/collections/holmes%20cd/Holmes%202/Programming/Basic/index.html) or on the [PRINTERS.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/PRINTERS.ATR) disk image.

## Atari 1029
The program A1029CHR.BAS prints out all the Atari 1029 character sets documented in the [Atari 1029 Programmable Printer Manual](https://atariage.com/forums/applications/core/interface/file/attachment.php?id=496311) (or in [Italian](https://archive.org/details/atari1029it/mode/2up)). Thank-you to Łukasz Maśko of the [Atari 8-Bit Computers](https://www.facebook.com/groups/181644898539691) FB group for debugging this program on his real, working Atari 1029 printer.

## Okimate 10

The [OKIMATE.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/OKIMATE.ATR) disk image contains two test programs and the [T1025.BAS](https://github.com/jeffpiep/Atari-Printer-Test-Programs/blob/master/README.md#atari-1025) program. The Okimate 10 was Atari 1025 compatible.

The program MNLDEMOS.BAS is a compilation of the short demo programs scattered throughout the [Okimate 10 Printer Handbook for Atari Computers](http://www.atarimania.com/8bit/files/Okimate_10_Printer_Handbook_Okidata.pdf). There is a horizontal position command that moves the printhead over by a number of dot spaces. The manual shows the number as a three ASCII character string. The "D:LEARN" program on the [pack-in disk](http://www.atarimania.com/utility-atari-400-800-xl-xe-okimate-10-atari-software_33598.html), however, outputs the number as three bytes, each byte ranges 0-9 and forms a decimal number as hundreds, tens, and ones places. The example in MNLDEMOS.BAS does the same. 

The program COLORS.BAS is an Atari BASIC translation of a program found in the [Okidata Okimate 10 Printer Manual for Commod'e(R) Computers](ftp://cbm8bit.com/hardware/manuals/Okimate_10_Printer_Manual_(Revised_1985_Jul).pdf) which prints samples of all the colors.
