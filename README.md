# XGpioPs_Config & XGpioPs_LookupConfig函数的用法
## 1.1定义
`XGpioPs_Config`是一个由 Xilinx 提供的结构体，通常用于描述Zynq系列处理器中的PS GPIO配置。`XGpioPs_Config` 结构体包含了 GPIO 控制器的硬件配置信息。
`XGpioPs_LookupConfig`函数根据设备ID查找和返回一个 GPIO 配置结构体的指针。
## 1.2实例
`XGpioPs_Config *mio_cfg_ptr;`
`mio_cfg_ptr = XGpioPs_LookupConfig(GPIO_DEVICE_ID);`

先声明一个指向`XGpioPs_Config`的指针，再通过`XGpioPs_LookupConfig`函数根据设备ID查找和返回一个 GPIO 配置结构体的指针。它查找硬件配置并返回一个指向 `XGpioPs_Config` 类型的指针。
