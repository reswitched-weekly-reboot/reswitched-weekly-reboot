+++
title = "Welcome to the first edition of ReSwitched Weekly (reboot)"
authors = ["Pokemod97", "substanc3", "pcy", "xyz"]
date = 2023-02-25
+++

[Reswitched Weekly](https://reswitched.github.io/blog/) was a blog covering the Nintendo Switch hacking scene as it developed from the point of view of the ReSwitched discord. It died out because the news slowed down. This attempted revival of ReSwitched Weekly continues the spirit of the original while expanding outside just the switch.  The ReSwitched Weekly reboot will consist of 2 formats - roundups, which will highlight the happenings in the community in the past week, and in-depth blog posts discussing a specific topic or event by an RS member. We're hoping to get lots of our great community members involved, showing off the cool things they have been working on. Let's start strong with a roundup of the 8th week of 2023!
<!-- more -->

Welcome to the attempted revival of ReSwitched Weekly.
## News
### Google Summer of Code
Google Summer of Code has released its [list of mentoring organizations](https://opensource.googleblog.com/2023/02/mentor-organizations-announced-for.html) for 2023. @Pokemod97 did it in the summer of 2021 and highly recommends it. For those who are unaware, Google Summer of Code is a program where Google pays college students to work on a project for an open-source organization, under a mentor, during the summer. It's a great alternative to an internship especially because it's available for multiple countries and fully remote. @Pokemod97 recommends contacting the organizations early and figure what you can do for them before applying. Good luck to all the college students who are applying.

## TIL
Today I Learned is a section that's gonna cover a selection of the interesting things the writers have found out about since the last roundup. Expect this to be a fun selection of factoids related to the world of hacking and much more!

### Gold vs GNU ld (spoiler: mold wins)
Gold is a [Google](https://opensource.googleblog.com/2008/04/gold-google-releases-new-and-improved.html) project that intends to create a linker faster than GNU ld and to make it a part of binutils.The project was started in 2008, but even though it has a ton of history attached to its name, don't get too excited. Unfortunately, it has fallen out of favor at Google, as they wish to focus more on LLVM for now. Fedora has split it into its own package instead of Binutils because of ["bitrot"](https://www.phoronix.com/news/GNU-Gold-Stagnate-F31). Don't worry, however, if you need to link things faster. Even though gold is likely already on your system, it is certainly not the only option, as [mold](https://github.com/rui314/mold) shows much more promise, both in the performance and the maintenance department. If you are looking to understand how gold and mold are designed for speed, you can check out [this blog post](https://www.airs.com/blog/archives/39) by the author of gold, and mold's [design notes](https://github.com/rui314/mold/blob/main/docs/design.md).
## Updates
This week, the Nintendo Switch received an update to the Horizon OS version 16.0.0, spelling a bit of trouble for homebrew users once again. While Atmosphère has been updated as swiftly as ever, the update came with some changes that break existing homebrew too, many of which will need updates.

The pl:s service now no longer gives applications access to the Switch's system fonts, meaning many homebrew applications will need to switch to the much more contested pl:u service. One of the most notable applications that needed this change is the Tesla overlay system. Unfortunately, the amount of processes that can access the service is limited to 5, of which the operating system uses 3 by default, which would cause an issue when trying to run a game, overlays, and a homebrew application using this service at the same time. Fortunately, Atmosphère has implemented a workaround freeing one of the 3 sessions used by the system, which will land in a future pre-release.

The ncm service has also received some updates breaking compatibility with homebrew that makes use of this service, which will need to be re-compiled with a new version of libnx.

However, not all updates to the OS have been homebrew-breaking. One notable update, in particular, happened in the Horizon Kernel, fixing a long-standing vulnerability that while not useful on its own, could have spelled trouble for the security of the system if combined with another exploit (of which there are not many, to be fair). Before 16.0.0, the kernel mapped its memory as both writable and executable into a set place in memory, allowing an attacker that already has some type of code execution in the kernel to bypass mitigations such as KASLR. While the kernel needs to do this at the start, the flaw stems from the fact that this area never seems to get unmapped. The fix seems to have been incidental, as it coincides with the change of the related code to be more versatile for use on new devices. Whatever the motivation behind this might be, it is yet another of the very few bugs remaining in the kernel being fixed as the kernel team at Nintendo keeps firing from all cylinders to create one of the most interesting pieces of software in modern history.

Of course, we can't fit all the goodies that have been added in 16.0.0 into this article, so if you're interested, go check a fuller changelog in the [usual places](https://switchbrew.org/wiki/16.0.0).

## Projects
### Tetris MBC5
[An interesting project by a ReSwitched member Y2K](https://github.com/Y2K-x/tetris-gb-disasm/tree/mbc5) aims to extend the classic Tetris Gameboy disassembly to allow for more modding. This improved version outputs a ROM in the MBC5 format and modifies the game code to allow more space for various experiments. By default, Tetris takes up all the address space available from the CPU for the cart. Memory Bank Controllers(MBC) work around this by changing the memory banks that the CPU is accessing in the cart on command. This is a jumping-off point for @Y2K to make further modifications to the game such as porting Tetris Gym to the Gameboy version of Tetris.
## DSi under Attack
[@pcy has successfully dumped the bootroms of the ARM9 and ARM7 CPUs of the DSi.](https://icosahedron.website/@pcy/109914279298940511)
These dumps are the first steps to finding a jailbreak attack on the bootroms, which is the subject of pcy's master's thesis. Such an attack would allow recovery from bricks caused by dead NANDs, as the latter suffers from bad wear leveling issues. Additional shoutout to @stuckpixel for his independent effort to dump the DSi bootrom.

## Other Blogposts
Shoutout to @Retroid's [blogpost about getting widevine running under Asahi Linux](https://www.da.vidbuchanan.co.uk/blog/netflix-on-asahi.html). 

## Coming up
### Xinu AARCH64
The operating systems class Pokemod97 is currently taking uses the [xinu](https://xinu.cs.purdue.edu/) operating system as the testing ground for the class. They currently run it on their BeagleBone Black(arm32), however, they plan to port the system to aarch64 QEMU and later perhaps the Nintendo Switch (I mean hey, we're ReSwitched after all...). The progress made so far consists of modifying a [bare metal qemu aarch64 hello world](https://github.com/Pokemod97/armv8-hello) project to use clang as the compiler.


