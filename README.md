<div align="center">
    <h1>Awesome LLM Compression</h1>
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg"/></a>
</div>

Awesome LLM compression research papers and tools to accelerate LLM training and inference. 

# Contents

- [📑 Papers](#papers)
  - [Survey](#survey)
  - [Quantization](#quantization)
  - [Pruning and Sparsity](#pruning-and-sparsity)
  - [Distillation](#distillation)
  - [Efficient Prompting](#efficient-prompting)
  - [Other](#other)
- [🔧 Tools](#tools)
- [🙌 Contributing](#contributing)
- [🌟 Star History](#star-history)

## Papers

### Survey

- A Survey on Model Compression for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.07633)

- The Efficiency Spectrum of Large Language Models: An Algorithmic Survey <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.00678)

- Efficient Large Language Models: A Survey <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.03863) [[GitHub Page]](https://github.com/AIoT-MLSys-Lab/Efficient-LLMs-Survey)

- Towards Efficient Generative Large Language Model Serving: A Survey from Algorithms to Systems <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.15234) 

- Understanding LLMs: A Comprehensive Overview from Training to Inference <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.02038) 

- A Survey of Resource-efficient LLM and Multimodal Foundation Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.08092) 

- A Survey on Hardware Accelerators for Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.09890) 

- A Comprehensive Survey of Compression Algorithms for Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.15347)
 
- Model Compression and Efficient Inference for Large Language Models: A Survey <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.09748) 

### Quantization

- ZeroQuant: Efficient and Affordable Post-Training Quantization for Large-Scale Transformers <br> NeurIPS 2022 [[Paper]](https://arxiv.org/abs/2206.01861) [[Code (DeepSpeed)]](https://github.com/microsoft/DeepSpeed)

- LLM.int8(): 8-bit Matrix Multiplication for Transformers at Scale <br> NeurIPS 2022 [[Paper]](https://arxiv.org/abs/2208.07339) [[Code]](https://github.com/TimDettmers/bitsandbytes)

- Outlier Suppression: Pushing the Limit of Low-bit Transformer Language Models <br> NeurIPS 2022 [[Paper]](https://arxiv.org/abs/2209.13325) [[Code]](https://github.com/wimh966/outlier_suppression)

- LUT-GEMM: Quantized Matrix Multiplication based on LUTs for Efficient Inference in Large-Scale Generative Language Models <br> Arxiv 2022 [[Paper]](https://arxiv.org/abs/2206.09557) 

- SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models <br> ICML 2023 [[Paper]](https://arxiv.org/abs/2211.10438) [[Code]](https://github.com/mit-han-lab/smoothquant)

- FlexRound: Learnable Rounding based on Element-wise Division for Post-Training Quantization <br> ICML 2023 [[Paper]](https://arxiv.org/abs/2306.00317) [[Code (DeepSpeed)]](https://github.com/microsoft/DeepSpeed)

- Understanding INT4 Quantization for Transformer Models: Latency Speedup, Composability, and Failure Cases <br> ICML 2023 [[Paper]](https://arxiv.org/abs/2301.12017) [[Code]](https://openreview.net/attachment?id=-tYCaP0phY_&name=supplementary_material)

- The case for 4-bit precision: k-bit Inference Scaling Laws <br> ICML 2023 [[Paper]](https://proceedings.mlr.press/v202/dettmers23a.html)

- GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers <br> ICLR 2023 [[Paper]](https://arxiv.org/abs/2210.17323) [[Code]](https://github.com/IST-DASLab/gptq)

- PreQuant: A Task-agnostic Quantization Approach for Pre-trained Language Models <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2306.00014) 

- Boost Transformer-based Language Models with GPU-Friendly Sparsity and Quantization <br> ACL 2023 [[Paper]](https://aclanthology.org/2023.findings-acl.15.pdf) 

- QLoRA: Efficient Finetuning of Quantized LLMs <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2305.14314) [[Code]](https://github.com/artidoro/qlora)

- The Quantization Model of Neural Scaling <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2303.13506)

- Quantized Distributed Training of Large Models with Convergence Guarantees <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2302.02390)

- RPTQ: Reorder-based Post-training Quantization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2304.01089) [[Code]](https://github.com/hahnyuan/RPTQ4LLM)

- ZeroQuant-V2: Exploring Post-training Quantization in LLMs from Comprehensive Study to Low Rank Compensation <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2303.08302) [[Code]](https://github.com/microsoft/DeepSpeed)

- Integer or Floating Point? New Outlooks for Low-Bit Quantization on Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.12356)

- Memory-Efficient Fine-Tuning of Compressed Large Language Models via sub-4-bit Integer Quantization <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2305.14152)

- Compress, Then Prompt: Improving Accuracy-Efficiency Trade-off of LLM Inference with Transferable Prompt <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.11186)

- AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.00978) [[Code]](https://github.com/mit-han-lab/llm-awq)

- LLM-QAT: Data-Free Quantization Aware Training for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.17888) [[Code]](https://github.com/facebookresearch/LLM-QAT)

- SpQR: A Sparse-Quantized Representation for Near-Lossless LLM Weight Compression <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.03078) [[Code]](https://github.com/Vahe1994/SpQR)

- OWQ: Lessons learned from activation outliers for weight quantization in large language models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.02272)

- SqueezeLLM: Dense-and-Sparse Quantization <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.07629)  [[Code]](https://github.com/SqueezeAILab/SqueezeLLM)

- INT2.1: Towards Fine-Tunable Quantized Large Language Models with Error Correction through Low-Rank Adaptation <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.08162)

- INT-FP-QSim: Mixed Precision and Formats For Large Language Models and Vision Transformers <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.03712) [[Code]](https://github.com/lightmatter-ai/INT-FP-QSim)

- QIGen: Generating Efficient Kernels for Quantized Inference on Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.03738) [[Code]](https://github.com/IST-DASLab/QIGen)

- Do Emergent Abilities Exist in Quantized Large Language Models: An Empirical Study <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.08072)

- ZeroQuant-FP: A Leap Forward in LLMs Post-Training W4A8 Quantization Using Floating-Point Formats <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.09782) [[Code (DeepSpeed)]](https://github.com/microsoft/DeepSpeed)

- OliVe: Accelerating Large Language Models via Hardware-friendly Outlier-Victim Pair Quantization <br> ISCA 2023 [[Paper]](https://arxiv.org/abs/2304.07493)

- NUPES : Non-Uniform Post-Training Quantization via Power Exponent Search <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.05600)

- GPT-Zip: Deep Compression of Finetuned Large Language Models <br> ICML 2023 Workshop ES-FoMO [[Paper]](https://openreview.net/forum?id=hO0c2tG2xL)

- Generating Efficient Kernels for Quantized Inference on Large Language Models <br> ICML 2023 Workshop ES-FoMO [[Paper]](https://openreview.net/forum?id=jjazoNAf1S)

- Gradient-Based Post-Training Quantization: Challenging the Status Quo <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.07662)

- FineQuant: Unlocking Efficiency with Fine-Grained Weight-Only Quantization for LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.09723)

- OmniQuant: Omnidirectionally Calibrated Quantization for Large Language Models <br> ICLR 2024 [[Paper]](https://arxiv.org/abs/2308.13137) [[Code]](https://github.com/OpenGVLab/OmniQuant)

- FPTQ: Fine-grained Post-Training Quantization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.15987)

- eDKM: An Efficient and Accurate Train-time Weight Clustering for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.00964)

- QuantEase: Optimization-based Quantization for Language Models -- An Efficient and Intuitive Algorithm <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.01885)

- Norm Tweaking: High-performance Low-bit Quantization of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.02784)

