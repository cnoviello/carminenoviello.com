+++
title = "Conditional breakpoint while debugging STM32"
slug = "conditional-breakpoint-debugging-stm32"
url = "/2015/06/09/conditional-breakpoint-debugging-stm32/"
date = "2015-06-09T16:34:33Z"
lastmod = "2015-06-09T16:34:33Z"
draft = false
description = "It's a really common situation when working with hardware (especially while debugging asynchronous events): to stop execution while debugging only if a given event occurs. This is also called conditional…"
categories = ["Programming","STM32"]
tags = []
showHero = true
showTableOfContents = true

[cover]
image = "images/legacy/conditional-breakpoint-debugging-stm32/cover-conditional-breakpoint.jpg"
alt = "conditional breakpoint"
hiddenInSingle = false
+++

It's a really common situation when working with hardware (especially while debugging asynchronous events): to stop execution while debugging only if a given event occurs. This is also called conditional breakpoint.

If you are working with the STM32 family and the CMSIS ARM package for Cortex-M processors, and your toolchain is GCC-based with GDB as debugger, you can place in your code this instruction:

``` c
#include "cortexm/ExceptionHandlers.h"
...
if(condition) {
    __DEBUG_BKPT();
}
...
```

GDB will automatically stop when the event occurs at that line.

This saved my life. Definitively.
