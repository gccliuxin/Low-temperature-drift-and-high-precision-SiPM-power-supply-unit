# 极低温漂高精度SiPM供电单元 Low temperature drift， high-precision SiPM power supply unit

# 介绍 Introduction

SPU-01-S是专用于SiPM等光电器件的单通道供电单元，其具有2ppm/℃极低输出温漂、2mV高精度、8cm²尺寸紧凑等特点，并含有电流电压监控功能。 模块预留一路1-wire接口可直接对前端探测反馈调整电压输出，用户也可自行测量前端温度，通过Uart接口进行配置。

The SPU-01-S is a single-channel power supply unit specifically designed for photon-sensor devices such as SiPMs. It features an extremely low output temperature drift of 2 ppm/°C, high precision of 2 mV, and a compact size of 8 cm², along with current and voltage monitoring functions. The module includes a 1-wire interface that allows direct adjustment of the output voltage based on front-end detector feedback. Users can also measure the front-end temperature independently and configure settings via a UART interface.

<img width="867" height="474" alt="尺寸" src="https://github.com/user-attachments/assets/60f5bbe9-386c-4146-9b85-1280eec92fda" />


# SiPM（硅光电倍增管）是什么？What is SiPM？

SiPM（硅光电倍增管）是一种可以探测光子并将其转换为电流信号的半导体器件，常用于

A silicon photomultiplier (SiPM) is a semiconductor device that can detect light (photons) and convert it into a current signal.  SiPMs are applied in a large variety of applications in fields such as the following:  

- 核医学影像（PET、γ相机）Medical imaging (PET, gamma cameras)  
- 电离辐射测量 Radiation detectors and dosimeters  
- 显微技术（激光扫描显微镜、双光子显微镜、荧光显微镜）Microscopy (for example, confocal laser scanning microscopy, two-photon microscopy, fluorescence microscopy)  
- 天体物理 Astrophysics  
- 高能物理 High-energy physics (HEP)  
- X-ray成像 X-ray imaging  
- 激光雷达（LiDAR）

SiPM（硅光电倍增管）通常由几千上万个工作于盖革模式的雪崩光电二极管组成。工作于盖革模式时，需要提供一般为几十V的偏置电压使其超过雪崩电压，其增益与过电压（偏置电压 - 雪崩电压）相关，而其雪崩电压与温度有线性的关系。所以要保证SiPM增益的稳定性，准确温度测量、电压输出精度和反馈调整是必要的。

SiPMs (silicon photomultipliers) typically consist of several thousand to tens of thousands of avalanche photodiodes （SPAD）operating in Geiger mode. When operating in Geiger mode, a bias voltage—usually several dozen volts—is required to exceed the breakdown voltage. The gain is related to the overvoltage (bias voltage minus breakdown voltage), and the breakdown voltage has a linear relationship with temperature. Therefore, to ensure SiPM gain stability, accurate temperature measurement, precise voltage output, and feedback adjustment are essential.

# 性能参数 Parameters

| 特性parameters                        | 典型值（单位）Typical（Units）       | 备注（Conditions） |
| ------------------------------------- | ------------------------------------ | ------------------ |
| 温度稳定性<br />temperature stability | ±2（ppm/℃）                          | T=-40~85℃          |
| 输出电压范围<br />output voltage      | 25~50（V）                           |                    |
| 输出电压纹波<br />ripple              | Vp-p : 1（mV）<br />Vrms : 150（uV） | No Load            |
| 最大输出电流<br />max load current    | 10（mA）                             |                    |
| 输出电压精度<br />output precison     | 0.025（%）± 2（mV）                  | T=23±5℃            |
| 输出电压分辨率<br />output resolution | 1（mV）                              |                    |
| 电压监控精度<br />Vmon precision      | 0.05（%）± 2（mV）                   | T=23±5℃            |
| 电流监控精度<br />Imon precision      | 1（%）± 0.1（mA）                    |                    |
| 长期稳定度<br />long term stability   | 20（ppm/√kHr）                       |                    |
| 外形尺寸<br />dimension               | ≤4.0×2.0（cm）                       |                    |
| 工作输入电压<br />supply voltage      | DC 6~15（V）                         |                    |
| 工作温度<br />operating temperature   | -40~85（℃）                          |                    |

# 实测 Tests

<img width="1024" height="600" alt="SDS1204X_HD_PNG_2" src="https://github.com/user-attachments/assets/3a273c67-e704-4c3c-b1df-f8cc70676f65" />


图1 输出电压纹波（Vout=25V AC耦合 带宽限制20MHz 空负载）

figure1 output ripple（Vout=25V AC-coupled Bandwith 20MHz No load）

<img width="617" height="477" alt="温漂" src="https://github.com/user-attachments/assets/b922951c-ffe9-4482-95f9-713580eb1181" />


图2 输出电压温漂（T=-35~65℃ Vout=42v）

figure2 temperature drift（T=-35~65℃ Vout=42v）

# 订购 Ordering Options

| 型号 models | 描述 description           | 编码 product code |
| ----------- | -------------------------- | ----------------- |
| SPU-01-S    | 单通道SiPM供电模块标准型号 | SPU01S000         |

# 文档版本 Documents Verison 

2026-07-01	首次建立 first time created

# 关于 About

作者：刘欣  aptx4689lx@gmail.com

2015-至今	成都永新医疗设备股份有限公司 核辐射监测事业部 副首席科学家
2016-2019	清华大学	核能与核技术工程
2006-2011	大连理工大学 电子工程系

Author：Xin Liu aptx4689lx@gmail.com
2015-now    Chengdu Novelmedical Co.ltd - Chief Scientist
2016-2019   Tsinghua University - Nuclear Science and Technology
2006-2011	Dalian University of Technology - Electronic and Engineering