- Understanding the Impact of Post-Training Quantization on Large-scale Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.05210)

- MEMORY-VQ: Compression for Tractable Internet-Scale Memory <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.14903)

- Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.05516) [[Code]](https://github.com/intel/neural-compressor)

- Efficient Post-training Quantization with FP8 Formats <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.14592) [[Code (Intel® Neural Compressor)]](https://github.com/intel/neural-compressor)

- QA-LoRA: Quantization-Aware Low-Rank Adaptation of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.14717) [[Code]](https://github.com/yuhuixu1993/qa-lora)

- Rethinking Channel Dimensions to Isolate Outliers for Low-bit Weight Quantization of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.15531) 

- ModuLoRA: Finetuning 3-Bit LLMs on Consumer GPUs by Integrating with Modular Quantizers <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.16119) 

- PB-LLM: Partially Binarized Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.00034) [[Code]](https://github.com/hahnyuan/PB-LLM)

- Dual Grained Quantization: Efficient Fine-Grained Quantization for LLM <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.04836) 

- Rethinking Channel Dimensions to Isolate Outliers for Low-bit Weight Quantization of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.15531) 

- QLLM: Accurate and Efficient Low-Bitwidth Quantization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.08041) 

- LoftQ: LoRA-Fine-Tuning-Aware Quantization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.08659) 

- QFT: Quantized Full-parameter Tuning of LLMs with Affordable Resources <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.07147) 

- TEQ: Trainable Equivalent Transformation for Quantization of LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.10944) [[Code (Intel® Neural Compressor)]](https://github.com/intel/neural-compressor)

- BitNet: Scaling 1-bit Transformers for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.11453) 

