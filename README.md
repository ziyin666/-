//需要额外引入的头文件
#include <stdio.h>
#include "SD.h"
#include "ff.h"
#include "integer.h"

//额外声明这个数组
extern SD_HandleTypeDef hsd;
//在MX_SDIO_SD_Init();后调用，避免因为初始化速率过高，挂起失败
hsd.Init.BusWide = SDIO_BUS_WIDE_1B;

//先使用atof将字符串转为double ，在将double 强转为float即可使用
double numberDouble = atof(char nub);
float numberFloat = (float)numberDouble;

函数的使用https://blog.csdn.net/qq_36347513/article/details/121776975
MX的设置https://blog.csdn.net/qq_49053936/article/details/145316195
