# FONAS: FPGA Optimized Neural Architecture Search for Hardware Efficiency through Evolutionary Search

## Summary
This project focuses on searching for efficient deep neural architectures (FPGANets) tailored for image classification tasks while adhering to constraints such as arithmetic intensity and latency for FPGA deployment. Our proposed FPGANets outperform existing networks in terms of both latency and accuracy on the ImageNet-1k dataset. The project also received a research grant from LogicTronix (AMD-Xilinx Partner).

## Project Work and Methodologies
- **Compressing EfficientNet-V2**: Implementation of channel pruning techniques to reduce the model size and enhance inference speed for FPGA deployment.
- **Leveraging NAS techniques**: Automation of task-specific neural network creation to target latency requirements on FPGA platforms.
- **Hardware Optimization**: Co-designing models and hardware for improved efficiency and performance.

### Hardware NAS Focus
- **Optimization Goals**: Minimizing latency, maximizing accuracy, and efficient resource utilization on FPGA platforms.
- **Architecture Sampling**: Generating diverse architectures meeting hardware constraints like latency and resource usage.
- **Evaluation Metrics**: Assessing performance based on accuracy, inference speed, and resource utilization for optimal architecture selection.

## Key Results and Findings
- **Compressed EfficientNet-V2**: Achieved an 88% reduction in channel count resulting in a model that is 14 times smaller, 2.5 times faster in inference speed, and has significantly fewer parameters and MAC operations.
- A comprehensive latency table was developed to aid latency estimation, and an accuracy predictor was used to filter out the best performing networks.
- Over 40 million architectures within the MobileNet-V3 search space were explored, targeting the Ultra96-V2 MPSoC board.
- An evolutionary search process was employed to discover seven architectures varying in size and latency.
- FPGANet_L25 emerged as a standout, achieving a top-1 accuracy of 79.12% on ILSVRC2012 within 25ms of inference time.
- The proposed approach outperformed established networks like EfficientNet-B0, ResNet-50, and MobileNet-V3 in both inference latency (measured on FPGA) and accuracy.
- A comprehensive latency table was developed to aid latency estimation, and an accuracy predictor was used to filter out the best performing networks.
- ![res](https://github.com/FPGA-Vision/FONAS/assets/50907565/e37a749d-6905-4a5b-b943-37ee1592b7f8)
![image](https://github.com/FPGA-Vision/FONAS/assets/50907565/18099282-9379-4a48-a134-66063a0d7524)
![image](https://github.com/FPGA-Vision/FONAS/assets/50907565/959de06d-11bd-4948-a786-871d683da10b)