- FP8-LM: Training FP8 Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.18313) [[Code]](https://github.com/Azure/MS-AMP)

- QUIK: Towards End-to-End 4-Bit Inference on Generative Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.09259) [[Code]](https://github.com/IST-DASLab/QUIK)

- AFPQ: Asymmetric Floating Point Quantization for LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.01792) [[Code]](https://github.com/zhangsichengsjtu/AFPQ)

- AWEQ: Post-Training Quantization with Activation-Weight Equalization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.01305) 

- Atom: Low-bit Quantization for Efficient and Accurate LLM Serving <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.19102) 

- QMoE: Practical Sub-1-Bit Compression of Trillion-Parameter Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.16795) 

- Dissecting the Runtime Performance of the Training, Fine-tuning, and Inference of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.03687) 

- How Does Calibration Data Affect the Post-training Pruning and Quantization of Large Language Models? <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.09755)

- A Speed Odyssey for Deployable Quantization of LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.09550)

- Enabling Fast 2-bit LLM on GPUs: Memory Alignment, Sparse Outlier, and Asynchronous Dequantization <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.16442)

- Quantizable Transformers: Removing Outliers by Helping Attention Heads Do Nothing <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2306.12929) [[Code]](https://github.com/Qualcomm-AI-research/outlier-free-transformers)

- Efficient LLM Inference on CPUs <br> NeurIPS 2023 on Efficient Natural Language and Speech Processing [[Paper]](https://arxiv.org/abs/2311.00502) [[Code]](https://github.com/intel/intel-extension-for-transformers)

- The Cost of Compression: Investigating the Impact of Compression on Parametric Knowledge in Language Models <br> EMNLP Findings 2023 [[Paper]](https://arxiv.org/abs/2312.00960) 

- Zero-Shot Sharpness-Aware Quantization for Pre-trained Language Models <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.13315) 

- Revisiting Block-based Quantisation: What is Important for Sub-8-bit LLM Inference? <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.05079) [[Code]](https://github.com/ChengZhang-98/llm-mixed-q) 

- Outlier Suppression+: Accurate quantization of large language models by equivalent and optimal shifting and scaling <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2304.09145)

- Watermarking LLMs with Weight Quantization <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.11237) [[Code]](https://github.com/Twilight92z/Quantize-Watermark)

- Enhancing Computation Efficiency in Large Language Models through Weight and Activation Quantization <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2311.05161)

- LLM-FP4: 4-Bit Floating-Point Quantized Transformers <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.16836) [[Code]](https://github.com/nbasyl/LLM-FP4)

- Agile-Quant: Activation-Guided Quantization for Faster Inference of LLMs on the Edge <br> AAAI 2024 [[Paper]](https://arxiv.org/abs/2312.05693)

- SmoothQuant+: Accurate and Efficient 4-bit Post-Training WeightQuantization for LLM <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.03788)

- CBQ: Cross-Block Quantization for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.07950)

- ZeroQuant(4+2): Redefining LLMs Quantization with a New FP6-Centric Strategy for Diverse Generative Tasks <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.08583)

- QuIP: 2-Bit Quantization of Large Language Models With Guarantees <br> NeurIPS 2023 [[Paper]](https://openreview.net/pdf?id=xrk9g5vcXR) [[Code]](https://github.com/jerry-chee/QuIP)

- A Performance Evaluation of a Quantized Large Language Model on Various Smartphones <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.12472)

- FlightLLM: Efficient Large Language Model Inference with a Complete Mapping Flow on FPGA <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.03868)

- Extreme Compression of Large Language Models via Additive Quantization <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.06118)

- Quantized Side Tuning: Fast and Memory-Efficient Tuning of Quantized Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.07159)

- Inferflow: an Efficient and Highly Configurable Inference Engine for Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.08294)

- FP6-LLM: Efficiently Serving Large Language Models Through FP6-Centric Algorithm-System Co-Design <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.14112)

- KVQuant: Towards 10 Million Context Length LLM Inference with KV Cache Quantization <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.18079)

- Can Large Language Models Understand Context? <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.18079)

- AffineQuant: Affine Transformation Quantization for Large Language Models <br> EACL 2024 [[Paper]](https://browse.arxiv.org/abs/2402.00858)

- EdgeQAT: Entropy and Distribution Guided Quantization-Aware Training for the Acceleration of Lightweight LLMs on the Edge <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.10787) [[Code]](https://github.com/shawnricecake/EdgeQAT)

- Any-Precision LLM: Low-Cost Deployment of Multiple, Different-Sized LLMs <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.10517) 

- LQER: Low-Rank Quantization Error Reconstruction for LLMs <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.02446) 

