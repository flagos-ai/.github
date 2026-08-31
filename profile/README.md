# FlagOS: A Unified, Open-Source AI System Software Stack

[![GitHub License](https://img.shields.io/github/license/flagos-ai/.github?style=flat-square)](https://github.com/flagos-ai/.github/blob/main/LICENSE) 

**Language:** [English](README.md) | [中文](README_zh.md)

---

## 📖 About FlagOS

FlagOS is a unified, open-source AI system software stack designed for multi-chip scenarios. It was jointly initiated and established by over ten domestic and international organizations, including chip companies, system manufacturers, algorithm and software-related entities, non-profit organizations, and research institutions.

Addressing core pain points in utilizing diverse AI chips, FlagOS builds a comprehensive system software ecosystem that demonstrates the potential to break down ecosystem barriers between different chip software stacks, effectively reducing migration costs for developers.

---

## 🎯 Core Components

Components are grouped by the SIG that owns them. See the [SIG overview](https://github.com/flagos-ai/community/tree/main/sigs) for charters, owners, and meeting calendars.

| SIG | Purpose | Repository |
|-----|---------|------------|
| [**sig-operator**](https://github.com/flagos-ai/community/tree/main/sigs/sig-operator) | Operator libraries: implementation, performance optimization, and multi-chip adaptation | [FlagGems](https://github.com/flagos-ai/FlagGems), [FlagAttention](https://github.com/flagos-ai/FlagAttention), [FlagFFT](https://github.com/flagos-ai/FlagFFT), [FlagSparse](https://github.com/flagos-ai/FlagSparse), [FlagDNN](https://github.com/flagos-ai/FlagDNN), [FlagBLAS](https://github.com/flagos-ai/FlagBLAS), [FlagTensor](https://github.com/flagos-ai/FlagTensor), [FlagAudio](https://github.com/flagos-ai/FlagAudio) |
| [**sig-compiler**](https://github.com/flagos-ai/community/tree/main/sigs/sig-compiler) | Unified AI compiler: IR design, optimization passes, and multi-chip code generation | [FlagTree](https://github.com/flagos-ai/FlagTree) |
| [**sig-network**](https://github.com/flagos-ai/community/tree/main/sigs/sig-network) | Unified communication library: collective communication and multi-chip, multi-node tuning | [FlagCX](https://github.com/flagos-ai/FlagCX) |
| [**sig-framework**](https://github.com/flagos-ai/community/tree/main/sigs/sig-framework) | Framework adapter layer for PyTorch, vLLM, SGLang, TransformerEngine, Megatron-LM, and veRL | [Torch-FL](https://github.com/flagos-ai/Torch-FL), [vllm-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL), [sglang-plugin-FL](https://github.com/flagos-ai/sglang-plugin-FL), [TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL), [Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL), [verl-FL](https://github.com/flagos-ai/verl-FL) |
| [**sig-training**](https://github.com/flagos-ai/community/tree/main/sigs/sig-training) | Training and inference orchestration: parallelism strategies, recipes, and Hugging Face integration | [FlagScale](https://github.com/flagos-ai/FlagScale) |
| [**sig-kernelgen**](https://github.com/flagos-ai/community/tree/main/sigs/sig-kernelgen) | AI-assisted kernel code generation and its evaluation | [KernelGen](https://github.com/flagos-ai/KernelGen), [KernelGenBench](https://github.com/flagos-ai/KernelGenBench) |
| [**sig-chip**](https://github.com/flagos-ai/community/tree/main/sigs/sig-chip) | Datacenter chip adaptation: vendor SDK integration, bring-up, and multi-chip CI | No dedicated repository; adaptation lands in the module repositories above |
| [**wg-embodied**](https://github.com/flagos-ai/community/tree/main/wg/wg-embodied) *(incubating)* | Robotics and embodied intelligence | [FlagOS-Robo](https://github.com/flagos-ai/FlagOS-Robo) |
| [**wg-ai4s**](https://github.com/flagos-ai/community/tree/main/wg/wg-ai4s) *(incubating)* | AI for Science, including quantum simulation | [FlagQuantum](https://github.com/flagos-ai/FlagQuantum) |
| [**sig-tools**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-tools.md) *(planned)* | Release management toolchain | [FlagRelease](https://github.com/flagos-ai/FlagRelease) |
| [**sig-agent**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-agent.md) *(planned)* | Skill packages for agents to complete tasks in a specific domain | [skills](https://github.com/flagos-ai/skills) |
| [**sig-benchmark**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-benchmark.md) *(planned)* | Multi-chip performance benchmarking and evaluation | [FlagPerf](https://github.com/flagos-ai/FlagPerf) |

---

## 🚀 Extended Ecosystem Components

### Developer Tools & Utilities

- **[KernelGenBench](https://github.com/flagos-ai/KernelGenBench)**: A benchmark framework for evaluating LLM and agent-based Triton kernel generation across multiple hardware platforms.

- **[libtriton_jit](https://github.com/flagos-ai/libtriton_jit)**: Triton JIT C++ runtime for reduced Python overhead.

### Framework Enhancements

- **[Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)**: GPU-optimized library for training transformer models at scale

- **[TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)**: FP8 mixed precision training for transformer models

- **[verl-FL](https://github.com/flagos-ai/verl-FL)**: A fork of verl designed to support diverse AI accelerators, built on top of FlagOS.

- **[Torch-FL](https://github.com/flagos-ai/Torch-FL)**: A custom PyTorch device plugin based on the `PrivateUse1` extension mechanism, registering FlagGems high-performance Triton operators as the flagos device backend for unified multi-chip support.

### Inference & Serving

- **[vLLM-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL)**: Advanced vLLM plugin for enhanced multi-chip support

- **[sglang-plugin-FL](https://github.com/flagos-ai/sglang-plugin-FL)**: An out-of-tree (OOT) plugin for SGLang, built on FlagOS's unified multi-chip backend 

### Domain-specific Operator Libraries

- **[FlagDNN](https://github.com/flagos-ai/FlagDNN)**: A deep neural network computing library oriented towards multiple chip backends.

- **[FlagBLAS](https://github.com/flagos-ai/FlagBLAS)**: A computing library that follows the BLAS standard interface and is oriented towards multiple chip backends.

- **[FlagFFT](https://github.com/flagos-ai/FlagFFT)**: Efficient algorithms that convert signals or data between the time/spatial domain and the frequency domain in
operations targeting multiple chip backends.

- **[FlagSparse](https://github.com/flagos-ai/FlagSparse)**: A package for sparse operations (SpMV, gather, scatter, sparse formats) targeting multiple chip backends.

- **[FlagTensor](https://github.com/flagos-ai/FlagTensor)**: A package for high-performance tensor operators targeting multiple chip backends.

- **[FlagAudio](https://github.com/flagos-ai/FlagAudio)**: A package for high-performance audio data processing targeting multiple chip backends.

- **[FlagAttention](https://github.com/flagos-ai/FlagAttention)**: A package for memory-efficient attention operators, initiated as an extension of multi-head attention.

- **[FlagGems-vLLM](https://github.com/flagos-ai/FlagGems-vllm)**: A collection of optimized implementations of common vLLM operators and supports high-performance inference and deployment for a variety of widely used models.

### Community & Resources

- **[EasyOfUse](https://github.com/flagos-ai/EasyOfUse)**: Simplify development for open compute - plug-and-play solutions and best practices.

- **[Community](https://github.com/flagos-ai/community)**: FlagOS community governance, contribution guides, and communication hub.

---

## 📚 Documentation & Resources

### Knowledge Base

- **FlagOS Wiki & Documentation**: [DeepWiki Portal](https://flagos-wiki.baai.ac.cn/)
- **Latest Release v1.5**: [Announcement](https://mp.weixin.qq.com/s/BCryw30j_eMwe0Pr80VtcA)

### Model Repositories

- **ModelScope**: [FlagRelease Models](https://modelscope.cn/organization/FlagRelease)
- **Hugging Face**: [FlagRelease Models](https://huggingface.co/FlagRelease/models)
- **WiseModel**: [FlagRelease Models](https://www.wisemodel.cn/organization/FlagRelease)

### Community Channels

- **WeChat Official Account**: FlagOpen
- **WeChat Channels Account**: FlagOpen

---

## 🌐 Join the Community

**Ready to contribute or learn more?** Visit the [FlagOS Community Repository](https://github.com/flagos-ai/community) for:
- 📖 Comprehensive contribution guidelines
- 💬 Community discussions and support
- 🤝 Ways to get involved
- 📚 Resources and documentation

---

## 💕 Contributing

We welcome contributions from the community! Whether through starring, forking, or submitting pull requests, your involvement helps make FlagOS better.

- ⭐ **Star** - Show your support!
- 🔔 **Watch** - Stay updated with our latest releases
- 🍴 **Fork** - Start contributing!

### Code of Conduct
Please read and respect our Code of Conduct:
- **[Code of Conduct](https://github.com/flagos-ai/community/blob/main/CODE_OF_CONDUCT.MD)** (English)

---

## 📄 License

FlagOS and its components are licensed under the Apache License 2.0. See individual repositories for details.

---

## 🤝 Partners & Contributors

FlagOS is jointly supported by leading organizations in chip manufacturing, system software, and AI research. This collaborative effort demonstrates the commitment to building an open, unified ecosystem for AI system software across diverse hardware platforms.

---

**Join us in building the future of AI system software! 🚀**
