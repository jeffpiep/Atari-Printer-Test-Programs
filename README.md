# Atari-Printer-Test-Programs
Here I have different Atari BASIC programs for testing printers. Some come from the field service manuals and others were written to test behavior. This repository originated from writing printer simulators for the [FujiNet project](https://github.com/FujiNetWIFI) and needing to validate their behavior. Below is some discussion on each program and links to relevant source material.

## Atari 1027
The program T1027.BAS is cited in the [Atari 1027 Field Service Manual](https://archive.org/details/Atari1027PrinterFieldServiceManualRev01/page/n19/mode/2up). The manual has sample output from the program, although I think what is printed in the manual was not generated with the exact program found online. Use caution when viewing the sample output in a PDF as there are two versions of the manual: one is scanned showing the original 1027 font (Prestige Elite?) and the other uses PDF built-in Adobe Type1 Courier font. If you have a restored 1027 and would run this program, a scanned image of your output would be appreciated. The program (and two other test programs for the 1020 and 1025) can be found on the [Atari FTP Archive](http://ftp.pigwa.net/stuff/collections/holmes%20cd/Holmes%202/Programming/Basic/index.html) or on the [PRINTERS.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/PRINTERS.ATR) disk image.

## Atari 820
The [Atari 820 Field Service Manual](https://archive.org/details/FD100048_Atari820FieldServiceManual/page/n53/mode/2up) has a type-in program and sample output for testing the printer. The version here I called T820.BAS has a couple statements removed from the original. I appears the original had some incomplete algorithm to make it loop, perhaps like the later T0127.BAS does.

I wrote some new test programs for the Atari 820 to check out its characeter sets and behavior, especially in the peculiar "sideways" mode. There are:
* CHARSET.BAS - prints out a numbered characeter set between ASCII 32 and 127 in normal mode.
* SIDESET.BAS - prints out a numbered characeter set between ASCII 32 and 127 in sideways mode.
* MORE820.BAS - explores some behavior of combining normal and sideways modes.

These programs are on the [A820.ATR](https://github.com/jeffpiep/Atari-Printer-Test-Programs/raw/master/A820.ATR) disk image.

[ANTIC Magazine Vol.2 No.10](https://archive.org/details/1984-01-anticmagazine/page/n31/mode/2up) has two type-in programs that use the 820 to print a [pocket-sized calendar](https://www.atarimagazines.com/v2n10/PocketCalendar1984.html). I included the CALENDAR.BAS and SIDEWRIT.BAS programs on the ATR as well.

The [Atari Home Computer Technical Reference Notes](https://archive.org/details/bitsavers_atari40080mputerTechnicalReferenceNotes1982_20170986/page/n179/mode/2up) has some description of the Atari 820, too.