- KIVI: A Tuning-Free Asymmetric 2bit Quantization for KV Cache <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.02750) [[Code]](https://github.com/jy-yuan/KIVI)

- BiLLM: Pushing the Limit of Post-Training Quantization for LLMs <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.04291) [[Code]](https://github.com/Aaronhuang-778/BiLLM)

- QuIP#: Even Better LLM Quantization with Hadamard Incoherence and Lattice Codebooks <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.04396) [[Code]](https://github.com/Cornell-RelaxML/quip-sharp)

- L4Q: Parameter Efficient Quantization-Aware Training on Large Language Models via LoRA-wise LSQ <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.04902) 

- TP-Aware Dequantization <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.04925) 

- ApiQ: Finetuning of 2-Bit Quantized Large Language Model <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.05147) 

- Accurate LoRA-Finetuning Quantization of LLMs via Information Retention <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.05445) [[Code]](https://github.com/htqin/ir-qlora)

- BitDelta: Your Fine-Tune May Only Be Worth One Bit <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.10193) [[Code]](https://github.com/FasterDecoding/BitDelta)

- QDyLoRA: Quantized Dynamic Low-Rank Adaptation for Efficient Large Language Model Tuning <br> AAAI EIW Workshop 2024 [[Paper]](https://arxiv.org/abs/2402.10462) 

- Any-Precision LLM: Low-Cost Deployment of Multiple, Different-Sized LLMs <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.10517) 

- BitDistiller: Unleashing the Potential of Sub-4-Bit LLMs via Self-Distillation <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.10631) [[Code]](https://github.com/DD-DuDa/BitDistiller)
- OneBit: Towards Extremely Low-bit Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2402.11295)


### Pruning and Sparsity

