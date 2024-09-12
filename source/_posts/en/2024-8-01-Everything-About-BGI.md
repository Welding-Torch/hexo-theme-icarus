---
layout: post
title: Everything About BGI
date: 2024-8-01
toc: true
author: Siddharth Bhatia
---
This is a short history of BGI (Borland Graphics Interface) which was once an extremely popular and easy way to implement presentation graphics in C programs. It is still used today to teach Computer Graphics at universities in India.  

`#include <graphics.h`  

This living document is still being worked on.  

## Quick Explanation
BGI: Borland Graphics Interface  
WinBGI: Borland Graphics Interface **for Windows**  
WinBGIm: Borland Graphics Interface for Windows **with mouse**  
WinBGIm-64: Borland Graphics Interface for Windows with mouse **supporting 64-bit computers**
<!-- more -->

## History

1987 - 1993 : Borland invents BGI  
1995 (probably because he made this on Windows 95) : Konstantin Knizhnik creates WinBGI  
1998 (or earlier) - 2016 : Michael Main creates WinBGIm  
2021 - Jan 2022 : Shakil Ahmed (Bangladesh) creates WinBGIm-64

<!-- 
## 1) BGI
http://www.thealmightyguru.com/Wiki/index.php?title=Borland_Graphics_Interface

## 2) WinBGI
WinBGI was developed by Konstantin Knizhnik.  
WinBGI README.txt: http://www.garret.ru/readme.txt
Konstantin Knizhnik's website: http://www.garret.ru/
His resume: http://www.garret.ru/resume.html

Allows you to run your old Turbo-C DOS applications in 32-bit mode
   in normal windows. So you can easily overcome all 64Kb limitations
   and getting 32-bit application by simple recompilation !

2) Graphics is much faster with WinBGI (because native Win32 API
   is used with minimal emulation overhead) in comparison with
   original application running in DOS session under Windows 
   (especially at my PPro-200 with NT). 
   Also it seems to me that some things (like switching of graphical 
   pages) are not working properly in DOS mode under Windows-NT.


## 3) WinBGIm
It's difficult to tell who worked on what parts of it, but I know that Michael Main started this thing as early as 1998 and then
It was also worked on by:
Grant Macklem (Grant.Macklem@colorado.edu)
Gregory Schmelter (Gregory.Schmelter@colorado.edu)
Alan Schmidt (Alan.Schmidt@colorado.edu)
Ivan Stashak (Ivan.Stashak@colorado.edu)

## 4) WinBGIm-64

