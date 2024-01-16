# WorkFlow


## Replacing SiLU with HardSwish
[Replacing with HardSwish](https://github.com/amitpant7/Replacing-Silu-in-efficientnetV2-with-Hard-Swish)
    Replacing all the SiLU activation functions from efficientnetv2 with HardSwish as they are computationaly cheaper, it will make FPGA implementation faster

## Pruning the EfficientNetV2:
 - [Unstructured Pruning](https://github.com/amitpant7/Pruning_efficienet_v2.git)
        Magnitude-based unstructured pruning to eliminate less valuable parameters from the network. I was able to prune 81% weights.  
 - [Channel Pruning](https://github.com/amitpant7/Channel-Pruning-EfficientNetV2)
        pruned 88% of channels of efficientNetV2 using LAMP pruning resulting 14x smaller model, 2.5x faster in inference, 14x fewer parameters & 2.5x fewer MACops. The loss in accuracy was somewhat 2% only.  


## Quantizing the Model
[Quantization of EfficientnetV2](https://github.com/amitpant7/Quantizing-Efficientnetv2-using-Vitis-AI-Pytorch.git)