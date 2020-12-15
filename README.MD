# NEST-C Data
본 저장소는 [NEST Compiler Project](https://github.com/etri/nest-compiler)에서 사용하는 Data를 포함한다.

![Glow Logo](./docs/nestc.png)


# 구성
## lib/VTA
- x86_sim : x86 환경에서 동작하는 EVTA 시뮬레이터 라이브러리
- zcu102 : zcu102 보드 환경에서 동작하는 EVTA 라이브러리
- zcu102_dbg : zcu102 보드 환경에서 디버깅 가능한 EVTA 라이브러리
- acl : ARM Cortex-A53에 최적화된 환경을 제공하는 라이브러리

## bitstreams
[Ultra96-V2](http://zedboard.org/product/ultra96-v2-development-board)와 [ZCU102](https://www.xilinx.com/products/boards-and-kits/ek-u1-zcu102-g.html) 보드에서 동작 가능한 EVTA bitstream을 포함한다
- ultra96_1x16_i8w8a32_15_15_18_17.bit
- ultra96_1x16_i8w8a32_16_15_18_17.bit
- zcu102_1x16_i8w8a32_15_15_18_17.bit
- zcu102_1x16_i8w8a32_16_15_18_17.bit
- zcu102_1x16_i8w8a32_16_16_19_18.bit
- zcu102_1x32_i8w8a32_15_15_18_17.bit
- zcu102_2_1x16_i8w8a32_15_15_18_17.bit
- zcu102_2_1x16_i8w8a32_16_15_18_17.bit
- zcu102_4_1x16_i8w8a32_16_15_18_17.bit

## models
[NEST Compiler Project](https://github.com/etri/nest-compiler)에서 사용하는 ONNX 모델을 포함한다
- GoogleNet V4 slim
- ResNet18 V1
- MobilNet V2
- ResNet50 V1
- ShuffleNet
- SqueezeNet

## Yaml
[NEST Compiler Project](https://github.com/etri/nest-compiler)에서 `양자화`를 위해서 사용하는 calibration 정보가 담긴 파일이며 ONNX 모델명별로 각각 다른 파일을 사용한다.
- googlenet_v4_slim.yaml	
- mobilenet.yaml	
- mobilenet_onnx.yaml	
- mxnet_exported_resnet18_calib_1.yaml	
- resnet50.yaml	
- shufflenet.yaml	
- squeezenet.yaml	

