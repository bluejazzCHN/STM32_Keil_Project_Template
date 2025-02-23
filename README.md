### Project Structure
```
Project/
├── Keil_Project/
│   ├── MDK-ARM/             // Keil工程文件（.uvprojx, .uvoptx）
│   └── Objects/            // 编译输出文件（.axf, .map, .hex）
├── Drivers/
│   ├── CMSIS/              // CMSIS核心文件（由CubeMX生成）
│   ├── STM32xx_HAL_Driver/ // ST官方HAL库
│   └── BSP/                // 板级支持包（核心）
│       ├── Inc/            // BSP头文件
│       │   ├── bsp_gpio.h
│       │   ├── bsp_uart.h
│       │   └── bsp_led.h
│       └── Src/            // BSP源文件
│           ├── bsp_gpio.c
│           ├── bsp_uart.c
│           └── bsp_led.c
├── Middlewares/
│   ├── FreeRTOS/           // RTOS中间件（可选）
│   └── FatFS/              // 文件系统（可选）
├── Application/
│   ├── Inc/                // 应用层头文件
│   │   ├── app_main.h
│   │   └── app_task.h
│   └── Src/                // 应用层源文件
│       ├── app_main.c
│       └── app_task.c
├── Utilities/
│   ├── debug_log/          // 调试日志工具
│   └── common/             // 通用工具（队列、内存管理等）
└── STM32CubeMX_Config/
    ├── Inc/                // CubeMX生成的头文件（main.h, gpio.h等）
    └── Src/                // CubeMX生成的初始化代码（main.c, gpio.c等）
```
