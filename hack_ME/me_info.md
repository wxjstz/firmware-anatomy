## Info about ME

"If you know the enemy and know yourself, you need not fear the result of a hundred battles. If you know yourself but not the enemy, for every victory gained you will also suffer a defeat. If you know neither the enemy nor yourself, you will succumb in every battle." ---  Sun Tzu 

We should know our enemeies from RING 3/0/-1/-2 and espeically the "devil" from RING -3 world.

## Slide

* [Introducing Ring -3 Rootkit - 2009-08](https://www.blackhat.com/presentations/bh-usa-09/TERESHKIN/BHUSA09-Tereshkin-Ring3Rootkit-SLIDES.pdf)
* [A Quest To The Core - 2009-09](http://invisiblethingslab.com/resources/misc09/Quest%20To%20The%20Core%20(public).pdf)
* [Security Evaluation of Intel's Active Management Technology - 2010](https://people.kth.se/~maguire/DEGREE-PROJECT-REPORTS/100402-Vassilios_Ververis-with-cover.pdf)
* [Intel AMT/ME Meet Intel's hardware backdoor - 2012-09](www.uberwall.org/bin/download/download/102/lacon12_intel_amt.pdf)
* [Rootkit in your laptop - 2012-10](http://me.bios.io/images/c/ca/Rootkit_in_your_laptop.pdf)
* [Intel ME Secrets - 2014-06](https://recon.cx/2014/slides/Recon%202014%20Skochinsky.pdf), [video1](https://www.youtube.com/watch?v=4kCICUPc9_8), [video2](https://www.youtube.com/watch?v=Y2_-VXz9E-w)
* [Intel ME: Two Years Later - 2014-10](https://github.com/skochinsky/papers/raw/master/2014-10%20%5BBreakpoint%5D%20Intel%20ME%20-%20Two%20Years%20Later.pdf)
* [Reversing firmware using radare2 - 2014-10](http://xvilka.me/h2hc2014-reversing-firmware-radare-slides.pdf)


## Article/paper

* [mysteries_intel.txt - 2012-07](https://code.coreboot.org/p/flashrom/source/tree/HEAD/trunk/Documentation/mysteries_intel.txt)
* [Intel Management Engine - 2012-10](http://vpro.by/intel-management-engine)
* [Intel x86 considered harmful - 2015-10](https://blog.invisiblethings.org/papers/2015/x86_harmful.pdf)
* [Безопасность прошивок на примере подсистемы Intel Management Engine - 2016-03](https://habrahabr.ru/company/dsec/blog/278549/)
* [Intel ME. Как избежать восстания машин? - 2016-04](https://habrahabr.ru/company/dsec/blog/282546/)
* [Why is the latest Intel hardware unsupported in libreboot?](https://libreboot.org/faq/#intelme)
* [Intel ME info on coreboot's wiki](https://www.coreboot.org/Intel_Management_Engine)
* [me.bios.io](http://me.bios.io), contains some early research about ME: [ME blob format](http://me.bios.io/ME_blob_format) might need update, get a proper version of [GNU toolchain for ARC](https://github.com/foss-for-synopsys-dwc-arc-processors/toolchain) and then try [ARC disassembly](http://me.bios.io/ARC_disassembly) on earlier ME versions.
* [Starting point of minimizing ME](https://www.coreboot.org/pipermail/coreboot/2016-November/082331.html) and see the [current status of me_cleaner](https://github.com/corna/me_cleaner/issues/3).
* [Neutralize ME firmware on SandyBridge and IvyBridge platforms](https://hardenedlinux.github.io/firmware/2016/11/17/neutralize_ME_firmware_on_sandybridge_and_ivybridge.html) is an operational manual and we [have done it on some mainboards](https://github.com/hardenedlinux/hardenedlinux_profiles/tree/master/coreboot)( including a Skylake-based one) so far.
* [Safeguarding rootkits: Intel BootGuard - 2016-12](https://github.com/flothrone/bootguard), ME is original set as ["Manufacturing Mode" until "OEM Public Key Hash" and "Boot Guard Profile Configuration" being copied to CPU fuses](https://trmm.net/Bootguard) to make it either enable or disable. Alexander Ermolov shows us the ["Schrodinger's Bootguard" is neither in enabled or disabled](https://support.lenovo.com/us/en/solutions/len_9903), which can be exploited for further persistent uses.


## Free/libre open source tools
* [me_cleaner](https://github.com/corna/me_cleaner/), neutralize the ME by minimizing its functions.
* [me-tools](https://github.com/skochinsky/me-tools), extract code modules for further understanding.
* [intelmetool](https://github.com/zamaudio/intelmetool), get info from ME via [MEI interfaces](https://www.kernel.org/doc/Documentation/misc-devices/mei/mei.txt) on GNU/Linux
* [MEAnalyzer](https://github.com/platomav/MEAnalyzer), show details of a image contains ME firmware.
* [Intel ME (Manageability engine) Huffman algorithm](https://io.netgarage.org/me/)
* [Intel Management Engine: Drivers, Firmware & System Tools](http://www.win-raid.com/t596f39-Intel-Management-Engine-Drivers-Firmware-amp-System-Tools.html), it's up-to-date Windows-only tools.

## News
* [Intel & ME, and why we should get rid of ME](https://www.fsf.org/blogs/licensing/intel-me-and-why-we-should-get-rid-of-me), by FSF( Free software foundation)
* [Researchers find vulnerability in older versions of Intel ME, but you probably don't need to worry](http://www.digitaltrends.com/computing/intel-me-vulnerability/)
