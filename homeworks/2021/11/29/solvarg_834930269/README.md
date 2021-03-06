# Chapter.9 虚拟内存

---------------

## 什么是虚拟内存

虚拟内存为一个进程提供了一个大的、一致的私有的地址空间。  
- 1. 它将主存看成是一个存储在磁盘上的地址空间的高速缓存
- 2. 为每一个进程提供了一致的地址空间
- 3. 保护了每个进程的地址空间不被其他进程破坏

## 为什么要理解虚拟内存

- 1. 它是核心的,了解他有助于了解系统是如何工作的
- 2. Power,可以加载与卸载一个内存片
- 3. 理解段错误,保护错误等

## 虚拟内存作为缓存的工具

虚拟内存被组织为一个`由存放在磁盘上的N个连续的字节大小的单元组成的数组`,**每个字节都有一个位移的虚拟地址**

虚拟内存又被分割为`虚拟页`，虚拟页对应的是缓存到`物理页`上

DRAM: `磁盘到主存的缓存映射`  
SRAM: `CPU和驻村之间的L1,L2,L3高速缓存映射`

通常磁盘比DRAM慢10W多倍,因此,DRAM不命中比SRAM不命中要昂贵得多  
以及DRAM查找第一个字节的时候的消耗比读这个扇区中国连续字节的消耗也要昂贵的多

DRAM是全相连的,即任何物理页都可以映射到任何虚拟页上

## 页表

页表是用来存储虚拟页到物理页映射的一个索引表(Page Table Entry,页表条目)









--------------


> Latex转Svg

https://www.latexlive.com/