- The Lazy Neuron Phenomenon: On Emergence of Activation Sparsity in Transformers <br> ICLR 2023 [[Paper]](https://openreview.net/forum?id=TJ2nxciYCk-)

- Deja Vu: Contextual Sparsity for Efficient LLMs at Inference Time <br> ICML 2023 [[Paper]](https://proceedings.mlr.press/v202/liu23am.html)  [[Code]](https://github.com/FMInference/DejaVu)

- LoSparse: Structured Compression of Large Language Models based on Low-Rank and Sparse Approximation <br> ICML 2023 [[Paper]](https://arxiv.org/abs/2306.11222)  [[Code]](https://github.com/yxli2123/LoSparse)

- LLM-Pruner: On the Structural Pruning of Large Language Models <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2305.11627) [[Code]](https://github.com/horseee/LLM-Pruner)

- ZipLM: Inference-Aware Structured Pruning of Language Models <br> NeurIPS 2023  [[Paper]](https://arxiv.org/abs/2302.04089) [[Code]](https://github.com/IST-DASLab/ZipLM)

- H2O: Heavy-Hitter Oracle for Efficient Generative Inference of Large Language Models <br> NeurIPS 2023 [[Paper]](https://arxiv.org/pdf/2306.14048.pdf) [[Code]](https://github.com/FMInference/H2O)

- Scissorhands: Exploiting the Persistence of Importance Hypothesis for LLM KV Cache Compression at Test Time <br> NeurIPS 2023 [[Paper]](https://arxiv.org/pdf/2305.17118.pdf)

- The Emergence of Essential Sparsity in Large Pre-trained Models: The Weights that Matter <br> NeurIPS 2023 [[Paper]](https://openreview.net/pdf?id=bU9hwbsVcy) [[Code]](https://github.com/VITA-Group/essential_sparsity)

- Learning to Compress Prompts with Gist Tokens <br> NeurIPS 2023 [[Paper]](https://arxiv.org/pdf/2304.08467.pdf)

- Dynamic Context Pruning for Efficient and Interpretable Autoregressive Transformers <br> NeurIPS 2023 [[Paper]](https://openreview.net/pdf?id=uvdJgFFzby)

- Prune and Tune: Improving Efficient Pruning Techniques for Massive Language Models <br> ICLR 2023 TinyPapers [[Paper]](https://openreview.net/pdf?id=cKlgcx7nSZ)

- SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2301.00774) [[Code]](https://github.com/IST-DASLab/sparsegpt)

- Unlocking Context Constraints of LLMs: Enhancing Context Efficiency of LLMs with Self-Information-Based Content Filtering <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2304.12102) [[Code]](https://github.com/liyucheng09/Selective_Context)

- Rethinking the Role of Scale for In-Context Learning: An Interpretability-based Case Study at 66 Billion Scale <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2212.09095) [[Code]](https://github.com/amazon-science/llm-interpret)

- Structured Pruning for Efficient Generative Pre-trained Language Models <br> ACL 2023 [[Paper]](https://aclanthology.org/2023.findings-acl.692.pdf)

- A Simple and Effective Pruning Approach for Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.11695) [[Code]](https://github.com/locuslab/wanda)

- Pruning Meets Low-Rank Parameter-Efficient Fine-Tuning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.18403) 

- Structural pruning of large language models via neural architecture search <br> AutoML 2023 [[Paper]](https://www.amazon.science/publications/structural-pruning-of-large-language-models-via-neural-architecture-search) 

- Pruning Large Language Models via Accuracy Predictor <br> ICASSP 2024 [[Paper]](https://arxiv.org/abs/2309.09507) 

- Flash-LLM: Enabling Cost-Effective and Highly-Efficient Large Generative Model Inference with Unstructured Sparsity <br> VLDB 2024 [[Paper]](https://arxiv.org/abs/2309.10285) [[Cde]](https://github.com/AlibabaResearch/flash-llm)

- Compressing LLMs: The Truth is Rarely Pure and Never Simple <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.01382) 

- Junk DNA Hypothesis: A Task-Centric Angle of LLM Pre-trained Weights through Sparsity <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.02277)  [[Code]](https://github.com/VITA-Group/Junk_DNA_Hypothesis)

- Model Tells You What to Discard: Adaptive KV Cache Compression for LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.01801)  

- Compresso: Structured Pruning with Collaborative Prompting Learns Compact Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.05015) [[Code]](https://github.com/microsoft/Moonlit/tree/main/Compresso)

- Outlier Weighed Layerwise Sparsity (OWL): A Missing Secret Sauce for Pruning LLMs to High Sparsity <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.05175) [[Code]](https://github.com/luuyin/OWL)

- Sheared LLaMA: Accelerating Language Model Pre-training via Structured Pruning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.06694) [[Code]](https://github.com/princeton-nlp/LLM-Shearing)

- Dynamic Sparse No Training: Training-Free Fine-tuning for Sparse LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.08915) [[Code]](https://github.com/zxyxmu/DSnoT)

- One-Shot Sensitivity-Aware Mixed Sparsity Pruning for Large Language Models <br> ICASSP 2024 [[Paper]](https://arxiv.org/abs/2310.09499) 

- Survival of the Most Influential Prompts: Efficient Black-Box Prompt Search via Clustering and Pruning <br> EMNLP 2023 Findings [[Paper]](https://arxiv.org/abs/2310.12774) 

- The Cost of Compression: Investigating the Impact of Compression on Parametric Knowledge in Language Models <br> EMNLP Findings 2023 [[Paper]](https://arxiv.org/abs/2312.00960) 

- Divergent Token Metrics: Measuring degradation to prune away LLM components -- and optimize quantization <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.01544) 

- LoRAShear: Efficient Large Language Model Structured Pruning and Knowledge Recovery <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.18356) 

- ReLU Strikes Back: Exploiting Activation Sparsity in Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.04564) 

- E-Sparse: Boosting the Large Language Model Inference through Entropy-based N:M Sparsity <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.15929)

- Beyond Size: How Gradients Shape Pruning Decisions in Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.04902) [[Code]](https://github.com/RocktimJyotiDas/GBLM-Pruner)

- How Does Calibration Data Affect the Post-training Pruning and Quantization of Large Language Models? <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.09755)

- BESA: Pruning Large Language Models with Blockwise Parameter-Efficient Sparsity Allocation <br> OpenReview [[Paper]](https://openreview.net/pdf?id=gC6JTEU3jl) [[Code]](https://github.com/LinkAnonymous/BESA)

- PUSHING GRADIENT TOWARDS ZERO: A NOVEL PRUNING METHOD FOR LARGE LANGUAGE MODELS <br> OpenReview 2023 [[Paper]](https://openreview.net/attachment?id=IU4L7wiwxw&name=pdf)

- An Efficient Plug-and-Play Post-Training Pruning Strategy in Large Language Models <br> Preprints 2023 [[Paper]](https://www.preprints.org/manuscript/202310.1487/download/final_file)

- Lighter, yet More Faithful: Investigating Hallucinations in Pruned Large Language Models for Abstractive Summarization <br> Arxiv 2023 [[Paper]](https://arxiv.org/pdf/2311.09335.pdf) [[Code]](https://github.com/casszhao/PruneHall)

- LORAPRUNE: PRUNING MEETS LOW-RANK PARAMETER-EFFICIENT FINE-TUNING <br> Arxiv 2023 [[Paper]](https://arxiv.org/pdf/2305.18403.pdf)

- Mini-GPTs: Efficient Large Language Models through Contextual Pruning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.12682) [[Code]](https://github.com/tval2/contextual-pruning)

- The LLM Surgeon <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.17244)

- Fluctuation-based Adaptive Structured Pruning for Large Language Models <br> AAAI 2024 [[Paper]](https://arxiv.org/abs/2312.11983)

- How to Prune Your Language Model: Recovering Accuracy on the "Sparsity May Cry'' Benchmark <br> CPAL 2024 [[Paper]](https://arxiv.org/abs/2312.13547)

- PERP: Rethinking the Prune-Retrain Paradigm in the Era of LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.15230)

- Fast and Optimal Weight Update for Pruned Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.02938)

- APT: Adaptive Pruning and Tuning Pretrained Language Models for Efficient Training and Inference <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.12200)

- Scaling Sparse Fine-Tuning to Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.16405)

- SliceGPT: Compress Large Language Models by Deleting Rows and Columns <br> ICLR 2024 [[Paper]](https://arxiv.org/abs/2401.15024) [[Code]](https://github.com/microsoft/TransformerCompression)

### Distillation

- Lifting the Curse of Capacity Gap in Distilling Language Models <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2305.12129) [[Code]](https://github.com/GeneZC/MiniMoE)

- Symbolic Chain-of-Thought Distillation: Small Models Can Also "Think" Step-by-Step <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2306.14050) 

- Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2305.02301) 

- SCOTT: Self-Consistent Chain-of-Thought Distillation <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2305.01879) 

- DISCO: Distilling Counterfactuals with Large Language Models <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2212.10534) [[Code]](https://github.com/eric11eca/disco)

- LaMini-LM: A Diverse Herd of Distilled Models from Large-Scale Instructions <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2304.14402) [[Code]](https://github.com/mbzuai-nlp/LaMini-LM)

- How To Train Your (Compressed) Large Language Model <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.14864) 

- The False Promise of Imitating Proprietary LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.15717)

- GPT4All: Training an Assistant-style Chatbot with Large Scale Data Distillation from GPT-3.5-Turbo <br> Arxiv 2023 [[Paper]](https://s3.amazonaws.com/static.nomic.ai/gpt4all/2023_GPT4All_Technical_Report.pdf) [[Code]](https://github.com/nomic-ai/gpt4all)

- PaD: Program-aided Distillation Specializes Large Models in Reasoning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.13888) 

- Knowledge Distillation of Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.08543) [[Code]](https://github.com/microsoft/LMOps/tree/main/minillm)

- GKD: Generalized Knowledge Distillation for Auto-regressive Sequence Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.13649)

- Chain-of-Thought Prompt Distillation for Multimodal Named Entity and Multimodal Relation Extraction <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2306.14122)

- Task-agnostic Distillation of Encoder-Decoder Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.12330)

- Sci-CoT: Leveraging Large Language Models for Enhanced Knowledge Distillation in Small Models for Scientific QA <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.04679)

- Can a student Large Language Model perform as well as it's teacher? <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.02421)

- Multistage Collaborative Knowledge Distillation from Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2311.08640)

- Lion: Adversarial Distillation of Closed-Source Large Language Model <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2305.12870) [[Code]](https://github.com/YJiangcm/Lion)

- MCC-KD: Multi-CoT Consistent Knowledge Distillation <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.14747)

