
#AVLeak

AVLeak is a tool for fingerprinting consumer antivirus emulators through automated black box testing. AVLeak can be used to extract fingerprints from AV emulators that may be used by malware to detect that it is being analyzed and subsequently evade detection, including environmental artifacts, OS API behavioral inconsistencies, emulation of network connectivity, timing inconsistencies, process introspection, and CPU emulator "red pills.”

Emulator fingerprints may be discovered through painstaking binary reverse engineering, or with time consuming black box testing using binaries that conditionally choose to behave benignly or drop malware based on the emulated environment. AVLeak significantly advances upon prior approaches to black box testing, allowing researchers to extract emulator fingerprints in just a few seconds, and to script out testing using powerful APIs.

AVLeak will be demoed live, showing real world fingerprints discovered using the tool that can be used to detect and evade popular consumer AVs including Kaspersky, Bitdefender engine (licensed out to 20+ other AV products), AVG, and VBA. This survey of emulation detection methods is the most comprehensive examination of the topic ever presented in one place.

[Black Hat 2016 Video]: https://www.youtube.com/watch?v=a6yOwvFds78