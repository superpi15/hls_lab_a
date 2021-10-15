# hls_lab_a
HLS lab a 

* Xilinx tool suit Version 2020.2
* [Vivado HLS has separated into two products: Vivado and Vitis](https://support.xilinx.com/s/question/0D52E00006lKUo6SAG/i-installed-vivado-20211-but-in-the-installed-software-vitis-hls-is-present-and-not-vivado-hls-why-is-vivado-hls-removed-is-vitis-hls-better-than-vivado-hls?language=en_US)
* [Vivado HLS manual 2020.1](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2020_1/ug871-vivado-high-level-synthesis-tutorial.pdf)

## pragma highlights
* loop
  * unroll
  * loop_flatten
* pipeline 
* latency 
  * when RTL cannot meet timing requirements, manually specify min/max delay of a scope
* array_partition 
  * use several BRAM to mitigate port count bottlenecks 
* reshape
  * partition data into BRAMs in order to relieve the insufficient number of BRAM ports
* ap_fifo
  * enabling streaming data transfer 
* Reference: https://www.xilinx.com/html_docs/xilinx2019_1/sdaccel_doc/hls-pragmas-okr1504034364623.html 

## bottlenecks
* IO port count of RAM
* data dependency 