- PromptMix: A Class Boundary Augmentation Method for Large Language Model Distillation <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.14192)

- YODA: Teacher-Student Progressive Learning for Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2401.15670)

### Efficient Prompting

- Did You Read the Instructions? Rethinking the Effectiveness of Task Definitions in Instruction Learning <br> ACL 2023 [[Paper]](https://arxiv.org/abs/2306.01150) [[Code]](https://github.com/fanyin3639/Rethinking-instruction-effectiveness)

- Batch Prompting: Efficient Inference with Large Language Model APIs <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2301.08721) [[Code]](https://github.com/HKUNLP/batch-prompting) 

- Adapting Language Models to Compress Contexts <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2305.14788) [[Code]](https://github.com/princeton-nlp/AutoCompressors)

- Compressing Context to Enhance Inference Efficiency of Large Language Models <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.06201) [[Code]](https://github.com/liyucheng09/Selective_Context)

- LLMLingua: Compressing Prompts for Accelerated Inference of Large Language Models <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.05736) [[Code]](https://github.com/microsoft/LLMLingua)

- Vector-Quantized Prompt Learning for Paraphrase Generation <br> EMNLP 2023 Findings [[Paper]](https://arxiv.org/abs/2311.14949)

- Efficient Prompting via Dynamic In-Context Learning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.11170)

- Learning to Compress Prompts with Gist Tokens <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2304.08467) [[Code]](https://github.com/jayelm/gisting)

- In-context Autoencoder for Context Compression in a Large Language Model <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.06945) 

- Discrete Prompt Compression with Reinforcement Learning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.08758) 

- BatchPrompt: Accomplish more with less <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.00384) 

- (Dynamic) Prompting might be all you need to repair Compressed LLMs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.00867) 

