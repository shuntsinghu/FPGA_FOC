# README

==！！工程尚未完成，持续更新中==

主要参考了 [WangXuan95/FpOC: FPGA-based Field Oriented Control (FOC) for driving BLDC/PMSM motor. 基于FPGA的FOC控制器，用于驱动BLDC/PMSM电机。 (github.com)](https://github.com/WangXuan95/FpOC) 这个工程似乎并没有上板验证，只是做了仿真，所以拿来并不能直接使用。我又根据我驱动板，编码器，电机的类型对程序进行适当的增删。但是很感谢 @WangXuan95 给我提供了思路，FOC程序的主要部分也是参考了他的程序。



主控使用的是[正点原子领航者ZYNQ开发板-tmall.com](https://detail.tmall.com/item.htm?abbucket=16&id=609032204975&ns=1&spm=a230r.1.14.13.39db6253bBDgJ8) 板载Xilinx XC7Z020clg400-2 FPGA芯片；电机使用的是[正点原子PMSM永磁同步电机-tmall.com](https://detail.tmall.com/item.htm?abbucket=1&id=676540034988&rn=002b74d6b804291c8b19e05b5231c03e&spm=a1z10.3-b-s.w4011-24686329152.28.13347467Jtka6Z) 8对磁极，自带HALL传感器和增量式光电编码器。电机驱动板[正点原子直流无刷电机驱动板ATK-PD6010B模块-tmall.com](https://detail.tmall.com/item.htm?spm=a220o.1000855.0.0.1fd81f6eV2i9bx&id=676336444645)，用户手册可以在[正点原子开源平台](http://www.openedv.com/docs/boards/stm32dj/index.html)下载，讲解视频可以在[B站](](https://www.bilibili.com/video/BV1hv4y1g7s3/?spm_id_from=333.999.0.0&vd_source=6fb5644884544e3f03e705a82bc176ae))观看，不过讲解的不甚详细，FOC部分也是讲了用力和用STM32库创建的工程。