## SDLBGI
WinBGI is developed by Guido Gonzato.  
In a "we've come full circle" turn of events, Konstantin has [referenced](http://www.garret.ru/lang.html#:~:text=Windows%20improved%20by-,Guido%20Gonzato,-)%3A%20xbgi%2D364) Guido Gonzato's work of "Xbgi" which became "[libXbgi](https://libxbgi.sourceforge.net/)" which became the SDL_bgi library, which is probably the best way to run `graphics.h` programs on modern computers.

a normal html comment -->

## Q and A
Q: Why did the CS department at the University of Colorado create WinBGIm?  
A: As far as I can tell, they did it because the computers around them had switched to Windows and they still wanted students to be able to learn and practice computer graphics programs written for BGI. So Michael Main and others worked on WinBGIm.  

Q: What is CSCI 1300?  
A: CSCI 1300, sometimes known as CS1300, is the university of Colorado Boulder's _Introduction to Computing Course_.  
WinBGIm was included in the Software Package for CS1300. It seems to have been used in the Labs sessions there. There's even a Lab exercise for it: https://home.cs.colorado.edu/~main/bgi/cs1300/lab/cs1300-3.html  

Q: What is the history of BGI  
A: It's a beautiful story about open source software, and how it can be picked up and worked on by anyone in the world. Konstantin Khiznik created a way to run Borland Graphics programs on Windows. Michael Main quickly forked the work and made WinBGIm which he worked on for several years, with collaborators at University of Colorado Boulder. Most recently, Sakhil Ahmed at Shahjalal University of Science and Technology in 

Q: How long was Michael Main working on WinBGIm?  
A: Michael Main was working on WinBGIm from [October 17, 1998](http://www.k3pgp.org/Notebook/Winbgi/winbgi.htm) (WinBGIm version 2.2) to November, 2005 (WinBGIm version 6.0). But there are updates to the source code as recently as December 2016.  

Q: Where is the source code for WinBGIm?  
A: Source Code: https://home.cs.colorado.edu/~main/cs1300/bgi  

Q: What's my souce?  
A: See [this](https://home.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html#:~:text=h%20header%20file.-,The%20source%20code.,-Sample%20programs%3A).  

**Note**  
Don't get confused between there two:  
1) The true source code of WinBGIm (updated 2016)  
https://home.cs.colorado.edu/~main/bgi/source/  

2) The mirrored source code in CS1300 (updated 2014)  
https://home.cs.colorado.edu/~main/cs1300/bgi/  

## People Involved

-   Konstantin Knizhnik (The original developer of WinBGI)
-   Michael Main (AFAIK the primary developer of WinBGIm)
-   Sakhil Ahmed (The developer of WinBGIm-64)

## Versions

-   WinBGI shareware developed by Konstantin Knizhnik at ISPRAS(Institute of System Programming Russian Academy of Sciences). README is here: https://home.cs.colorado.edu/~main/bgi/doc/knizhnik.txt
-   WinBGIm (Windows BGI - with mouse) version 6.0 was maintained and distributed by Michael Main at the University of Colorado http://www.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html
-   WinBGIm for MinGW a.k.a for the GCC Compiler by Al Stevens made some extremely trivial changes to WinBGIm. Created: November 2005. Last Modified: July 2006.

## Documentation for WinBGIm

is hosted here: https://home.cs.colorado.edu/~main/bgi/doc/  
Functions without the 'Win' tag are originally from BGI. Functions with the 'Win' tag are unique to WinBGIm.

## Konstantin

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

## WinBGIm (Windows Borland Graphics Interface and Mouse) at University Of Colorado Boulder(1998/2004 - 2016)

Developed at the Computer Science department of the University of Colorado Boulder.  

CS1300 BGI Graphics Exercises - https://home.cs.colorado.edu/~main/bgi/cs1300/lab/cs1300-3.html  
Note: WinBGIm contains its own versions of getch, delay, and kbhit. You do not need to include conio.h to use these functions.  
Mouse Stuff Explanation: https://home.cs.colorado.edu/~main/cs1300/doc/bgi/bgi.html  
Use with Visual Studio: https://home.cs.colorado.edu/~main/bgi/visual/

## Codecutter (2005 - 2011)

https://winbgim.codecutter.org/  
https://winbgim.codecutter.org/V6\_0/doc/initwindow.html  
The site was last updated in 2011.  
AFAIK, Al Stevens is the developer of all the projects at codecutter.org. This includes CodeBlocks Edu, Koolplot, Quincy C/C++ IDE, MakeGen(used to generate makefiles compatible with the free Borland C/C++ compiler),

Al Steven's Personal Website: http://www.alstevens.com/bio.html

## Actually Modern BGI Projects (2023)

-   https://sdl-bgi.sourceforge.io/  
    Description: SDL*bgi can be used to port old programs written for Turbo/Borland C to modern systems. And, of course, to write new graphics programs with minimal effort: BGI, once extremely popular, was probably the simplest way to implement presentation graphics in C programs. The same ease of programming can be obtained on modern systems. Programming fractals, cellular automata, geometry, physics models etc. is a breeze with SDL*bgi.

## Alternatives to WinBGIm

-   https://openbgi.sourceforge.net/ https://sourceforge.net/projects/openbgi/
-   https://gomphics.sourceforge.net/ https://sourceforge.net/projects/gomphics/files/
-   https://sourceforge.net/projects/graphicsmsvs/

## Additional Links

Jordan Hargrave's SVGA BGI drivers: https://github.com/jharg93/SvgaBGI  
CodeBlocks Edu Portable includes WinBGIm. Recommended only if all other methods to run BGI programs on Windows fails: https://codeblocks.codecutter.org/  
Quincy C/C++ IDE includes WinBGIm: https://quincy.codecutter.org/

More BGI libraries here: https://home.cs.colorado.edu/~main/bgi/source/  
with the most recent update as early as 2016!

Sitemap of Uni Colorado Michael Main:  
https://www.xml-sitemaps.com/details-home.cs.colorado.edu-9234475b5.html

https://en.wikipedia.org/wiki/Borland*Graphics*Interface

Moscow State Industrial University