- RECOMP: Improving Retrieval-Augmented LMs with Compression and Selective Augmentation <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.04408) [[Code]](https://github.com/carriex/recomp)

- LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.06839) [[Code]](https://github.com/microsoft/LLMLingua)

- Extending Context Window of Large Language Models via Semantic Compression <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.09571)

- Boosting LLM Reasoning: Push the Limits of Few-shot Learning with Reinforced In-Context Pruning <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.08901)

- The Impact of Reasoning Step Length on Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.04925)

### Other

- TensorGPT: Efficient Compression of the Embedding Layer in LLMs based on the Tensor-Train Decomposition <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.00526)

- Dynamic Context Pruning for Efficient and Interpretable Autoregressive Transformers <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.15805)

- SkipDecode: Autoregressive Skip Decoding with Batching and Caching for Efficient LLM Inference <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.02628)

- Scaling In-Context Demonstrations with Structured Attention <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.02690)

- Response Length Perception and Sequence Scheduling: An LLM-Empowered LLM Inference Pipeline <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2305.13144) [[Code]](https://github.com/zhengzangw/Sequence-Scheduling)

- CPET: Effective Parameter-Efficient Tuning for Compressed Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2307.07705)

- Ternary Singular Value Decomposition as a Better Parameterized Form in Linear Mapping <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2308.07641)

- LLMCad: Fast and Scalable On-device Large Language Model Inference <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.04255)

- LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.12307) [[Code]](https://github.com/dvlab-research/LongLoRA)

- LORD: Low Rank Decomposition Of Monolingual Code LLMs For One-Shot Compression <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.14021) [[Code]](https://huggingface.co/nolanoAI)

- Mixture of Tokens: Efficient LLMs through Cross-Example Aggregation <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2310.15961) 

- Efficient Streaming Language Models with Attention Sinks <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2309.17453) [[Code]](https://github.com/mit-han-lab/streaming-llm)

- Efficient Large Language Models Fine-Tuning On Graphs <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.04737)

- SparQ Attention: Bandwidth-Efficient LLM Inference <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.04985)

- Rethinking Compression: Reduced Order Modelling of Latent Features in Large Language Models <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.07046) 

