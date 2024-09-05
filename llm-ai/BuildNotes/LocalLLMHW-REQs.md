# Local LLM Hardware REquirements


CPU Extensions
- AVX2 - Advanced Vector Extensions 2


Models with FP32 and FP16 precision usually need to run on GPU servers, while models with INT8 and INT4 precision can run on CPUs.
https://medium.com/@tubelwj/introduction-to-ai-model-quantization-formats-dc643bfc335c


GPTQ runs faster on GPUs, while GGML runs faster on CPUs.

https://medium.com/@tubelwj/introduction-to-ai-model-quantization-formats-dc643bfc335c


Recommendations
If you’re interested in updating your machine to more efficiently run LLMs locally, you would generally want a GPU with a large amount of VRAM (Video Random Access Memory) to handle the memory-intensive operations involved in processing these models. GPUs with higher CUDA core counts and memory bandwidth can also contribute to faster computation.

In order to ensure your system can handle hefty local LLM hardware requirements, we recommend you double check the available RAM and VRAM based on these specifications:

Llama2 7B, a model trained by Meta AI optimized for completing general tasks.
Requires a minimum of 5.6GB RAM for the CPU model and 5.6GB of VRAM for the GPU-accelerated model.
Mistral 7B, a dense Transformer, fast-deployed and fine-tuned on code datasets. Small, yet powerful for a variety of use cases.
Requires a minimum of 6GB RAM for the CPU model and 6GB of VRAM for the GPU-accelerated model.
Phi-2 2.7B, a small language model that demonstrates outstanding reasoning and language understanding capabilities.
Requires a minimum of 3.1GB RAM for the CPU model and 3.1GB of VRAM for the GPU-accelerated model.

https://code.pieces.app/blog/how-to-run-an-llm-locally-with-pieces


https://www.reddit.com/r/LocalLLaMA/comments/13f5gwn/home_llm_hardware_suggestions/


https://www.techpowerup.com/gpu-specs/tesla-p40.c2878 



The two recommended CPU platforms are Intel Xeon W and AMD Threadripper Pro. 

 As a rule of thumb, at least 4 cores for each GPU accelerator is recommended. However, if your workload has a significant CPU compute component then 32 or even 64 cores could be ideal. In any case, a 16-core processor would generally be considered minimal for this type of workstation.

 The first rule of thumb is to have at least double the amount of CPU memory as there is total GPU memory in the system. For example, a system with 2x GeForce RTX 3090 GPUs would have 48GB of total VRAM – so the system should be configured with 128GB (96GB would be double, but 128GB is usually the closest configurable amount).

 https://www.pugetsystems.com/solutions/ai-and-hpc-workstations/machine-learning-ai/hardware-recommendations/ 

 https://www.pugetsystems.com/solutions/ai-and-hpc-workstations/machine-learning-ai/hardware-recommendations/ 

 https://lambdalabs.com/  - note Desktops

 