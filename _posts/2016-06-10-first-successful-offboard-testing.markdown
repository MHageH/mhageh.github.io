---
layout: post
title: "First successful offboard testing"
date : 2016-05-28 22:00:00 +0200
categories : Misc
---

First stable start of the drone, after a number of failures, from an offboard computer :
[Footage](http://jmfriedt.sequanux.org/mohamed/20160609_202506.mp4)

Note that the drone kept its position relative to x and y axis, and climbed further in the z axis (as requested by the set_point command). The offboard computer for this footage is a Linux PC, but will reproduce the same effect on the STM32F4 evaluation board.
The commanding software is the modified C UART Interface that much likely run as same as the original version. The behavior of this software is theorized to be exact on STM32F4 (confirmed by simulation, need effective testing on the field), yet more tests will be done to assure the reliability of this code.