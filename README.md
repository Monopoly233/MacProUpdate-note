# MacProUpdate-note&log 
this is a MacPro2009 Upgrade note for me

It is not that easy so I have to record those process

to remind me in the next update

## How did it all begin

I acquired this Mac Pro 2009 probably two or three years ago, and then, following various online tutorials, I managed to update it to macOS13.4.1 a few months ago

Over the past two to three years, I gradually installed modern hardware components into my Mac Pro. These include a Wi-Fi-enabled network card, two SATA storage drives, and an RX580 4GB graphics card. I also upgraded the CPU to two X5690 processors and increased the memory to 128GB

It took me a lot of time and money, but each time I updated, I had to seek help for the same issues repeatedly. So, this document is intended to record all the problems that occur during system updates

# The common issues

## Graphics card driver installation failed, resulting in lagging

open core legacy patcher provide a bunch of patch, If you keep their original patches, it will lead to lagging, and keeping their original patches makes it impossible to update. So you need to disable their original patches, but if you disable their patches, it will result in a black screen. If you don't want to end up with a black screen, you must keep their original patches, leading to an endless loop.

this problem can be fixed by safe boot, because my mac pro has no keyboard allowed me to press the key when boot

so just type this code in terminal 

'''sudo nvram boot-args="-x"'''
