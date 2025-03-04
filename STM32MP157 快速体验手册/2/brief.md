---
title: '小节前言'
sidebar_position: 1
---

# 小节前言

&emsp;&emsp;用户收到ATK-STM32MP157开发板后，出厂时已经固化好系统到核心板上eMMC储存上了。出厂系统**预装Yocto文件系统**。所以可以无需再烧写（固件）系统到开发板，直接上机测试或者使用。

&emsp;&emsp;但是由于以下原因用户可能需要更新出厂系统

&emsp;&emsp;（1）	由于资料出厂固件更新，可能优化或者更新了系统。

&emsp;&emsp;（2）	由于出厂系统被损坏，被修改或者删除了里面的文件，启动不起来，想恢复到出厂系统。

&emsp;&emsp;（3）	由于在学习过程中，根据驱动指南烧写了自己的内核、Uboot及系统，但是无法验证硬件功能，需要烧写回出厂系统，先验证硬件是否正常工作，再修改软件。

&emsp;&emsp;这里我们提供三种方法固化Linux系统到开发板，如下：<br />
&emsp;&emsp;（1）	Windows使用STM32CubeProgrammer固化Linux系统（需要安装Java环境，安装比较麻烦，用户要有足够的耐心去安装！如果不想在Windows下使用STM32CubeProgrammer，可直接到2.3小节使用Linux烧写固件），相当于线刷，需要使用USB3.0接口，请勿使用USB2.0接口（因为会烧写很慢！虽然板子OTG是2.0的），烧写1G文件系统整体耗时约6分钟。<br />
&emsp;&emsp;（2）	Linux使用STM32CubeProgrammer固化Linux系统（需要安装Java环境），相当于线刷，需要使用**USB3.0**接口，烧写1G文件系统整体耗时约6分钟。<br />
&emsp;&emsp;（3）	TF(SD)卡固化Linux系统烧，写1G文件系统，只需要2-3分钟。
