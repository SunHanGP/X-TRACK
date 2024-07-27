# X-Track - 2.0英寸PCB，嘉立创版本
感谢@FASTSHIFT的开源项目X-TRACK
此版本PCB完全基于 [FASTSHIFT/X-TRACK/2.0-inch](https://github.com/FASTSHIFT/X-TRACK/tree/2.0-inch) 版本微调，**但采用嘉立创DEA专业版绘制，元件编号齐全，方便直接下单(PCB/SMT都可以)**

## 硬件改动基本与2.0跟原版的改动一致
* 使用四层PCB，方便走线，PCB厚度 *1.6mm*
* 主控芯片AT32F403ACGU7 QFN48pin6*6**（注意原2.0用的AT32F403ACGT7 LQFP48pin7\*7）**
* 串口线片更换为 *CP2102*
* IMU更换为 *MPU6050*
* 地磁极更换为 *QMC6310* **(换成QMC6310U，6310没买到)**
* 增加了电池电量计 *BQ27220*, 由于电量计是ROM-Base, 固件需要通过SD卡持久化保存电量计数据
* PCB接口由原来的焊盘更换为 *GH1.25*, 方便安装
* USB接口更换为Type-C
* 电源网络使用覆铜覆盖( [电池购买 523450](https://m.tb.cn/h.gRCxnBpw4CXNIVr?tk=aSf93cC6xcm ) )
* 充电芯片挪至PCB背面，可以更好的散热
* GPS模块内部集成了LDO, 因此将GPS模块VCC直接接电池减小*3.3v LDO*负载，**TX、RX串联一个100欧电阻**( [HT1818Z3G5L 购买地址](https://m.tb.cn/h.gRCCOYWMzNhfpTW?tk=wUBG3cCSN8j ) )
* 充电指示灯挪至边缘

## 注意事项
* 由于地线和电源线均采用覆铜走线，对烙铁焊接不够友好，建议使用 **低温锡膏** 加 **风枪** 方式焊接。
* 焊接最好使用延长排线加长屏幕排线，方便安装进外壳（**新增了14PIN插接款屏幕的PCB**）[插接屏2.0寸](https://m.tb.cn/h.gRCAggSShlwLRUn?tk=XvCI3cCREUD )
* ***BQ27220*** 电量计是可选项，BGA封装对焊接不够友好，新手不推荐安装（建议使用嘉立创的优惠券，有免费SMT订单）

