# USBTO3DO-GOLDSTAR-GDO101M
这是Francois CARON的SATATO3DO项目https://github.com/FCare/SataTo3DO 的拓展，使用了集成电路来缩小体积并扩展至GOLDSTAR-GDO101M，具体使用方法请参考其方案

BOM: 最小系统：

U1 RP2040 PICO模块(兼容引脚功能看2040pico.jpg）

U2/U3 TXS0108EPWR TSSOP-20

U4 74LVC4245 TSSOP-24

X1 有源晶振OSC SMD7050 16.93Mhz

POWER FFC插座14P 1.25mm  （FFC & FPC Connectors POST PLATED VERT 14P 1.25mm）

CDROM FFC插座30P 1.25mm  （FFC & FPC Connectors POST PLATED VERT 30P 1.25mm）





如果你要在模块上建立一个读盘灯（同主机面板绿色读盘灯）：

你需要增加： R1：470Ω（SMD0603 或直插） LED：3MM（直插）

预留了电容的位置，可以不需要安装， C1/C2：220uf-470uf/10V(直插）  C3/C4/C5/C6：0.1uf（SMD0603）

反面预留了(+5V,D-,D+,GND)接口，可以安装一个USB母座，注意此接口要与2040模块要焊接连线，具体方法请参考PCB背面图示:注意，这里并没有HUB功能，只能使用其中的一个，其意义是省去一根TYPE-C的转换线。

注意，此板可用于SANYO_TRY_IMP-21J的使用，但主机面板绿色“读盘灯”显示会比较暗淡