- PowerInfer: Fast Large Language Model Serving with a Consumer-grade GPU <br> Arxiv 2023 [[Paper]](https://arxiv.org/abs/2312.12456)  [[Code]](https://github.com/SJTU-IPADS/PowerInfer)

- Dataset Quantization <br> ICCV 2023 [[Paper]](https://arxiv.org/abs/2308.10524) [[Code]](https://github.com/magic-research/Dataset_Quantization)

- Text Alignment Is An Efficient Unified Model for Massive NLP Tasks <br> NeurIPS 2023 [[Paper]](https://arxiv.org/abs/2307.02729) [[Code]](https://github.com/yuh-zha/Align)

- Context Compression for Auto-regressive Transformers with Sentinel Tokens <br> EMNLP 2023 [[Paper]](https://arxiv.org/abs/2310.08152) [[Code]](https://github.com/DRSY/KV_Compression)

- TCRA-LLM: Token Compression Retrieval Augmented Large Language Model for Inference Cost Reduction <br> EMNLP 2023 Findings [[Paper]](https://arxiv.org/abs/2310.15556)

- Retrieval-based Knowledge Transfer: An Effective Approach for Extreme Large Language Model Compression <br> EMNLP 2023 Findings [[Paper]](https://arxiv.org/abs/2310.15594)

- FFSplit: Split Feed-Forward Network For Optimizing Accuracy-Efficiency Trade-off in Language Model Inference <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.04044)

- LoMA: Lossless Compressed Memory Attention <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.09486)

- Medusa: Simple LLM Inference Acceleration Framework with Multiple Decoding Heads <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.10774) [[Code]](https://github.com/FasterDecoding/Medusa)

- BiTA: Bi-Directional Tuning for Lossless Acceleration in Large Language Models <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.12522) [[Code]](https://github.com/linfeng93/BiTA)

- CompactifAI: Extreme Compression of Large Language Models using Quantum-Inspired Tensor Networks <br> Arxiv 2024 [[Paper]](https://arxiv.org/abs/2401.14109)

## Tools

- BMCook: Model Compression for Big Models [[Code]](https://github.com/OpenBMB/BMCook)
  
- llama.cpp: Inference of LLaMA model in pure C/C++ [[Code]](https://github.com/ggerganov/llama.cpp)

- LangChain: Building applications with LLMs through composability [[Code]](https://github.com/hwchase17/langchain)

- GPTQ-for-LLaMA: 4 bits quantization of LLaMA using GPTQ [[Code]](https://github.com/qwopqwop200/GPTQ-for-LLaMa)

- Alpaca-CoT: An Instruction Fine-Tuning Platform with Instruction Data Collection and Unified Large Language Models Interface [[Code]](https://github.com/PhoebusSi/Alpaca-CoT)

- vllm: A high-throughput and memory-efficient inference and serving engine for LLMs [[Code]](https://github.com/vllm-project/vllm)

- LLaMA Efficient Tuning: Fine-tuning LLaMA with PEFT (PT+SFT+RLHF with QLoRA) [[Code]](https://github.com/hiyouga/LLaMA-Efficient-Tuning)

- gpt-fast: Simple and efficient pytorch-native transformer text generation in <1000 LOC of python. [[Code]](https://github.com/pytorch-labs/gpt-fast)

- Efficient-Tuning-LLMs: (Efficient Finetuning of QLoRA LLMs). QLoRA, LLama, bloom, baichuan-7B, GLM [[Code]](https://github.com/jianzhnie/Efficient-Tuning-LLMs)

- bitsandbytes: 8-bit CUDA functions for PyTorch [[Code]](https://github.com/TimDettmers/bitsandbytes)

- ExLlama: A more memory-efficient rewrite of the HF transformers implementation of Llama for use with quantized weights. [[Code]](https://github.com/turboderp/exllama)

- lit-gpt: Hackable implementation of state-of-the-art open-source LLMs based on nanoGPT. Supports flash attention, 4-bit and 8-bit quantization, LoRA and LLaMA-Adapter fine-tuning, pre-training. [[Code]](https://github.com/Lightning-AI/lit-gpt)

- Lit-LLaMA: Implementation of the LLaMA language model based on nanoGPT. Supports flash attention, Int8 and GPTQ 4bit quantization, LoRA and LLaMA-Adapter fine-tuning, pre-training. [[Code]](https://github.com/Lightning-AI/lit-llama)

- lama.onnx: LLaMa/RWKV onnx models, quantization and testcase [[Code]](https://github.com/tpoisonooo/llama.onnx)

- fastLLaMa: An experimental high-performance framework for running Decoder-only LLMs with 4-bit quantization in Python using a C/C++ backend. [[Code]](https://github.com/PotatoSpudowski/fastLLaMa)

- Sparsebit: A model compression and acceleration toolbox based on pytorch. [[Code]](https://github.com/megvii-research/Sparsebit)

- llama2.c: Inference Llama 2 in one file of pure C [[Code]](https://github.com/karpathy/llama2.c)

- Megatron-LM: Ongoing research training transformer models at scale [[Code]](https://github.com/NVIDIA/Megatron-LM)

- ggml: Tensor library for machine learning [[Code]](https://github.com/ggerganov/ggml)

- LLamaSharp: C#/.NET binding of llama.cpp, including LLaMa/GPT model inference and quantization, ASP.NET core integration and UI [[Code]](https://github.com/SciSharp/LLamaSharp)

- rwkv.cpp: NT4/INT5/INT8 and FP16 inference on CPU for RWKV language model [[Code]](https://github.com/saharNooby/rwkv.cpp)

- Can my GPU run this LLM?: Calculate GPU memory requirement & breakdown for training/inference of LLM models. Supports ggml/bnb quantization [[Code]](https://github.com/RahulSChand/gpu_poor)

- TinyChatEngine: On-Device LLM Inference Library [[Code]](https://github.com/mit-han-lab/TinyChatEngine)

- TensorRT-LLM: TensorRT-LLM provides users with an easy-to-use Python API to define Large Language Models (LLMs) and build TensorRT engines that contain state-of-the-art optimizations to perform inference efficiently on NVIDIA GPUs. [[Code]](https://github.com/NVIDIA/TensorRT-LLM)

- IntLLaMA: A fast and light quantization solution for LLaMA [[Code]](https://github.com/megvii-research/IntLLaMA)

- EasyLLM: Built upon Megatron-Deepspeed and HuggingFace Trainer, EasyLLM has reorganized the code logic with a focus on usability. While enhancing usability, it also ensures training efficiency [[Code]](https://github.com/ModelTC/EasyLLM)

- GreenBit LLaMA: Advanced Ultra-Low Bitrate Compression Techniques for the LLaMA Family of LLMs [[Code]](https://github.com/GreenBitAI/low_bit_llama)

## Contributing

This is an active repository and your contributions are always welcome! Before you add papers/tools into the awesome list, please make sure that:

- The paper or tools is related to **Large Language Models (LLMs)**. If the compression algorithms or tools are only evaluated on small-scale language models (e.g., BERT), they should not be included in the list.
- The paper should be inserted in the correct position in chronological order (publication/arxiv release time). 
- The link to [Paper] should be the arxiv page, not the pdf page if this is a paper posted on arxiv.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=HuangOwen/Awesome-LLM-Compression&type=Date)](https://star-history.com/#HuangOwen/Awesome-LLM-Compression&Date)

