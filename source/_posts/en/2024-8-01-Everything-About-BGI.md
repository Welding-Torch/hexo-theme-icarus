---
layout: post
title: Everything About BGI
date: 2024-8-01
toc: true
author: Siddharth Bhatia
---

# WinBGIm (Windows Borland Graphics Interface and Mouse)

Developed at the Computer Science department of the University of Colorado.

# History

1987 - Borland invents BGI  
1995 (probably because he made this on Windows 95) - Konstantin Knizhnik creates WinBGI  
1998 (or earlier) - Michael Main creates WinBGIm  
2021 to Jan 2022 - Shakil Ahmed (Bangladesh) creates WinBGIm-64

https://home.cs.colorado.edu/~main/cs1300/doc/bgi/index.html and https://winbgim.codecutter.org/V6*0/doc/ are the same documentation  
Similarily  
https://home.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html and https://winbgim.codecutter.org/V6*0/doc/bgi.html

# People Involved

-   Konstantin Knizhnik (AFAIK the original developer of WinBGI)
-   Michael Main (AFAIK the primary developer of WinBGIm)

# Versions

-   WinBGI shareware developed by Konstantin Knizhnik at ISPRAS(Institute of System Programming Russian Academy of Sciences). Created: August, 2004. README is here: https://home.cs.colorado.edu/~main/bgi/doc/knizhnik.txt
-   WinBGIm (Windows BGI - with mouse) version 6.0 was maintained and distributed by Michael Main at the University of Colorado http://www.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html
-   WinBGIm for MinGW a.k.a for the GCC Compiler by Al Stevens made some extremely trivial changes to WinBGIm. Created: November 2005. Last Modified: July 2006.

# Documentation for WinBGIm

is hosted here: https://home.cs.colorado.edu/~main/bgi/doc/  
Functions without the 'Win' tag are originally from BGI. Functions with the 'Win' tag are unique to WinBGIm.

# Konstantin

http://www.garret.ru/lang.html (scroll down to 'BGI for Windows')  
My e-mail address:  
knizhnik@cecmow.enet.dec.com

"  
BGI emulation  
PtoC now provides emulation libraries of Borland Graphics Interface (BGI) for X-Windows and Windows-95/NT are included in this distribution (BGI emulators can be also used without converter for C programs using BGI). I found source code of BGI emulator for X-Windows in Internet, so I only have to do some changes and fix few bugs. Unfortunately this emulation library is not fully completed and tested, also not all BGI functionality is supported. And BGI emulator for MS-Windows I created myself (in Internet I found only commercial products). I called this library WinBGI.  
WinBGI strictly emulates most of BGI functions (except using of non-standard drivers). Also may be mapping of fonts is not correct. But as far as sources are also available, you can easily customize them for your application. Unfortunately direct work with palette colors (setpalette, setbkcolor, write and putimage modes other than COPYPUT) is supported only for 256-colors Windows mode. Also I have used this library for only few programs (bgidemo is certainly the most complex one) so I can't guaranty that all functions always work properly. I am also sorry for the lack of parameter checking in WinBGI functions.  
"  
- from http://www.garret.ru/ptoc/Readme.htm#winbgi

GitHub for original WinBGI: https://github.com/knizhnik/ptoc/tree/master/WinBGI

FUN FACT: Years later, he actually got a job at Borland Co, Moscow branch! He was employed there from 2003-2006.

# University Of Colorado (1998/2004 - 2016)

CS1300 BGI Graphics Exercises - https://home.cs.colorado.edu/~main/bgi/cs1300/lab/cs1300-3.html  
Note: WinBGIm contains its own versions of getch, delay, and kbhit. You do not need to include conio.h to use these functions.  
Mouse Stuff Explanation: https://home.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html  
Use with Visual Studio: https://home.cs.colorado.edu/~main/bgi/visual/

# Codecutter (2005 - 2011)

https://winbgim.codecutter.org/  
https://winbgim.codecutter.org/V6\_0/doc/initwindow.html  
The site was last updated in 2011.  
AFAIK, Al Stevens is the developer of all the projects at codecutter.org. This includes CodeBlocks Edu, Koolplot, Quincy C/C++ IDE, MakeGen(used to generate makefiles compatible with the free Borland C/C++ compiler),

Al Steven's Personal Website: http://www.alstevens.com/bio.html

# Actually Modern BGI Projects (2023)

-   https://sdl-bgi.sourceforge.io/  
    Description: SDL*bgi can be used to port old programs written for Turbo/Borland C to modern systems. And, of course, to write new graphics programs with minimal effort: BGI, once extremely popular, was probably the simplest way to implement presentation graphics in C programs. The same ease of programming can be obtained on modern systems. Programming fractals, cellular automata, geometry, physics models etc. is a breeze with SDL*bgi.

# Alternatives to WinBGIm

-   https://openbgi.sourceforge.net/ https://sourceforge.net/projects/openbgi/
-   https://gomphics.sourceforge.net/ https://sourceforge.net/projects/gomphics/files/
-   https://sourceforge.net/projects/graphicsmsvs/

# Additional Links

Jordan Hargrave's SVGA BGI drivers https://github.com/jharg93/SvgaBGI  
CodeBlocks Edu Portable includes WinBGIm. Recommended only if all other methods to run BGI programs on Windows fails. https://codeblocks.codecutter.org/  
Quincy C/C++ IDE includes WinBGIm. https://quincy.codecutter.org/

More BGI libraries here: https://home.cs.colorado.edu/~main/bgi/source/  
with the most recent update as early as 2016!

Sitemap of Uni Colorado Michael Main:  
https://www.xml-sitemaps.com/details-home.cs.colorado.edu-9234475b5.html

https://en.wikipedia.org/wiki/Borland*Graphics*Interface

Moscow State Industrial University
