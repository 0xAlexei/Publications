
# Reverse Engineering Windows Defender's Windows Binary Emulator

* Presented at REcon Montreal, Black Hat USA, and DEF CON *

Windows Defender's `mpengine.dll` implements the core of Defender antivirus' functionality in an enormous ~11 MB, 30,000+ function DLL. 

In this presentation, we'll look at Defender's emulator for analysis of potentially malicious Windows PE binaries on the endpoint. To the best of my knowledge, there has never been a conference talk or publication on reverse engineering the internals of any antivirus binary emulator before.

I'll cover a range of topics including emulator internals (bytecode to intermediate language lifting and execution; memory management; Windows API emulation; NT kernel emulation; file system and registry emulation; integration with Defender's antivirus features; the virtual environment; etc.), how I built custom tooling to assist in reverse engineering and attacking the emulator; tricks that malicious binaries can use to evade or subvert analysis; and attack surface within the emulator. 

Code available at <https://github.com/0xAlexei/WindowsDefenderTools>
